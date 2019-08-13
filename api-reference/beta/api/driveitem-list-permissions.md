---
author: JeremyKelley
description: DriveItem の有効な共有アクセス許可を一覧表示します。
ms.date: 09/10/2017
title: ファイルへのアクセス権を持つユーザーを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4a209d81f10541e54e56899973c7b7ff9eb5d3d3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324371"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a>DriveItem の共有アクセス許可を一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[DriveItem](../resources/driveitem.md) の有効な共有アクセス許可を一覧表示します。

## <a name="access-to-sharing-permissions"></a>共有アクセス許可へのアクセス

アクセス許可のコレクションには、機密情報が含まれている可能性があり、呼び出し元によっては使用できないこともあります。

* アイテムのオーナーの場合は、すべての共有アクセス許可が返されます。 これには、共同所有者が含まれます。
* 所有者以外の呼び出し元の場合、その呼び出し元に適用される共有アクセス許可のみが返されます。
* 秘密 (`shareId` や `webUrl` など) を含む共有アクセス許可のプロパティは、その共有アクセス許可を作成できる呼び出し元にのみ返されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|アプリケーション | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前          | 型   | 説明                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | string | この要求ヘッダーが含まれている場合、指定された etag がアイテムの現在の etag に一致すると、`HTTP 304 Not Modified` 応答が返されます。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Permission](../resources/permission.md) リソースのコレクションを返します。

DriveItem の有効な共有アクセス許可は、次の 2 つのソースが元になります。

* DriveItem 自体に直接適用される共有アクセス許可
* DriveItem の先祖から継承された共有アクセス許可

呼び出し元は、**inheritedFrom** プロパティを確認して、アクセス許可が継承されているかどうかによって区別できます。このプロパティは、アクセス許可が継承された先祖を参照する [**itemReference**](../resources/itemreference.md) リソースです。

アイテムに設定された SharePoint アクセス許可レベルは、'SP' というプレフィックス付きで返されます。 たとえば、SP.View Only、SP.Limited Access、SP.View Web Analytics Data などです。 [SharePoint ロールの完全なリスト](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)を参照してください。

## <a name="example"></a>例

この例では、サインイン ユーザーのドライブ内のアイテムに対するアクセス許可のコレクションを取得します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/permissions
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

この応答例には、3 つのアクセス許可が含まれています。1 つ目は編集権限を伴う共有リンク、2 つ目は親フォルダーから継承された、John という名前のユーザーへの明示的なアクセス許可、3 つ目はアプリケーションによって作成された読み取り/書き込み共有リンクです。

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>備考

DriveItem の **permissions** リレーションシップは、[DriveItem の取得](driveitem-get.md)または DriveItem のコレクションの取得の一環として展開することはできません。permissions プロパティに直接アクセスする必要があります。

## <a name="error-responses"></a>エラー応答

エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
}
-->
