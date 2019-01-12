---
title: 'bookingBusiness: 発行'
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 33e11fac5690e66664038705b482480ef689db6e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917322"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="91d7f-104">bookingBusiness: 発行</span><span class="sxs-lookup"><span data-stu-id="91d7f-104">bookingBusiness: publish</span></span>

 > <span data-ttu-id="91d7f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91d7f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91d7f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91d7f-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="91d7f-107">このビジネスのスケジュール ページを外部の顧客が使用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="91d7f-107">Make the scheduling page of this business available to external customers.</span></span> 

<span data-ttu-id="91d7f-108">True の場合、およびスケジュールのページの URL を**publicUrl**プロパティに**isPublished**プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="91d7f-108">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="91d7f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91d7f-109">Permissions</span></span>
<span data-ttu-id="91d7f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91d7f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91d7f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91d7f-112">Permission type</span></span>      | <span data-ttu-id="91d7f-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91d7f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91d7f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91d7f-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="91d7f-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="91d7f-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="91d7f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91d7f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91d7f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91d7f-117">Not supported.</span></span>   |
|<span data-ttu-id="91d7f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91d7f-118">Application</span></span> | <span data-ttu-id="91d7f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91d7f-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="91d7f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91d7f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="91d7f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91d7f-121">Request headers</span></span>
| <span data-ttu-id="91d7f-122">名前</span><span class="sxs-lookup"><span data-stu-id="91d7f-122">Name</span></span>       | <span data-ttu-id="91d7f-123">説明</span><span class="sxs-lookup"><span data-stu-id="91d7f-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="91d7f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="91d7f-124">Authorization</span></span>  | <span data-ttu-id="91d7f-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="91d7f-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="91d7f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="91d7f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="91d7f-127">応答</span><span class="sxs-lookup"><span data-stu-id="91d7f-127">Response</span></span>
<span data-ttu-id="91d7f-p104">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="91d7f-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91d7f-130">例</span><span class="sxs-lookup"><span data-stu-id="91d7f-130">Example</span></span>
<span data-ttu-id="91d7f-131">次に、この API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="91d7f-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91d7f-132">要求</span><span class="sxs-lookup"><span data-stu-id="91d7f-132">Request</span></span>
<span data-ttu-id="91d7f-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91d7f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="91d7f-134">応答</span><span class="sxs-lookup"><span data-stu-id="91d7f-134">Response</span></span>
<span data-ttu-id="91d7f-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91d7f-135">The following is an example of the response.</span></span> 
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
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
