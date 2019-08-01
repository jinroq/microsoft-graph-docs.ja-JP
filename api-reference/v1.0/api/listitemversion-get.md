---
title: ListItemVersion リソースを取得する
description: ListItem の特定のバージョンのメタデータを取得します。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 331708b7e544d4b38fff9f5270a28f766790963a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023143"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="35388-103">ListItemVersion リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="35388-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="35388-104">[ListItem](../resources/listitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="35388-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35388-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="35388-105">Permissions</span></span>

<span data-ttu-id="35388-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="35388-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35388-108">Permission type</span></span>             | <span data-ttu-id="35388-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="35388-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="35388-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35388-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="35388-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35388-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="35388-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35388-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35388-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="35388-113">n/a</span></span>                                         |
| <span data-ttu-id="35388-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35388-114">Application</span></span>                            | <span data-ttu-id="35388-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35388-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="35388-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35388-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="35388-117">応答</span><span class="sxs-lookup"><span data-stu-id="35388-117">Response</span></span>

<span data-ttu-id="35388-118">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ListItemVersion](../resources/listitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="35388-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="35388-119">例</span><span class="sxs-lookup"><span data-stu-id="35388-119">Example</span></span>

<span data-ttu-id="35388-120">この例では、listItem の 1 つのバージョンを取得し、fields コレクションを展開して listItem 内のフィールドの値を要求します。</span><span class="sxs-lookup"><span data-stu-id="35388-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="35388-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35388-121">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="35388-122">プロトコル</span><span class="sxs-lookup"><span data-stu-id="35388-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35388-123">C#</span><span class="sxs-lookup"><span data-stu-id="35388-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35388-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="35388-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35388-125">目的-C</span><span class="sxs-lookup"><span data-stu-id="35388-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="35388-126">Java</span><span class="sxs-lookup"><span data-stu-id="35388-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35388-127">応答</span><span class="sxs-lookup"><span data-stu-id="35388-127">Response</span></span>

<span data-ttu-id="35388-128">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="35388-128">This returns a collection of versions:</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
