---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからエントリを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: c46fed1c2da3ac246212dbbcdfeb35479699efe6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613072"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="247d9-102">リスト内のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="247d9-102">Get an item in a list</span></span>

<span data-ttu-id="247d9-103">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="247d9-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="247d9-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="247d9-106">Permissions</span></span>

<span data-ttu-id="247d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="247d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="247d9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="247d9-109">Permission type</span></span>      | <span data-ttu-id="247d9-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="247d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="247d9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="247d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="247d9-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="247d9-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="247d9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="247d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="247d9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="247d9-114">Not supported.</span></span>    |
|<span data-ttu-id="247d9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="247d9-115">Application</span></span> | <span data-ttu-id="247d9-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="247d9-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="247d9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="247d9-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="247d9-118">例</span><span class="sxs-lookup"><span data-stu-id="247d9-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="247d9-119">要求</span><span class="sxs-lookup"><span data-stu-id="247d9-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="247d9-120">応答</span><span class="sxs-lookup"><span data-stu-id="247d9-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="247d9-121">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="247d9-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="247d9-122">C#</span><span class="sxs-lookup"><span data-stu-id="247d9-122">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="247d9-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="247d9-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
