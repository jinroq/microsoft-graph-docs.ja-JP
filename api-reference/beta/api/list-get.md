---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f796d7b02750034be6d2205a4a25f51c2911f5f2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521657"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="f7926-102">リストのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="f7926-102">Get metadata for a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7926-103">[list][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="f7926-103">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="f7926-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7926-105">Permissions</span></span>

<span data-ttu-id="f7926-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7926-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f7926-108">Permission type</span></span>      | <span data-ttu-id="f7926-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f7926-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7926-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f7926-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7926-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7926-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7926-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f7926-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7926-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7926-113">Not supported.</span></span>    |
|<span data-ttu-id="f7926-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f7926-114">Application</span></span> | <span data-ttu-id="f7926-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7926-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7926-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f7926-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="f7926-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="f7926-117">Request body</span></span>

<span data-ttu-id="f7926-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f7926-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="f7926-119">例</span><span class="sxs-lookup"><span data-stu-id="f7926-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f7926-120">要求</span><span class="sxs-lookup"><span data-stu-id="f7926-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="f7926-121">応答</span><span class="sxs-lookup"><span data-stu-id="f7926-121">Response</span></span>

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

<span data-ttu-id="f7926-122">`select` ステートメントと `expand` ステートメントを使用すれば、リストのメタデータ、列定義、リスト アイテムを単一の要求で取得できます。</span><span class="sxs-lookup"><span data-stu-id="f7926-122">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="f7926-123">要求</span><span class="sxs-lookup"><span data-stu-id="f7926-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="f7926-124">応答</span><span class="sxs-lookup"><span data-stu-id="f7926-124">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
    "Error: /api-reference/beta/api/list-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
