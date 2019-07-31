---
author: JeremyKelley
description: ドライブ項目の共有への招待を送信します。
ms.date: 09/10/2017
title: アイテムにアクセスするための招待状を送信する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 116024447d21edc353f8d774c30d32aae8c4e8fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957083"
---
# <a name="send-a-sharing-invitation"></a>共有の招待状を送信する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**DriveItem** の共有の招待状を送信します。共有の招待状は受信者にアクセス許可を提供します。また、任意で受信者に、アイテムが共有されたことを通知する電子メールを送信します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| パラメーター        | 型                                            | 説明                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| Recipients       | Collection([DriveRecipient](../resources/driverecipient.md)) | アクセスおよび共有の招待状を受信する、受信者のコレクション。                                            |
| message          | String                                          | 共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。 |
| requireSignIn    | Boolean                                         | 共有アイテムを表示するために、招待状の受信者がサインインする必要のある場所を指定します。            |
| sendInvitation   | ブール値                                         | 電子メールまたは投稿が生成されるのか (false)、アクセス許可のみが作成されるのか (true) を指定します。            |
| roles            | Collection(String)                              | 共有の招待状の受信者に付与されるロールを指定します。                         |
| expirationDateTime | DateTimeOffset                       | アクセス許可の有効期限が切れる日時を指定します。 OneDrive for business、SharePoint、プレミアム個人用 OneDrive のアカウントで利用できます。
| パスワード           | String                         | 作成者による招待に設定されたパスワード。 省略可能および OneDrive 個人用のみ

## <a name="example"></a>例

この例では、"ryan@contoso.org" というメール アドレスを持つユーザーに共有の招待状を、共同作業中のファイルについてのメッセージと共に送信します。
この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。

### <a name="http-request"></a>HTTP 要求

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

以下は、応答の例です。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="partial-success-response"></a>正常な応答の一部

複数の受信者への招待では、一部の受信者に対して通知が成功する可能性があります。
この場合、サービスは、HTTP 状態コードが207である部分的な成功応答を返します。
部分的な成功が返された場合は、失敗した各`error`受信者の応答に、発生した問題とその修正方法に関する情報を持つオブジェクトが含まれます。

部分的な応答の例を次に示します。  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a>SendNotification エラー
通知の送信が失敗した場合に、入れ子になっ`innererror`たオブジェクト内でアプリに発生する可能性があるその他のエラーを次に示します。 アプリでは、これらを処理する必要はありません。

| コード                           | 説明
|:-------------------------------|:--------------------------------------------------------------------------------------
| accountVerificationRequired    | 通知の送信のブロックを解除するには、アカウントの確認が必要です。
| hipCheckRequired               | HIP を解決する必要があります。 [通知の送信をブロック解除する] チェックボックスをオンにします。
| exchangeInvalidUser            | 現在のユーザーのメールボックスが見つかりませんでした。
| exchangeOutOfMailboxQuota      | クォータが不足しています。
| exchangeMaxRecipients          | 一度に通知を送信できる受信者の最大数を超過しました。

>**注:** このサービスは、新しいエラーコードを追加するか、または、いつでも古いものを返すことを停止できます。

## <a name="remarks"></a>備考

* `personal` (OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。
* 使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration-values)」を参照してください。

## <a name="error-responses"></a>エラー応答

エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
}
-->
