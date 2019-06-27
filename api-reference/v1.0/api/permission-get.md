---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: アクセス許可の取得
localization_priority: Normal
ms.openlocfilehash: a2518745ea89e3d2192dae69ec4195d59ea31399
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275538"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a>ファイルまたはフォルダーの共有アクセス許可を取得する

特定のアクセス許可リソースに対する、有効な共有アクセス許可を返します。

アイテムの有効なアクセス許可は、アイテム自体に直接設定されたアクセス許可、またはアイテムの先祖から継承したアクセス許可の 2 つのソースから取得できます。

呼び出し元は、`inheritedFrom` プロパティを確認することで、アクセス許可が継承されたものかどうかを区別できます。このプロパティは、アクセス許可の継承元になる先祖を参照する [ItemReference](../resources/itemreference.md) リソースです。

アイテムに設定された SharePoint アクセス許可レベルは、'SP' というプレフィックス付きで返されます。 たとえば、SP.View Only、SP.Limited Access、SP.View Web Analytics Data などです。 [SharePoint ロールの完全なリスト](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)を参照してください。

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
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

応答を形成するため、このメソッドは、[$select クエリ パラメーター](/graph/query-parameters) をサポートしています。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Permission](../resources/permission.md) リソースを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、フォルダーのアクセス許可にアクセスするための要求の例です。

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a>応答

成功した場合、このメソッドは、指定された ID の [Permission](../resources/permission.md) リソースを返します。 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-item-permission-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-item-permission-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-item-permission-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a>備考

[アクセス権](../resources/permission.md)リソースは、_ファセット_を使用してリソースによって表されるアクセス許可の種類に関する情報を提供します。

[**リンク**](../resources/sharinglink.md) ファセットのあるアクセス許可は、項目上に作成された共有するリンクを表します。共有リンクは、リンクを持つすべてのユーザーのアイテムへのアクセス許可を提供する固有のトークンを含みます。

[**招待**](../resources/sharinginvitation.md) ファセットを持つアクセス許可は、指定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。

### <a name="error-responses"></a>エラー応答

エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
    "Error: /api-reference/v1.0/api/permission-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/permission-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/permission-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
