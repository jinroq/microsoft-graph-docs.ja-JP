---
title: Bookingbusiness を更新します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 53115469821bc39c05c4e7a262e5f9fc15b376ce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824998"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="2aee5-104">Bookingbusiness を更新します。</span><span class="sxs-lookup"><span data-stu-id="2aee5-104">Update bookingbusiness</span></span>

 > <span data-ttu-id="2aee5-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2aee5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2aee5-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2aee5-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="2aee5-107">[BookingBusiness](../resources/bookingbusiness.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2aee5-107">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2aee5-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2aee5-108">Permissions</span></span>
<span data-ttu-id="2aee5-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2aee5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2aee5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2aee5-111">Permission type</span></span>      | <span data-ttu-id="2aee5-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2aee5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2aee5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2aee5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="2aee5-114">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="2aee5-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2aee5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2aee5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2aee5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2aee5-116">Not supported.</span></span>   |
|<span data-ttu-id="2aee5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2aee5-117">Application</span></span> | <span data-ttu-id="2aee5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2aee5-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="2aee5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2aee5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="2aee5-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2aee5-120">Optional request headers</span></span>
| <span data-ttu-id="2aee5-121">名前</span><span class="sxs-lookup"><span data-stu-id="2aee5-121">Name</span></span>       | <span data-ttu-id="2aee5-122">説明</span><span class="sxs-lookup"><span data-stu-id="2aee5-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2aee5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2aee5-123">Authorization</span></span>  | <span data-ttu-id="2aee5-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2aee5-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2aee5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2aee5-125">Request body</span></span>
<span data-ttu-id="2aee5-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2aee5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2aee5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2aee5-129">Property</span></span>     | <span data-ttu-id="2aee5-130">種類</span><span class="sxs-lookup"><span data-stu-id="2aee5-130">Type</span></span>   |<span data-ttu-id="2aee5-131">説明</span><span class="sxs-lookup"><span data-stu-id="2aee5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2aee5-132">address</span><span class="sxs-lookup"><span data-stu-id="2aee5-132">address</span></span>|[<span data-ttu-id="2aee5-133">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2aee5-133">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="2aee5-134">ビジネスの住所。</span><span class="sxs-lookup"><span data-stu-id="2aee5-134">The street address of the business.</span></span>|
|<span data-ttu-id="2aee5-135">businessHours</span><span class="sxs-lookup"><span data-stu-id="2aee5-135">businessHours</span></span>|<span data-ttu-id="2aee5-136">[bookingWorkHours](../resources/bookingworkhours.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2aee5-136">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="2aee5-137">ビジネスの操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="2aee5-137">The hours of operation for the business.</span></span>|
|<span data-ttu-id="2aee5-138">businessType</span><span class="sxs-lookup"><span data-stu-id="2aee5-138">businessType</span></span>|<span data-ttu-id="2aee5-139">String</span><span class="sxs-lookup"><span data-stu-id="2aee5-139">String</span></span>|<span data-ttu-id="2aee5-140">ビジネスの種類。</span><span class="sxs-lookup"><span data-stu-id="2aee5-140">The type of business.</span></span>|
|<span data-ttu-id="2aee5-141">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="2aee5-141">defaultCurrencyIso</span></span>|<span data-ttu-id="2aee5-142">String</span><span class="sxs-lookup"><span data-stu-id="2aee5-142">String</span></span>|<span data-ttu-id="2aee5-143">ビジネスが Microsoft 予約上で動作する通貨コード。</span><span class="sxs-lookup"><span data-stu-id="2aee5-143">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="2aee5-144">displayName</span><span class="sxs-lookup"><span data-stu-id="2aee5-144">displayName</span></span>|<span data-ttu-id="2aee5-145">String</span><span class="sxs-lookup"><span data-stu-id="2aee5-145">String</span></span>|<span data-ttu-id="2aee5-146">ビジネス顧客とやり取りするための名前です。</span><span class="sxs-lookup"><span data-stu-id="2aee5-146">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="2aee5-147">email</span><span class="sxs-lookup"><span data-stu-id="2aee5-147">email</span></span>|<span data-ttu-id="2aee5-148">String</span><span class="sxs-lookup"><span data-stu-id="2aee5-148">String</span></span>|<span data-ttu-id="2aee5-149">ビジネスの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="2aee5-149">The email address for the business.</span></span>|
|<span data-ttu-id="2aee5-150">phone</span><span class="sxs-lookup"><span data-stu-id="2aee5-150">phone</span></span>|<span data-ttu-id="2aee5-151">String</span><span class="sxs-lookup"><span data-stu-id="2aee5-151">String</span></span>|<span data-ttu-id="2aee5-152">ビジネスの電話番号です。</span><span class="sxs-lookup"><span data-stu-id="2aee5-152">The telephone number for the business.</span></span>|
|<span data-ttu-id="2aee5-153">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="2aee5-153">schedulingPolicy</span></span>|[<span data-ttu-id="2aee5-154">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="2aee5-154">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="2aee5-155">このビジネスでの予約を作成する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="2aee5-155">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="2aee5-156">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="2aee5-156">webSiteUrl</span></span>|<span data-ttu-id="2aee5-157">String</span><span class="sxs-lookup"><span data-stu-id="2aee5-157">String</span></span>|<span data-ttu-id="2aee5-158">ビジネスの web サイトの URL です。</span><span class="sxs-lookup"><span data-stu-id="2aee5-158">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="2aee5-159">応答</span><span class="sxs-lookup"><span data-stu-id="2aee5-159">Response</span></span>
<span data-ttu-id="2aee5-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2aee5-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2aee5-162">例</span><span class="sxs-lookup"><span data-stu-id="2aee5-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2aee5-163">要求</span><span class="sxs-lookup"><span data-stu-id="2aee5-163">Request</span></span>
<span data-ttu-id="2aee5-164">次の使用例は、ビジネスの電子メール アドレスおよびビジネス既定の予約の時間帯を 1 時間に変更し、最大で 30 日間の予約を進めるには、ポリシーのスケジュール設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="2aee5-164">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```
##### <a name="response"></a><span data-ttu-id="2aee5-165">応答</span><span class="sxs-lookup"><span data-stu-id="2aee5-165">Response</span></span>
<span data-ttu-id="2aee5-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2aee5-166">The following is an example of the response.</span></span> <span data-ttu-id="2aee5-167">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2aee5-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2aee5-168">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2aee5-168">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
