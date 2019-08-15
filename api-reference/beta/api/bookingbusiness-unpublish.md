---
title: 'bookingBusiness: 未発行'
description: 外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: a1e6218ae78e867b83decb34319ed25b9049930f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419462"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="79fca-103">bookingBusiness: 未発行</span><span class="sxs-lookup"><span data-stu-id="79fca-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79fca-104">外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。</span><span class="sxs-lookup"><span data-stu-id="79fca-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="79fca-105">**IsPublished**プロパティを false に設定し、 **publicurl**プロパティを null に設定します。</span><span class="sxs-lookup"><span data-stu-id="79fca-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="79fca-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79fca-106">Permissions</span></span>
<span data-ttu-id="79fca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79fca-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79fca-109">Permission type</span></span>      | <span data-ttu-id="79fca-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79fca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79fca-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79fca-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="79fca-112">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="79fca-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="79fca-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79fca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79fca-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79fca-114">Not supported.</span></span>   |
|<span data-ttu-id="79fca-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79fca-115">Application</span></span> | <span data-ttu-id="79fca-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79fca-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="79fca-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79fca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="79fca-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79fca-118">Request headers</span></span>
| <span data-ttu-id="79fca-119">名前</span><span class="sxs-lookup"><span data-stu-id="79fca-119">Name</span></span>       | <span data-ttu-id="79fca-120">説明</span><span class="sxs-lookup"><span data-stu-id="79fca-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79fca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="79fca-121">Authorization</span></span>  | <span data-ttu-id="79fca-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="79fca-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="79fca-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="79fca-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="79fca-124">応答</span><span class="sxs-lookup"><span data-stu-id="79fca-124">Response</span></span>
<span data-ttu-id="79fca-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="79fca-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79fca-127">例</span><span class="sxs-lookup"><span data-stu-id="79fca-127">Example</span></span>
<span data-ttu-id="79fca-128">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79fca-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79fca-129">要求</span><span class="sxs-lookup"><span data-stu-id="79fca-129">Request</span></span>
<span data-ttu-id="79fca-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79fca-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79fca-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="79fca-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79fca-132">C#</span><span class="sxs-lookup"><span data-stu-id="79fca-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79fca-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79fca-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79fca-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="79fca-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79fca-135">応答</span><span class="sxs-lookup"><span data-stu-id="79fca-135">Response</span></span>
<span data-ttu-id="79fca-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="79fca-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
