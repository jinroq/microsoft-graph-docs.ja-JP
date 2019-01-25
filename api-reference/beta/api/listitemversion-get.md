---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 旧バージョンのリスト アイテムを取得する - SharePoint API
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a23a8218b2be3ff36d719ee25e6fb0c960c5750f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526257"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="1e417-102">ListItemVersion リソースを取得する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="1e417-102">Get a ListItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e417-103">[ListItem](../resources/listitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="1e417-103">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e417-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e417-104">Permissions</span></span>

<span data-ttu-id="1e417-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="1e417-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e417-107">Permission type</span></span>             | <span data-ttu-id="1e417-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e417-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1e417-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e417-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e417-110">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e417-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="1e417-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e417-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e417-112">該当なし</span><span class="sxs-lookup"><span data-stu-id="1e417-112">n/a</span></span>                                         |
| <span data-ttu-id="1e417-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e417-113">Application</span></span>                            | <span data-ttu-id="1e417-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e417-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="1e417-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e417-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="1e417-116">応答</span><span class="sxs-lookup"><span data-stu-id="1e417-116">Response</span></span>

<span data-ttu-id="1e417-117">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ListItemVersion](../resources/listitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1e417-117">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="1e417-118">例</span><span class="sxs-lookup"><span data-stu-id="1e417-118">Example</span></span>

<span data-ttu-id="1e417-119">この例では、listItem の 1 つのバージョンを取得し、fields コレクションを展開して listItem 内のフィールドの値を要求します。</span><span class="sxs-lookup"><span data-stu-id="1e417-119">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="1e417-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e417-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="1e417-121">応答</span><span class="sxs-lookup"><span data-stu-id="1e417-121">Response</span></span>

<span data-ttu-id="1e417-122">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1e417-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/listitemversion-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
