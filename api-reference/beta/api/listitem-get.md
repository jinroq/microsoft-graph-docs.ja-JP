---
author: JeremyKelley
description: list 内の item のメタデータを返します。
ms.date: 09/11/2017
title: SharePoint リストからエントリを取得する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b75a9a8542e4bf92f4e4ad36e5431881623808b7
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415394"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="48083-103">リスト内のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="48083-103">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48083-104">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="48083-104">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="48083-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48083-107">Permissions</span></span>

<span data-ttu-id="48083-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48083-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48083-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48083-110">Permission type</span></span>      | <span data-ttu-id="48083-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48083-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48083-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48083-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48083-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48083-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="48083-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48083-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48083-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48083-115">Not supported.</span></span>    |
|<span data-ttu-id="48083-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48083-116">Application</span></span> | <span data-ttu-id="48083-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48083-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48083-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48083-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="48083-119">例</span><span class="sxs-lookup"><span data-stu-id="48083-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="48083-120">要求</span><span class="sxs-lookup"><span data-stu-id="48083-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="48083-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="48083-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48083-122">C#</span><span class="sxs-lookup"><span data-stu-id="48083-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48083-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48083-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48083-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="48083-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="48083-125">応答</span><span class="sxs-lookup"><span data-stu-id="48083-125">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
}
-->
