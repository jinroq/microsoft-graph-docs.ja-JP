---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: サイト内の SharePoint リストを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bab9766071aff67758bc7bef35799fa02a7e6eb4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449240"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="7d1b2-102">サイト内のリストを列挙する</span><span class="sxs-lookup"><span data-stu-id="7d1b2-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d1b2-103">[サイト][]の[リスト][]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7d1b2-103">Get the collection of [lists][] for a [site][].</span></span>

[サイト]: ../resources/list.md
[lists]: ../resources/list.md
[リスト]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="7d1b2-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d1b2-106">Permissions</span></span>

<span data-ttu-id="7d1b2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d1b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d1b2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d1b2-109">Permission type</span></span>      | <span data-ttu-id="7d1b2-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d1b2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d1b2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d1b2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d1b2-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d1b2-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7d1b2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d1b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d1b2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d1b2-114">Not supported.</span></span>    |
|<span data-ttu-id="7d1b2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d1b2-115">Application</span></span> | <span data-ttu-id="7d1b2-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d1b2-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d1b2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d1b2-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="7d1b2-118">例</span><span class="sxs-lookup"><span data-stu-id="7d1b2-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7d1b2-119">要求</span><span class="sxs-lookup"><span data-stu-id="7d1b2-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7d1b2-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7d1b2-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7d1b2-121">C#</span><span class="sxs-lookup"><span data-stu-id="7d1b2-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d1b2-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d1b2-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7d1b2-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="7d1b2-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7d1b2-124">応答</span><span class="sxs-lookup"><span data-stu-id="7d1b2-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
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
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="7d1b2-125">注釈</span><span class="sxs-lookup"><span data-stu-id="7d1b2-125">Remarks</span></span>

<span data-ttu-id="7d1b2-126">[system][] ファセットのあるリストは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="7d1b2-126">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="7d1b2-127">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="7d1b2-127">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
  ]
}
-->
