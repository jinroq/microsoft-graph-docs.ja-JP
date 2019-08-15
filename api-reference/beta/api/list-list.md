---
author: JeremyKelley
description: サイトのリストのコレクションを取得します。
ms.date: 09/11/2017
title: サイト内の SharePoint リストを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 89b56b45d2522923d6cdfcd977a327c6abf359ee
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415436"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="83323-103">サイト内のリストを列挙する</span><span class="sxs-lookup"><span data-stu-id="83323-103">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83323-104">[サイト][]の[リスト][]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="83323-104">Get the collection of [lists][] for a [site][].</span></span>

[サイト]: ../resources/list.md
[lists]: ../resources/list.md
[リスト]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="83323-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83323-107">Permissions</span></span>

<span data-ttu-id="83323-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83323-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83323-110">Permission type</span></span>      | <span data-ttu-id="83323-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83323-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83323-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83323-112">Delegated (work or school account)</span></span> | <span data-ttu-id="83323-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83323-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="83323-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83323-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83323-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83323-115">Not supported.</span></span>    |
|<span data-ttu-id="83323-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83323-116">Application</span></span> | <span data-ttu-id="83323-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83323-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83323-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83323-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="83323-119">例</span><span class="sxs-lookup"><span data-stu-id="83323-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="83323-120">要求</span><span class="sxs-lookup"><span data-stu-id="83323-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="83323-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="83323-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83323-122">C#</span><span class="sxs-lookup"><span data-stu-id="83323-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83323-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83323-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83323-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="83323-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="83323-125">応答</span><span class="sxs-lookup"><span data-stu-id="83323-125">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="83323-126">注釈</span><span class="sxs-lookup"><span data-stu-id="83323-126">Remarks</span></span>

<span data-ttu-id="83323-127">[system][] ファセットのあるリストは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="83323-127">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="83323-128">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="83323-128">To list them, include `system` in your `$select` statement.</span></span>

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
