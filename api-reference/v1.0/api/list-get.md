---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストを取得する
localization_priority: Priority
ms.prod: sharepoint
description: list のメタデータを返します。
doc_type: apiPageType
ms.openlocfilehash: 93c007a761b431131236b9c3ba66f36f071ab250
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023175"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="e7980-103">リストのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="e7980-103">Get metadata for a list</span></span>

<span data-ttu-id="e7980-104">[list][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="e7980-104">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="e7980-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7980-106">Permissions</span></span>

<span data-ttu-id="e7980-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7980-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7980-109">Permission type</span></span>      | <span data-ttu-id="e7980-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7980-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7980-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7980-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7980-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7980-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7980-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7980-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7980-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7980-114">Not supported.</span></span>    |
|<span data-ttu-id="e7980-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7980-115">Application</span></span> | <span data-ttu-id="e7980-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7980-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7980-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7980-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="e7980-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7980-118">Request body</span></span>

<span data-ttu-id="e7980-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7980-119">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="e7980-120">例</span><span class="sxs-lookup"><span data-stu-id="e7980-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e7980-121">要求</span><span class="sxs-lookup"><span data-stu-id="e7980-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7980-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7980-122">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7980-123">C#</span><span class="sxs-lookup"><span data-stu-id="e7980-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7980-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7980-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7980-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7980-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7980-126">Java</span><span class="sxs-lookup"><span data-stu-id="e7980-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7980-127">応答</span><span class="sxs-lookup"><span data-stu-id="e7980-127">Response</span></span>

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

<span data-ttu-id="e7980-128">`select` ステートメントと `expand` ステートメントを使用すれば、リストのメタデータ、列定義、リスト アイテムを単一の要求で取得できます。</span><span class="sxs-lookup"><span data-stu-id="e7980-128">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="e7980-129">要求</span><span class="sxs-lookup"><span data-stu-id="e7980-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7980-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7980-130">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7980-131">C#</span><span class="sxs-lookup"><span data-stu-id="e7980-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7980-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7980-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7980-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7980-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7980-134">Java</span><span class="sxs-lookup"><span data-stu-id="e7980-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7980-135">応答</span><span class="sxs-lookup"><span data-stu-id="e7980-135">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
  ]
} -->
