---
title: 'bookingBusiness: 発行'
description: この業務の [スケジュール] ページを外部のお客様が利用できるようにします。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f533a9759db0b2e47c57b1ab55282804f4acf235
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258003"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="65979-103">bookingBusiness: 発行</span><span class="sxs-lookup"><span data-stu-id="65979-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65979-104">この業務の [スケジュール] ページを外部のお客様が利用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="65979-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="65979-105">**IsPublished**プロパティを true に、 **publicurl**プロパティを [スケジュール] ページの URL に設定します。</span><span class="sxs-lookup"><span data-stu-id="65979-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="65979-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65979-106">Permissions</span></span>
<span data-ttu-id="65979-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65979-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65979-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65979-109">Permission type</span></span>      | <span data-ttu-id="65979-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65979-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65979-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65979-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="65979-112">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="65979-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="65979-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65979-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65979-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65979-114">Not supported.</span></span>   |
|<span data-ttu-id="65979-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65979-115">Application</span></span> | <span data-ttu-id="65979-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65979-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="65979-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65979-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="65979-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65979-118">Request headers</span></span>
| <span data-ttu-id="65979-119">名前</span><span class="sxs-lookup"><span data-stu-id="65979-119">Name</span></span>       | <span data-ttu-id="65979-120">説明</span><span class="sxs-lookup"><span data-stu-id="65979-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="65979-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65979-121">Authorization</span></span>  | <span data-ttu-id="65979-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="65979-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="65979-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="65979-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="65979-124">応答</span><span class="sxs-lookup"><span data-stu-id="65979-124">Response</span></span>
<span data-ttu-id="65979-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="65979-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65979-127">例</span><span class="sxs-lookup"><span data-stu-id="65979-127">Example</span></span>
<span data-ttu-id="65979-128">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65979-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="65979-129">要求</span><span class="sxs-lookup"><span data-stu-id="65979-129">Request</span></span>
<span data-ttu-id="65979-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65979-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="65979-131">応答</span><span class="sxs-lookup"><span data-stu-id="65979-131">Response</span></span>
<span data-ttu-id="65979-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65979-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="65979-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="65979-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="65979-134">C#</span><span class="sxs-lookup"><span data-stu-id="65979-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65979-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="65979-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="65979-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="65979-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
