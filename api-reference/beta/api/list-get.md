---
author: JeremyKelley
title: リストのメタデータを取得する
description: '[List] [] のメタデータを返します。'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 60764674ab8aeca106434c4c4400b339a7296152
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840776"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="cfc69-103">リストのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="cfc69-103">Get metadata for a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfc69-104">[リスト][]のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="cfc69-104">Return the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="cfc69-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cfc69-106">Permissions</span></span>

<span data-ttu-id="cfc69-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfc69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfc69-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfc69-109">Permission type</span></span>      | <span data-ttu-id="cfc69-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfc69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfc69-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfc69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cfc69-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfc69-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cfc69-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfc69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfc69-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfc69-114">Not supported.</span></span>    |
|<span data-ttu-id="cfc69-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfc69-115">Application</span></span> | <span data-ttu-id="cfc69-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfc69-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfc69-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfc69-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="cfc69-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="cfc69-118">Request body</span></span>

<span data-ttu-id="cfc69-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cfc69-119">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="cfc69-120">例</span><span class="sxs-lookup"><span data-stu-id="cfc69-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cfc69-121">要求</span><span class="sxs-lookup"><span data-stu-id="cfc69-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cfc69-122">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cfc69-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfc69-123">C#</span><span class="sxs-lookup"><span data-stu-id="cfc69-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfc69-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfc69-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfc69-125">目的-C</span><span class="sxs-lookup"><span data-stu-id="cfc69-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cfc69-126">応答</span><span class="sxs-lookup"><span data-stu-id="cfc69-126">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

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

<span data-ttu-id="cfc69-127">`select` ステートメントと `expand` ステートメントを使用すれば、リストのメタデータ、列定義、リスト アイテムを単一の要求で取得できます。</span><span class="sxs-lookup"><span data-stu-id="cfc69-127">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="cfc69-128">要求</span><span class="sxs-lookup"><span data-stu-id="cfc69-128">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cfc69-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cfc69-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfc69-130">C#</span><span class="sxs-lookup"><span data-stu-id="cfc69-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfc69-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfc69-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfc69-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="cfc69-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cfc69-133">応答</span><span class="sxs-lookup"><span data-stu-id="cfc69-133">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
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
#### <a name="request"></a><span data-ttu-id="cfc69-134">要求</span><span class="sxs-lookup"><span data-stu-id="cfc69-134">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="cfc69-135">次の例は、名前、数量、カテゴリの3つの列を含むリストのメタデータを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cfc69-135">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="cfc69-136">[管理](https://docs.microsoft.com/en-us/sharepoint/managed-metadata)された```Category```メタデータ列。用語 ID と用語名のペアとしての戻り値など。</span><span class="sxs-lookup"><span data-stu-id="cfc69-136">[Managed Metadata](https://docs.microsoft.com/en-us/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="cfc69-137">応答</span><span class="sxs-lookup"><span data-stu-id="cfc69-137">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    },
    {
      "name": "Category",
      "description": "Category of the item"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Quantity": 503,
        "Category": {
          "termId": "791d537a-9c1c-3b05-97b0-1ce7ece7e1a4",
          "name": "Tool"
         }
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Quantity": 2357,
        "Category": {
          "termId": "902e568b-9b2d-4d06-87c2-2cf8ecf9f2b5" ,
          "name": "Mechanical Device"
         }
       }
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
  ]
}
-->
