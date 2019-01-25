---
title: デバイス コマンドのステータスを取得します。
description: デバイス上には、コマンドのステータスを取得します。 ステータス コードの完全なリスト、actionStatus のリストを参照してください。
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510114"
---
# <a name="get-device-command-status"></a>デバイス コマンドのステータスを取得します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

デバイス上には、コマンドのステータスを取得します。 ステータス コードの完全なリスト、 [actionStatus のリスト](#list-of-actionstatus)を参照してください。

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

## <a name="list-of-actionstatus"></a>ActionStatus の一覧

- 要求、またはコマンドで作成された、処理を待機しています。
- sentToTarget、またはターゲット ・ デバイスに送信されたコマンド/
- 実行するとターゲット ・ デバイスは、コマンドの受信を確認し、実行しています。
- 完了すると、コマンドの実行が完了しました
- failedToSend、またはターゲット ・ デバイスにコマンドを送信するサービスが失敗したと
- executionFailed、または、コマンドの実行に失敗しました
- commandDropped、またはデバイスは ConnectedStandby の状態にある場合に、コマンドがクライアントによって削除/
- 取り消すには、//コマンドのキャンセル
- キャンセルする、またはコマンドをキャンセルすると
- キャンセルするには、//、コマンドは取り消されました
- 再試行、またはサービスがターゲットにコマンドを送信する再試行/
- 有効期限が切れた、またはコマンドの処理の有効期限を超過すると
- エラー、または内部またはコマンドの処理中にエラー
- カスタム/カスタム/ステータス

## <a name="example"></a>例

この例では、デバイスの ID とデバイスに発行されたコマンドの ID を必要があります。 GET を発行するときに ID が返されるデバイスの呼び出しの`/me/devices`の投稿を行うときに ID が返されるコマンドを呼び出すと`/me/devices/{id}/command`。

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
  "@odata.type": "microsoft.graph.commandobject",
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


## <a name="get-command-payload"></a>コマンドのペイロードを取得します。

デバイス上の特定のアクションの応答の内容を取得します。 応答の内容は、データを再度実行するために、アプリケーション サービスを照会するときに使用されます。


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

この例では、デバイスの ID とデバイスに発行されたコマンドの ID を必要があります。 に対して GET を発行するときに ID が返されるデバイスを呼び出す`/me/devices`の投稿を行うときに ID が返されるコマンドを呼び出すと`/me/devices/{id}/command`。

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
  "@odata.type": "microsoft.graph.commandobject",
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/get-device-command-status.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
