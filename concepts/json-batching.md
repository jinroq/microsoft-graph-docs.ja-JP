---
title: JSON バッチ処理を使用した複数要求の単一 HTTP 呼び出しへの統合
description: JSON のバッチ処理を使用すると、複数の要求を単一の JSON オブジェクトに統合することにより、アプリケーションを最適化することができます。たとえば、次のような互いに無関係なデータからビューを作成する場合、
author: piotrci
ms.openlocfilehash: d41fb252b9c5c1c1b8f6260b5b45244fc0b32b8b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323227"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a>JSON バッチ処理を使用した複数要求の単一 HTTP 呼び出しへの統合

JSON のバッチ処理を使用すると、複数の要求を単一の JSON オブジェクトに統合することにより、アプリケーションを最適化することができます。たとえば、次のような互いに無関係なデータからビューを作成する場合、

1. OneDrive に保存されているイメージ
2. Planner タスクのリスト
3. グループの予定表

これらの 3 つの要求を 1 つのバッチ要求にまとめることで、ネットワーク待機時間を大きく削減できます。

## <a name="first-json-batch-request"></a>JSON の最初のバッチ要求

まず、前の例の JSON バッチ要求を作成します。このシナリオでは、各要求に相互の依存関係はありません。よって、バッチ要求には、各要求を任意の順序で配置できます。

```http
POST https://graph.microsoft.com/v1.0/$batch
Accept: application/json
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "/me/drive/root:/{file}:/content"
    },
    {
      "id": "2",
      "method": "GET",
      "url": "/me/planner/tasks"
    },
    {
      "id": "3",
      "method": "GET",
      "url": "/groups/{id}/events"
    },
    {
      "id": "4",
      "url": "/me",
      "method": "PATCH",
      "body": {
        "city" : "Redmond"
      },
      "headers": {
        "Content-Type": "application/json"
      }
    }
  ]
}
```

バッチ要求への応答は、異なる順序で返されることがあります。`id` プロパティを使い、各要求と応答を対応させることができます。

```http
200 OK
Content-Type: application/json
```

```json
{
  "responses": [
    {
      "id": "1",
      "status": 302,
      "headers": {
        "location": "https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi"
      }
    },
    {
      "id": "3",
      "status": 401,
      "body": {
        "error": {
          "code": "Forbidden",
          "message": "..."
        }
      }
    },
    {
      "id": "2",
      "status": 200,
      "body": {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    },
    {
      "id": "4",
      "status": 204,
      "body": null
    }
  ]
}
```

## <a name="request-format"></a>要求の形式

バッチ要求は常に `/$batch` エンドポイントに対して `POST` を使用して送信されます。

JSON バッチ要求本文は必須のプロパティ `requests` をもつ単一の JSON オブジェクトです。`requests` プロパティは個別要求の配列です。個別要求には、それぞれ `id`、`method`、および`url` プロパティが必要です。


            `id` プロパティは主に個別の応答と要求を関連付けるための相互関係値として機能します。これにより、サーバーでは最も効率のよい順序でバッチの要求処理が可能となります。


            `method` および `url` プロパティは、指定した任意の HTTP 要求の先頭と同一のものです。メソッドは HTTP であり、URL は各要求が通常送信される宛先のリソースの URL です。

個々の要求は、任意で、`headers` プロパティと `body` プロパティを含むこともできます。 これら両方のプロパティは、前の例のように、通常 JSON オブジェクトです。 場合によっては、`body` は JSON オブジェクトではなく、Base64 で URL エンコードされた値となることがあります。たとえば、本文が画像である場合などです。 要求に `body` が含まれている場合、`headers` オブジェクトには `Content-Type` の値が含まれている必要があります。

## <a name="response-format"></a>応答の形式

JSON バッチ要求への応答の形式は、要求の形式と似ています。主な違いを以下に示します。

* メインの JSON オブジェクトのプロパティは、`requests` ではなく、`responses` と命名されている。
* 個々の応答は、要求と異なる順序で返されることがある。
* `method` と `url` ではなく、個々の応答には `status` プロパティが存在する。`status` の値は、HTTP ステータス コードを表す数字である。

バッチ応答のステータス コードは、通常 `200` または `400` です。バッチ要求自体が正しい形式でない場合、状態コードは `400` になります。バッチ要求が解析可能であれば、状態コードは `200` になります。バッチ応答のステータス コード `200` はバッチ内の個々の要求が成功したことを示すものではありません。そのため、`responses` プロパティの個々の応答にステータス コードがあります。

`responses` プロパティに加え、バッチ応答には `nextLink` プロパティが存在することがあります。これにより、Microsoft Graph が個々の要求が完了するとすぐにバッチ応答を返すようにできます。個々の応答を確実にすべて受信するため、`nextLink` が存在する限りそのリンクを追い続けます。

## <a name="sequencing-requests-with-the-dependson-property"></a>dependsOn プロパティによる要求の順序指定

`dependsOn` プロパティを使い、個別の要求の実行順序を指定できます。このプロパティは個別の要求の `id` を参照する文字列の配列です。このため、`id` の値は一意である必要があります。たとえば、次の要求で、クライアントは要求 1 と 3 を先に実行し、その後に 2 そして 4 を実行するよう指定しています。

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "2",
      "dependsOn": [ "1" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

個々の要求が失敗した場合、その要求に依存するすべての要求が失敗し、ステータス コードは `424` (Failed Dependency) になります。

## <a name="bypassing-url-length-limitations-with-batching"></a>バッチ処理による URL 長さ制限の回避

他にも、URL の長さの制限を回避するために JSON バッチ処理を利用できます。フィルター句が複雑な場合、URL の長さがブラウザーまたはその他の HTTP クライアントによる制限を超えることがあります。JSON バッチ処理を使うと、長い URL は単純に要求のペイロードとなるため、制限を回避できます。

## <a name="known-issues"></a>既知の問題

バッチ処理に関連する現在の制限事項の一覧は「[既知の問題][batching-known-issues]」を参照してください。

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a>関連項目

JSON のバッチ要求/応答形式の詳細については「[OData JSON 形式バージョン 4.01 仕様][odata-4.01-json]」のセクション 18 を参照してください。この仕様は現在ドラフト バージョンですが、変更の予定はありません。

