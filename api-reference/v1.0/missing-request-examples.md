---
title: (me) をシングルトンとして定義します。
description: Markdown を確認するためにドキュメントに追加する必要があるのは、次のような点です。
localization_priority: Normal
ms.openlocfilehash: 62d222b2e6b3145371f3eac564236dc75d222315
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273466"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="332b8-103">ヘルパー (ドキュメントに含まれていない例)</span><span class="sxs-lookup"><span data-stu-id="332b8-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="332b8-104">これらはマークダウン スキャナーがグラフ ドキュメントを適切に処理できるようにするため、ドキュメントに追加する必要があったものです。</span><span class="sxs-lookup"><span data-stu-id="332b8-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="332b8-105">(me) をシングルトンとして定義します。</span><span class="sxs-lookup"><span data-stu-id="332b8-105">Define the /me as singleton</span></span>

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="332b8-106">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="332b8-106">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="332b8-107">C#</span><span class="sxs-lookup"><span data-stu-id="332b8-107">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_current_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="332b8-108">Javascript</span><span class="sxs-lookup"><span data-stu-id="332b8-108">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_current_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="332b8-109">目的-C</span><span class="sxs-lookup"><span data-stu-id="332b8-109">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_current_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="332b8-110">ドライブをクエリ可能な entityset として定義します。</span><span class="sxs-lookup"><span data-stu-id="332b8-110">Define drives as an queryable entityset</span></span>
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="332b8-111">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="332b8-111">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="332b8-112">C#</span><span class="sxs-lookup"><span data-stu-id="332b8-112">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_drive_from_id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="332b8-113">Javascript</span><span class="sxs-lookup"><span data-stu-id="332b8-113">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_drive_from_id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="332b8-114">目的-C</span><span class="sxs-lookup"><span data-stu-id="332b8-114">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_drive_from_id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="332b8-115">ユーザーをクエリ可能な entityset として定義します。</span><span class="sxs-lookup"><span data-stu-id="332b8-115">define users as an queryable entityset</span></span>

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="332b8-116">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="332b8-116">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="332b8-117">C#</span><span class="sxs-lookup"><span data-stu-id="332b8-117">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="332b8-118">Javascript</span><span class="sxs-lookup"><span data-stu-id="332b8-118">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="332b8-119">目的-C</span><span class="sxs-lookup"><span data-stu-id="332b8-119">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_users-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d73
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Missing Requests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /missing-request-examples.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /missing-request-examples.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /missing-request-examples.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
