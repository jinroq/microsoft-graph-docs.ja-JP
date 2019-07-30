---
author: kevklam
ms.author: kevinlam
title: アクセス許可の付与
description: 指定したリンクを使用するためのアクセス許可の一覧をユーザーに付与する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 710ec2ada243d4753573ef1a069a2dff69ee9690
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932875"
---
# <a name="grant-permission"></a>アクセス許可の付与

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[アクセス許可][]で表されるリンクへのアクセスをユーザーに許可します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                   | アクセス許可 (特権の小さいものから大きいものへ)              |
|:----------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明  |
|:------------- |:------------ |
| Authorization | ベアラー \{トークン\}。 必須です。 |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| パラメーター          | 型                           | 説明
|:-------------------|:-------------------------------|:-------------------------
| recipients         | コレクション ([driveRecipient][]) | アクセスを受信する受信者のコレクション。
| roles              | Collection(String)             | リンクが "既存のアクセス" リンクの場合は、ユーザーに付与する役割を指定します。 それ以外の場合は、リンクのロールと一致する必要があります。

使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration-values)」を参照してください。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[permission][]コレクションを返します。

更新されたリンクを表す[アクセス許可][]は、成功時に結果セットで常に返されます。 更新されたリンクは、' scope ' プロパティを含む ' link ' ファセットが存在することで識別できます。 場合によっては、更新されたリンクの URL が元のリンクと異なる場合があります。その場合は、新しい URL を使用する必要があります。

エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。


## <a name="example"></a>例

この例では、リンク上の他の既存のアクセス許可を変更せずに、共有リンクへの john@contoso.com および ryan@external.com アクセスをユーザーに許可します。

### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST https://graph.microsoft.com/beta/shares/{encoded-sharing-url}/permission/grant
Content-type: application/json

{
  "recipients": [
    {
      "email": "john@contoso.com"
    },
    {
      "email": "ryan@external.com"
    }
  ],
  "roles": ["read"]
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

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "5fab944a-47ec-48d0-a9b5-5178a926d00f",
      "link": {
        "preventsDownload": false,
        "scope": "users",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/design/EZexPoDjW4dMtKFUfAl6BK4BvIUuss52hLYzihBfx-PD6Q"
      },
      "roles": [
        "read"
      ]
    }
  ]
}
```

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

リンクが[既存の access](../resources/permission.md#existing-access-link)リンクの場合は、次のものを表す追加のアクセス許可が返されます。

- アクセスが正常に付与された受信者を表す、ユーザーの種類のアクセス許可。 これらは、 **grantedTo**プロパティのプレゼンスによって識別できます。
- アクセス権を取得するために、認識されない外部ユーザーに送信する必要がある招待を表すリンクの種類のアクセス許可。 これらは、[招待](../resources/sharinginvitation.md)ファセットが存在することによって識別できます。 これらのエントリには、招待 URL の[リンク][sharing-link]が含まれており、grantedToIdentities コレクションは、そのリンクを送信するユーザーを示します。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "00000000-0000-0000-0000-000000000000",
      "link": {
        "preventsDownload": false,
        "scope": "existingAccess",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/teams/design/shareddocs/Document.docx"
      },
      "roles": [
        "read"
      ]
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "John Smith",
          "email": "john@contoso.com",
          "id": "47aecee2-d061-4730-8ecb-4c61360441ae"
        }
      },
      "id": "aTowIy5mfG1lbWJlcnNoaXB8bGltaXRlZDJAa2xhbW9kYi5vbm1pY3Jvc29mdC5jb20",
      "roles": [
        "read"
      ]
    },
    {
      "grantedToIdentities": [
        {
          "user": {
            "email": "ryan@external.com"
          }
        }
      ],
      "invitation": {
        "signInRequired": true
      },
      "roles": [
        "read"
      ],
      "link": {
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/teams/design/EZexPoDjW4dMtKFUfAl6BK4Bw_F7gFH63O310A7lDtK0mQ"
      }
    }
  ]
}

```

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[permission]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
