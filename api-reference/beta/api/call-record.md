---
title: '通話: レコード'
description: 通話を録音します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 473816bb52d441b4111632a69d767319ff59a17e
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062013"
---
# <a name="call-record"></a>通話: レコード

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通話から短いオーディオクリップを録音します。 これは、ボットがプロンプトに従って発信者からの音声応答を取得したい場合に便利です。

> [!Note]
> Record アクションは、 [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)を使用して開始された[通話](../resources/call.md)に対してのみサポートされます。 この操作では、呼び出し全体が記録されることはありません。 録音の最大長は5分です。 レコーディングは、クラウドコミュニケーションプラットフォームによって permamently には保存されず、通話が終了した直後に破棄されます。 Bot は、録音操作が終了した後で、(完了した通知で指定された**recordingLocation**値を使用して) すぐにレコーディングをダウンロードする必要があります。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
| :-------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | サポート対象外        |
| 委任 (個人用 Microsoft アカウント) | サポート対象外        |
| アプリケーション     | Calls.AccessMedia.All                       |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a>要求ヘッダー
| 名前          | 説明               |
|:--------------|:--------------------------|
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター      | 型    |説明|
|:---------------|:--------|:----------|
|促し|[Mediaprompt](../resources/mediaprompt.md)コレクション | レコーディングの開始前に再生するプロンプトのコレクション (ある場合)。 ユーザーは、"playPrompt" アクションを個別に指定するか、"record" の一部として指定することができます。ほとんどすべてのレコードはプロンプトで preceeded れます。 Current support は、コレクションの一部として1つのプロンプトのみを対象としています。 |
|bargeInAllowed|Boolean| True の場合、このレコードの要求は、キューに登録されている他の既存のレコード/再生プロンプト要求になります。 既定値は false です。 |
|initialSilenceTimeoutInSeconds | Int32| 操作を開始する前にレコード操作を開始するときに許容される最大初期無音時間 (ユーザー無音)。 プロンプトを再生している場合は、プロンプトが終了した後、このタイマーが開始されます。 既定値 = 5 秒、最小値 = 1 秒、最大 = 300 秒 |
|maxSilenceTimeoutInSeconds|Int32| ユーザーが話し始めた後に許可される最大無音時間 (一時停止時間)。 既定値は5秒、最小値は1秒、最大値は300秒です。|
|maxRecordDurationInSeconds|Int32| レコーディングを停止する前のレコード操作の最大期間。 既定値は5秒、最小値は1秒、最大値は300秒です。|
|再生のビープ音|Boolean| True の場合は、ユーザーにメッセージの録音を開始できることを示す警告音を鳴らします。 既定値は true です。|
|stopTones|文字列コレクション|録音を終了するために指定されたトーンを停止します。|
|clientContext|String|一意のクライアントコンテキスト文字列。 最大256文字を使用できます。|

## <a name="response"></a>応答
このメソッドは、 `200 OK`応答コードと、この要求に対して作成された[RECORDOPERATION](../resources/recordoperation.md)への URI を持つ Location ヘッダーを返します。

## <a name="example"></a>例
次の例は、この API を呼び出す方法を示しています。

##### <a name="request"></a>要求
次の例は要求を示しています。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/record
Content-Type: application/json
Content-Length: 394

{
  "bargeInAllowed": true,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      }
    }
  ],
  "maxRecordDurationInSeconds": 10,
  "initialSilenceTimeoutInSeconds": 5,
  "maxSilenceTimeoutInSeconds": 2,
  "playBeep": true,
  "stopTones": [ "#", "1", "*" ]
}
```
# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答
次の例は応答を示しています。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a>通知-操作が完了しました

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed",
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

##### <a name="get-recording-file---request"></a>レコーディングファイルの取得-要求
次の例は、レコーディングの内容を取得する要求を示しています。

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="get-recording-file---response"></a>レコーディングファイル応答の取得
以下は、応答の例です。 

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
  "truncated": true
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Transfer-Encoding: chunked
Date: Thu, 17 Jan 2019 01:46:37 GMT
Content-Type: application/octet-stream

(application/octet-stream of size 160696 bytes)
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
