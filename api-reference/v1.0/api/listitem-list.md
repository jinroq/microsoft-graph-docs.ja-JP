---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからアイテムを取得する
localization_priority: Priority
ms.prod: sharepoint
description: リスト内のアイテムのコレクションを取得します。
doc_type: apiPageType
ms.openlocfilehash: 49ca1090411a1a53be3db193821c14df51edef61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023115"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="97f4f-103">リスト内のアイテムを列挙する</span><span class="sxs-lookup"><span data-stu-id="97f4f-103">Enumerate items in a list</span></span>

<span data-ttu-id="97f4f-104">[リスト][]内の[アイテム][item]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="97f4f-104">Get the collection of [items][item] in a [list][].</span></span>

[リスト]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="97f4f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="97f4f-106">Permissions</span></span>

<span data-ttu-id="97f4f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97f4f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="97f4f-109">Permission type</span></span>      | <span data-ttu-id="97f4f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="97f4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97f4f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="97f4f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97f4f-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97f4f-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="97f4f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="97f4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97f4f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97f4f-114">Not supported.</span></span>    |
|<span data-ttu-id="97f4f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="97f4f-115">Application</span></span> | <span data-ttu-id="97f4f-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97f4f-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97f4f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97f4f-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="97f4f-118">例</span><span class="sxs-lookup"><span data-stu-id="97f4f-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="97f4f-119">要求</span><span class="sxs-lookup"><span data-stu-id="97f4f-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="97f4f-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="97f4f-120">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97f4f-121">C#</span><span class="sxs-lookup"><span data-stu-id="97f4f-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97f4f-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="97f4f-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97f4f-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97f4f-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97f4f-124">Java</span><span class="sxs-lookup"><span data-stu-id="97f4f-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97f4f-125">応答</span><span class="sxs-lookup"><span data-stu-id="97f4f-125">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
} -->
