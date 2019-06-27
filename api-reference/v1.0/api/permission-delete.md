---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: アイテムへのアクセスを削除する
localization_priority: Normal
ms.openlocfilehash: ebbc3388e1e207b83ec3cd7ea45635a49f5f7a01
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275545"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a>ファイルまたはフォルダーの共有アクセス許可を削除する

[DriveItem](../resources/driveitem.md) へのアクセスを削除します。

継承されて**いない**共有アクセス許可のみを削除することができます。
**InheritedFrom** プロパティは `null` である必要があります。

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
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前          | 型   | 説明                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | string | この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

この例では、現在のユーザーの OneDrive 内の項目 {item-id} から {perm-id} として識別されるアクセス許可を削除します。

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a>応答

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-permission-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-permission-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete-permission-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a>注釈

* `personal` (OneDrive Personal) の **driveType** を持つ[ドライブ](../resources/drive.md)は、DriveItem のルートでの作成やアクセス許可の変更を行えません。 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions",
  "suppressions": [
    "Error: /api-reference/v1.0/api/permission-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/permission-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/permission-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
