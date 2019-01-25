---
title: Bookingbusiness を更新します。
description: BookingBusiness オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: dba24dafef030ae53fc83fb06d1cc7b99ed71e81
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528803"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="26f8f-103">Bookingbusiness を更新します。</span><span class="sxs-lookup"><span data-stu-id="26f8f-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26f8f-104">[BookingBusiness](../resources/bookingbusiness.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="26f8f-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="26f8f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26f8f-105">Permissions</span></span>
<span data-ttu-id="26f8f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26f8f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26f8f-108">Permission type</span></span>      | <span data-ttu-id="26f8f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26f8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26f8f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26f8f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="26f8f-111">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="26f8f-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="26f8f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26f8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26f8f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26f8f-113">Not supported.</span></span>   |
|<span data-ttu-id="26f8f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26f8f-114">Application</span></span> | <span data-ttu-id="26f8f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26f8f-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="26f8f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26f8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="26f8f-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26f8f-117">Optional request headers</span></span>
| <span data-ttu-id="26f8f-118">名前</span><span class="sxs-lookup"><span data-stu-id="26f8f-118">Name</span></span>       | <span data-ttu-id="26f8f-119">説明</span><span class="sxs-lookup"><span data-stu-id="26f8f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="26f8f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="26f8f-120">Authorization</span></span>  | <span data-ttu-id="26f8f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="26f8f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="26f8f-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="26f8f-122">Request body</span></span>
<span data-ttu-id="26f8f-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="26f8f-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26f8f-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26f8f-126">Property</span></span>     | <span data-ttu-id="26f8f-127">型</span><span class="sxs-lookup"><span data-stu-id="26f8f-127">Type</span></span>   |<span data-ttu-id="26f8f-128">説明</span><span class="sxs-lookup"><span data-stu-id="26f8f-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26f8f-129">address</span><span class="sxs-lookup"><span data-stu-id="26f8f-129">address</span></span>|[<span data-ttu-id="26f8f-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="26f8f-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="26f8f-131">ビジネスの住所。</span><span class="sxs-lookup"><span data-stu-id="26f8f-131">The street address of the business.</span></span>|
|<span data-ttu-id="26f8f-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="26f8f-132">businessHours</span></span>|<span data-ttu-id="26f8f-133">[bookingWorkHours](../resources/bookingworkhours.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="26f8f-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="26f8f-134">ビジネスの操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="26f8f-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="26f8f-135">businessType</span><span class="sxs-lookup"><span data-stu-id="26f8f-135">businessType</span></span>|<span data-ttu-id="26f8f-136">String</span><span class="sxs-lookup"><span data-stu-id="26f8f-136">String</span></span>|<span data-ttu-id="26f8f-137">ビジネスの種類。</span><span class="sxs-lookup"><span data-stu-id="26f8f-137">The type of business.</span></span>|
|<span data-ttu-id="26f8f-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="26f8f-138">defaultCurrencyIso</span></span>|<span data-ttu-id="26f8f-139">String</span><span class="sxs-lookup"><span data-stu-id="26f8f-139">String</span></span>|<span data-ttu-id="26f8f-140">ビジネスが Microsoft 予約上で動作する通貨コード。</span><span class="sxs-lookup"><span data-stu-id="26f8f-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="26f8f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="26f8f-141">displayName</span></span>|<span data-ttu-id="26f8f-142">String</span><span class="sxs-lookup"><span data-stu-id="26f8f-142">String</span></span>|<span data-ttu-id="26f8f-143">ビジネス顧客とやり取りするための名前です。</span><span class="sxs-lookup"><span data-stu-id="26f8f-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="26f8f-144">email</span><span class="sxs-lookup"><span data-stu-id="26f8f-144">email</span></span>|<span data-ttu-id="26f8f-145">String</span><span class="sxs-lookup"><span data-stu-id="26f8f-145">String</span></span>|<span data-ttu-id="26f8f-146">ビジネスの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="26f8f-146">The email address for the business.</span></span>|
|<span data-ttu-id="26f8f-147">phone</span><span class="sxs-lookup"><span data-stu-id="26f8f-147">phone</span></span>|<span data-ttu-id="26f8f-148">String</span><span class="sxs-lookup"><span data-stu-id="26f8f-148">String</span></span>|<span data-ttu-id="26f8f-149">ビジネスの電話番号です。</span><span class="sxs-lookup"><span data-stu-id="26f8f-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="26f8f-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="26f8f-150">schedulingPolicy</span></span>|[<span data-ttu-id="26f8f-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="26f8f-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="26f8f-152">このビジネスでの予約を作成する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8f-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="26f8f-153">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="26f8f-153">webSiteUrl</span></span>|<span data-ttu-id="26f8f-154">String</span><span class="sxs-lookup"><span data-stu-id="26f8f-154">String</span></span>|<span data-ttu-id="26f8f-155">ビジネスの web サイトの URL です。</span><span class="sxs-lookup"><span data-stu-id="26f8f-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="26f8f-156">応答</span><span class="sxs-lookup"><span data-stu-id="26f8f-156">Response</span></span>
<span data-ttu-id="26f8f-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="26f8f-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26f8f-159">例</span><span class="sxs-lookup"><span data-stu-id="26f8f-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26f8f-160">要求</span><span class="sxs-lookup"><span data-stu-id="26f8f-160">Request</span></span>
<span data-ttu-id="26f8f-161">次の使用例は、ビジネスの電子メール アドレスおよびビジネス既定の予約の時間帯を 1 時間に変更し、最大で 30 日間の予約を進めるには、ポリシーのスケジュール設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="26f8f-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="26f8f-162">応答</span><span class="sxs-lookup"><span data-stu-id="26f8f-162">Response</span></span>
<span data-ttu-id="26f8f-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26f8f-163">The following is an example of the response.</span></span> <span data-ttu-id="26f8f-164">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="26f8f-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="26f8f-165">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="26f8f-165">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
