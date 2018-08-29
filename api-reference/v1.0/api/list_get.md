---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストを取得する
ms.openlocfilehash: 042e9d6352d99f3a9e8d57daed685b6d9b2f7f65
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264015"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="5ca4f-102">リストのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="5ca4f-102">Get metadata for a list</span></span>

<span data-ttu-id="5ca4f-103">[list][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="5ca4f-103">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="5ca4f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ca4f-105">Permissions</span></span>

<span data-ttu-id="5ca4f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ca4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ca4f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ca4f-108">Permission type</span></span>      | <span data-ttu-id="5ca4f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ca4f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ca4f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ca4f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ca4f-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca4f-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ca4f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ca4f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ca4f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ca4f-113">Not supported.</span></span>    |
|<span data-ttu-id="5ca4f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ca4f-114">Application</span></span> | <span data-ttu-id="5ca4f-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca4f-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ca4f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ca4f-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="5ca4f-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ca4f-117">Request body</span></span>

<span data-ttu-id="5ca4f-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5ca4f-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="5ca4f-119">例</span><span class="sxs-lookup"><span data-stu-id="5ca4f-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5ca4f-120">要求</span><span class="sxs-lookup"><span data-stu-id="5ca4f-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="5ca4f-121">応答</span><span class="sxs-lookup"><span data-stu-id="5ca4f-121">Response</span></span>

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

<span data-ttu-id="5ca4f-122">`select` ステートメントと `expand` ステートメントを使用すれば、リストのメタデータ、列定義、リスト アイテムを単一の要求で取得できます。</span><span class="sxs-lookup"><span data-stu-id="5ca4f-122">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="5ca4f-123">要求</span><span class="sxs-lookup"><span data-stu-id="5ca4f-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="5ca4f-124">応答</span><span class="sxs-lookup"><span data-stu-id="5ca4f-124">Response</span></span>

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
  "tocPath": "Lists/Get metadata"
} -->
