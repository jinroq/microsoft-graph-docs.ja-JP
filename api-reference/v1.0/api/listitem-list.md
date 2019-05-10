---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからアイテムを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 6038b5d82ed91b94a9388689ba39c890f1dc4f6c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613565"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="641ca-102">リスト内のアイテムを列挙する</span><span class="sxs-lookup"><span data-stu-id="641ca-102">Enumerate items in a list</span></span>

<span data-ttu-id="641ca-103">[リスト][]内の[アイテム][item]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="641ca-103">Get the collection of [items][item] in a [list][].</span></span>

[リスト]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="641ca-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="641ca-105">Permissions</span></span>

<span data-ttu-id="641ca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="641ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="641ca-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="641ca-108">Permission type</span></span>      | <span data-ttu-id="641ca-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="641ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="641ca-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="641ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="641ca-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="641ca-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="641ca-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="641ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="641ca-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="641ca-113">Not supported.</span></span>    |
|<span data-ttu-id="641ca-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="641ca-114">Application</span></span> | <span data-ttu-id="641ca-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="641ca-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="641ca-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="641ca-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="641ca-117">例</span><span class="sxs-lookup"><span data-stu-id="641ca-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="641ca-118">要求</span><span class="sxs-lookup"><span data-stu-id="641ca-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="641ca-119">応答</span><span class="sxs-lookup"><span data-stu-id="641ca-119">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="641ca-120">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="641ca-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="641ca-121">C#</span><span class="sxs-lookup"><span data-stu-id="641ca-121">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="641ca-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="641ca-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-items-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
