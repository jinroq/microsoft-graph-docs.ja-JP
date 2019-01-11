---
title: 'bookingBusiness: 非公開'
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: fc2556b62ab3b9a32ca278704864265c2de4d25e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838788"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="e97f3-104">bookingBusiness: 非公開</span><span class="sxs-lookup"><span data-stu-id="e97f3-104">bookingBusiness: unpublish</span></span>

 > <span data-ttu-id="e97f3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e97f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e97f3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e97f3-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e97f3-107">外部の顧客に、利用できないこのビジネスでのスケジュールのページを加えます。</span><span class="sxs-lookup"><span data-stu-id="e97f3-107">Make the scheduling page of this business not available to external customers.</span></span> 

<span data-ttu-id="e97f3-108">**IsPublished**プロパティを false、および**publicUrl**プロパティを null に設定します。</span><span class="sxs-lookup"><span data-stu-id="e97f3-108">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="e97f3-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e97f3-109">Permissions</span></span>
<span data-ttu-id="e97f3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e97f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e97f3-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e97f3-112">Permission type</span></span>      | <span data-ttu-id="e97f3-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e97f3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e97f3-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e97f3-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="e97f3-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e97f3-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e97f3-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e97f3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e97f3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e97f3-117">Not supported.</span></span>   |
|<span data-ttu-id="e97f3-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e97f3-118">Application</span></span> | <span data-ttu-id="e97f3-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e97f3-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="e97f3-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e97f3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="e97f3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e97f3-121">Request headers</span></span>
| <span data-ttu-id="e97f3-122">名前</span><span class="sxs-lookup"><span data-stu-id="e97f3-122">Name</span></span>       | <span data-ttu-id="e97f3-123">説明</span><span class="sxs-lookup"><span data-stu-id="e97f3-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e97f3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e97f3-124">Authorization</span></span>  | <span data-ttu-id="e97f3-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e97f3-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e97f3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e97f3-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e97f3-127">応答</span><span class="sxs-lookup"><span data-stu-id="e97f3-127">Response</span></span>
<span data-ttu-id="e97f3-p104">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e97f3-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e97f3-130">例</span><span class="sxs-lookup"><span data-stu-id="e97f3-130">Example</span></span>
<span data-ttu-id="e97f3-131">次に、この API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="e97f3-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e97f3-132">要求</span><span class="sxs-lookup"><span data-stu-id="e97f3-132">Request</span></span>
<span data-ttu-id="e97f3-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e97f3-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="e97f3-134">応答</span><span class="sxs-lookup"><span data-stu-id="e97f3-134">Response</span></span>
<span data-ttu-id="e97f3-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e97f3-135">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
