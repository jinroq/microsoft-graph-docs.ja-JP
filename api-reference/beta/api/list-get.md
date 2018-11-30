---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストを取得する
ms.openlocfilehash: 8cda18e17197a6f14a3c60903fa0c4ad43ed684d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070740"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="745e9-102">リストのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="745e9-102">Get metadata for a list</span></span>

> <span data-ttu-id="745e9-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="745e9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="745e9-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="745e9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="745e9-105">[list][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="745e9-105">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="745e9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="745e9-107">Permissions</span></span>

<span data-ttu-id="745e9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="745e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="745e9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="745e9-110">Permission type</span></span>      | <span data-ttu-id="745e9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="745e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="745e9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="745e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="745e9-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="745e9-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="745e9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="745e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="745e9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="745e9-115">Not supported.</span></span>    |
|<span data-ttu-id="745e9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="745e9-116">Application</span></span> | <span data-ttu-id="745e9-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="745e9-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="745e9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="745e9-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="745e9-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="745e9-119">Request body</span></span>

<span data-ttu-id="745e9-120">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="745e9-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="745e9-121">例</span><span class="sxs-lookup"><span data-stu-id="745e9-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="745e9-122">要求</span><span class="sxs-lookup"><span data-stu-id="745e9-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="745e9-123">応答</span><span class="sxs-lookup"><span data-stu-id="745e9-123">Response</span></span>

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

<span data-ttu-id="745e9-124">`select` ステートメントと `expand` ステートメントを使用すれば、リストのメタデータ、列定義、リスト アイテムを単一の要求で取得できます。</span><span class="sxs-lookup"><span data-stu-id="745e9-124">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="745e9-125">要求</span><span class="sxs-lookup"><span data-stu-id="745e9-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="745e9-126">応答</span><span class="sxs-lookup"><span data-stu-id="745e9-126">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata"
} -->
