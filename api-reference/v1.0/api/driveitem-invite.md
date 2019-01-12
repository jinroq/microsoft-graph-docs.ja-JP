---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: アイテムにアクセスするために招待状を送信する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 23e58c063e31f8ad68ac887a4fd1d2cd4dcd5274
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976962"
---
# <a name="send-a-sharing-invitation"></a>共有の招待状を送信する

の**DriveItem**の共有への招待を送信します。
共有への招待は、受信者へのアクセス許可を提供し、オプションで[リンクを共有][]して電子メールを送信します。

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

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

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

| パラメーター        | 型                           | 説明
|:-----------------|:-------------------------------|:-------------------------
| Recipients       | Collection([DriveRecipient][]) | アクセスおよび共有の招待状を受信する、受信者のコレクション。
| message          | String                         | 共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。
| requireSignIn    | Boolean                        | 招待の受信者は、共有アイテムを表示するのにはサインインする必要かどうかを指定します。
| sendInvitation   | Boolean                        | True の場合、[リンクを共有する][]は、受信者に送信されます。 それ以外の場合、通知を送信せずに直接アクセス許可が与えられます。
| roles            | Collection(String)             | 共有への招待の受信者に許可するロールを指定します。

## <a name="example"></a>例

次の使用例は、共同作業中のファイルについてのメッセージには、"ryan@contoso.com"の電子メール アドレスを持つユーザーに共有への招待を送信します。
この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。

### <a name="http-request"></a>HTTP 要求

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。

<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

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
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a>備考

* `personal` (OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。
* 使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration)」を参照してください。

## <a name="error-responses"></a>エラー応答

エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[リンクの共有]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
