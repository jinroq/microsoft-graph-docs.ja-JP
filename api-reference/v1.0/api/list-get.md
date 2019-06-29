---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 4f623aa940ad71a593d68df1d86e4d18360277b9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272059"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="d0f44-102">リストのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="d0f44-102">Get metadata for a list</span></span>

<span data-ttu-id="d0f44-103">[list][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="d0f44-103">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="d0f44-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d0f44-105">Permissions</span></span>

<span data-ttu-id="d0f44-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0f44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0f44-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0f44-108">Permission type</span></span>      | <span data-ttu-id="d0f44-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0f44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0f44-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0f44-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0f44-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f44-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0f44-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0f44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0f44-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0f44-113">Not supported.</span></span>    |
|<span data-ttu-id="d0f44-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0f44-114">Application</span></span> | <span data-ttu-id="d0f44-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f44-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0f44-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0f44-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="d0f44-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0f44-117">Request body</span></span>

<span data-ttu-id="d0f44-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d0f44-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="d0f44-119">例</span><span class="sxs-lookup"><span data-stu-id="d0f44-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d0f44-120">要求</span><span class="sxs-lookup"><span data-stu-id="d0f44-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="d0f44-121">応答</span><span class="sxs-lookup"><span data-stu-id="d0f44-121">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1234-112-112-4",
  "name": "MicroFeed",
  "createdDateTime": "2016-08-30T08:32:00Z",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "list": {
    "hidden": false,
    "template": "genericList"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d0f44-122">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d0f44-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d0f44-123">C#</span><span class="sxs-lookup"><span data-stu-id="d0f44-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0f44-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0f44-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d0f44-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0f44-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d0f44-126">`select` ステートメントと `expand` ステートメントを使用すれば、リストのメタデータ、列定義、リスト アイテムを単一の要求で取得できます。</span><span class="sxs-lookup"><span data-stu-id="d0f44-126">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="d0f44-127">要求</span><span class="sxs-lookup"><span data-stu-id="d0f44-127">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="d0f44-128">応答</span><span class="sxs-lookup"><span data-stu-id="d0f44-128">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1234-112-112-4",
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Color",
      "description": "Color of the item in stock"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d0f44-129">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d0f44-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d0f44-130">C#</span><span class="sxs-lookup"><span data-stu-id="d0f44-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0f44-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0f44-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d0f44-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0f44-132">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
