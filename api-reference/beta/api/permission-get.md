---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: アクセス許可の取得
localization_priority: Normal
ms.openlocfilehash: 1af1cdaa434a95ed77da360334c88dd653d8747a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520026"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a>ファイルまたはフォルダーの共有アクセス許可を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
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

## <a name="remarks"></a>備考

[アクセス権](../resources/permission.md)リソースは、_ファセット_を使用してリソースによって表されるアクセス許可の種類に関する情報を提供します。

[**リンク**](../resources/sharinglink.md) ファセットのあるアクセス許可は、項目上に作成された共有するリンクを表します。共有リンクは、リンクを持つすべてのユーザーのアイテムへのアクセス許可を提供する固有のトークンを含みます。

[**招待**](../resources/sharinginvitation.md) ファセットを持つアクセス許可は、指定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission",
  "suppressions": [
    "Error: /api-reference/beta/api/permission-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
