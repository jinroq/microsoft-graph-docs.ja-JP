---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからエントリを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 90095dce5b5cfdadfd37696cd9b43a7a5475b6f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880235"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="a2e5f-102">リスト内のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="a2e5f-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2e5f-103">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="a2e5f-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="a2e5f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2e5f-106">Permissions</span></span>

<span data-ttu-id="a2e5f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2e5f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2e5f-109">Permission type</span></span>      | <span data-ttu-id="a2e5f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2e5f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2e5f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2e5f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a2e5f-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e5f-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2e5f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2e5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2e5f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2e5f-114">Not supported.</span></span>    |
|<span data-ttu-id="a2e5f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2e5f-115">Application</span></span> | <span data-ttu-id="a2e5f-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e5f-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2e5f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2e5f-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="a2e5f-118">例</span><span class="sxs-lookup"><span data-stu-id="a2e5f-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a2e5f-119">要求</span><span class="sxs-lookup"><span data-stu-id="a2e5f-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a2e5f-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a2e5f-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2e5f-121">C#</span><span class="sxs-lookup"><span data-stu-id="a2e5f-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2e5f-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2e5f-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2e5f-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="a2e5f-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a2e5f-124">Java</span><span class="sxs-lookup"><span data-stu-id="a2e5f-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2e5f-125">応答</span><span class="sxs-lookup"><span data-stu-id="a2e5f-125">Response</span></span>

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
