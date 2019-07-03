---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからアイテムを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 640702bc65ef36f50a0b548e0e10720a71a2c807
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449149"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="29bfa-102">リスト内のアイテムを列挙する</span><span class="sxs-lookup"><span data-stu-id="29bfa-102">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29bfa-103">[リスト][]内の[アイテム][item]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="29bfa-103">Get the collection of [items][item] in a [list][].</span></span>

[リスト]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="29bfa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29bfa-105">Permissions</span></span>

<span data-ttu-id="29bfa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29bfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29bfa-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29bfa-108">Permission type</span></span>      | <span data-ttu-id="29bfa-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29bfa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29bfa-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29bfa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29bfa-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29bfa-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="29bfa-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29bfa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29bfa-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29bfa-113">Not supported.</span></span>    |
|<span data-ttu-id="29bfa-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29bfa-114">Application</span></span> | <span data-ttu-id="29bfa-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29bfa-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29bfa-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29bfa-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="29bfa-117">例</span><span class="sxs-lookup"><span data-stu-id="29bfa-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="29bfa-118">要求</span><span class="sxs-lookup"><span data-stu-id="29bfa-118">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="29bfa-119">プロトコル</span><span class="sxs-lookup"><span data-stu-id="29bfa-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29bfa-120">C#</span><span class="sxs-lookup"><span data-stu-id="29bfa-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29bfa-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="29bfa-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29bfa-122">目的-C</span><span class="sxs-lookup"><span data-stu-id="29bfa-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29bfa-123">応答</span><span class="sxs-lookup"><span data-stu-id="29bfa-123">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
}
-->
