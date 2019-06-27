---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リスト内のレコードを更新する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f365331b5941da48178194c9b02f61aaf1893ed6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264527"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="b6540-102">リスト内のアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="b6540-102">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6540-103">**[listItem][]** のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b6540-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6540-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6540-104">Permissions</span></span>

<span data-ttu-id="b6540-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6540-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6540-107">Permission type</span></span>      | <span data-ttu-id="b6540-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6540-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6540-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6540-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b6540-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6540-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b6540-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6540-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6540-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6540-112">Not supported.</span></span>    |
|<span data-ttu-id="b6540-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6540-113">Application</span></span> | <span data-ttu-id="b6540-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6540-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6540-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6540-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="b6540-116">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6540-116">Optional request headers</span></span>

| <span data-ttu-id="b6540-117">名前</span><span class="sxs-lookup"><span data-stu-id="b6540-117">Name</span></span>       | <span data-ttu-id="b6540-118">値</span><span class="sxs-lookup"><span data-stu-id="b6540-118">Value</span></span> | <span data-ttu-id="b6540-119">説明</span><span class="sxs-lookup"><span data-stu-id="b6540-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="b6540-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="b6540-120">_if-match_</span></span> | <span data-ttu-id="b6540-121">etag</span><span class="sxs-lookup"><span data-stu-id="b6540-121">etag</span></span>  | <span data-ttu-id="b6540-122">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは更新されません。</span><span class="sxs-lookup"><span data-stu-id="b6540-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="b6540-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6540-123">Request body</span></span>

<span data-ttu-id="b6540-124">要求本文に、更新するフィールドを指定する [fieldValueSet][] の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6540-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="b6540-125">例</span><span class="sxs-lookup"><span data-stu-id="b6540-125">Example</span></span>

<span data-ttu-id="b6540-126">ここでは、リスト アイテムの Color フィールドと Quantity フィールドを新しい値で更新する例を示します。</span><span class="sxs-lookup"><span data-stu-id="b6540-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="b6540-127">listItem の他の値はすべてそのままです。</span><span class="sxs-lookup"><span data-stu-id="b6540-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="b6540-128">応答</span><span class="sxs-lookup"><span data-stu-id="b6540-128">Response</span></span>

<span data-ttu-id="b6540-129">成功した場合、このメソッドは更新されたリスト アイテムの応答本文で [fieldValueSet][] を返します。</span><span class="sxs-lookup"><span data-stu-id="b6540-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b6540-130">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="b6540-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b6540-131">C#</span><span class="sxs-lookup"><span data-stu-id="b6540-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6540-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="b6540-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b6540-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="b6540-133">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
