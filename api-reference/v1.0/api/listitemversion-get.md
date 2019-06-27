---
title: ListItemVersion リソースを取得する
description: ListItem の特定のバージョンのメタデータを取得します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 36164373d0df1ddfd69df4d9e5800d52b2363108
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271961"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="2c234-103">ListItemVersion リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="2c234-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="2c234-104">[ListItem](../resources/listitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="2c234-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c234-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2c234-105">Permissions</span></span>

<span data-ttu-id="2c234-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="2c234-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2c234-108">Permission type</span></span>             | <span data-ttu-id="2c234-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2c234-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2c234-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2c234-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c234-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c234-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="2c234-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2c234-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c234-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="2c234-113">n/a</span></span>                                         |
| <span data-ttu-id="2c234-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2c234-114">Application</span></span>                            | <span data-ttu-id="2c234-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c234-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="2c234-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2c234-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="2c234-117">応答</span><span class="sxs-lookup"><span data-stu-id="2c234-117">Response</span></span>

<span data-ttu-id="2c234-118">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ListItemVersion](../resources/listitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2c234-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="2c234-119">例</span><span class="sxs-lookup"><span data-stu-id="2c234-119">Example</span></span>

<span data-ttu-id="2c234-120">この例では、listItem の 1 つのバージョンを取得し、fields コレクションを展開して listItem 内のフィールドの値を要求します。</span><span class="sxs-lookup"><span data-stu-id="2c234-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c234-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2c234-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="2c234-122">応答</span><span class="sxs-lookup"><span data-stu-id="2c234-122">Response</span></span>

<span data-ttu-id="2c234-123">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2c234-123">This returns a collection of versions:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c234-124">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="2c234-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c234-125">C#</span><span class="sxs-lookup"><span data-stu-id="2c234-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c234-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c234-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c234-127">目的-C</span><span class="sxs-lookup"><span data-stu-id="2c234-127">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
