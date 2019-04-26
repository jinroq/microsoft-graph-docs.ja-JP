---
title: デバイス コマンドの状態を取得する
description: デバイス上のコマンドの状態を取得します。 状態コードの完全な一覧については、「actionstatus の一覧」を参照してください。
localization_priority: Normal
ms.openlocfilehash: 9b914cdfde78ce50df812acb09dc034c978c7e08
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324998"
---
# <a name="get-device-command-status"></a>デバイス コマンドの状態を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

デバイス上のコマンドの状態を取得します。 状態コードの完全な一覧については、「 [actionstatus の一覧](#list-of-actionstatus)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | サポートされていません。    |
|委任 (個人用 Microsoft アカウント) | Device.Command    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー |値
|:----|:------|
|Authorization| ベアラー {トークン}。必須。 |
|承諾 | application/json |

## <a name="response"></a>応答
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a>actionstatus の一覧

- 要求のコマンドが作成され、処理を待っています
- 送信ターゲット、//コマンドがターゲットデバイスに送信されました
- コマンドを実行中で、ターゲットデバイスの確認済み受信を実行中です。
- 完了、//コマンドの実行が完了
- 失敗/送信、//サービスがターゲットデバイスにコマンドを送信できませんでした
- executionfailed、//コマンドの実行に失敗しました
- デバイスが connectedstandby の状態にある場合、コマンドはクライアントによってドロップされています。
- cancel、コマンドをキャンセルする
- コマンドをキャンセルする、//キャンセルする
- 取り消し済み//コマンドは取り消されました
- 再試行、//サービスはターゲットへのコマンドの送信を再試行しています
- 期限切れ、コマンド処理が有効期限を超過しました
- エラー、コマンドの処理中に内部エラーが発生しました
- カスタム/カスタム状態

## <a name="example"></a>例

この例では、デバイスの id と、デバイスに発行されたコマンドの id が必要になります。 デバイス ID は GET 呼び出し`/me/devices`を発行したときに返され、に対して`/me/devices/{id}/command`POST 呼び出しを実行すると、コマンド id が返されます。

#### <a name="request"></a>要求

次の例は要求を示しています。

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>応答

次の例は応答を示しています。
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a>コマンドペイロードの取得

デバイス上の特定のアクションの応答ペイロードを取得します。 応答ペイロードは、アプリケーションサービスに対してクエリを実行してデータを返すときに使用されます。


### <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | サポートされていません。    |
|委任 (個人用 Microsoft アカウント) | Device.Command    |
|アプリケーション | サポートされていません。 |

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a>要求ヘッダー

| ヘッダー |値
|:----|:------|
|Authorization| ベアラー {トークン}。必須。 |
|承諾 | application/json |

### <a name="response"></a>応答
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a>例

この例では、デバイスの id と、デバイスに発行されたコマンドの id が必要になります。 デバイス ID は GET 呼び出し`/me/devices`を発行したときに返され、に対して`/me/devices/{id}/command`POST 呼び出しを実行すると、コマンド id が返されます。

#### <a name="request"></a>要求

次の例は要求を示しています。

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>応答

次の例は応答を示しています。

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```
