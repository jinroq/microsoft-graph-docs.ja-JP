---
title: Microsoft Graph で Microsoft Bookings API を使用する
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7fc58a4fe0fb616963fd91d83a401d4ad8e1c43e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529860"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="9078b-104">Microsoft Graph で Microsoft Bookings API を使用する</span><span class="sxs-lookup"><span data-stu-id="9078b-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="9078b-105">Microsoft Bookings では、中小企業のオーナーが最小限の設定で顧客の予約と情報を管理できます。</span><span class="sxs-lookup"><span data-stu-id="9078b-105">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="9078b-106">ビジネス オーナーは、一連のサービスを提供するビジネスを 1 つ以上作成できます。</span><span class="sxs-lookup"><span data-stu-id="9078b-106">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="9078b-107">オーナーはスタッフを設定し、各スタッフが実施するサービスを指定できます。</span><span class="sxs-lookup"><span data-stu-id="9078b-107">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="9078b-108">顧客は当該ビジネスの特定のサービスをオンラインまたはモバイル アプリから予約できます。</span><span class="sxs-lookup"><span data-stu-id="9078b-108">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="9078b-109">Bookings では、ビジネス、スタッフ、顧客に対し常に最新の予約情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="9078b-109">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="9078b-110">Bookings API の [bookingBusiness](bookingbusiness.md) は、プログラムで次のオブジェクトを使用します。</span><span class="sxs-lookup"><span data-stu-id="9078b-110">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="9078b-111">1 つまたは複数の [bookingStaffMember](bookingstaffmember.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="9078b-111">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="9078b-112">1 つまたは複数の [bookingService](bookingservice.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="9078b-112">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="9078b-113">一連の[bookingAppointment](bookingappointment.md)インスタンス</span><span class="sxs-lookup"><span data-stu-id="9078b-113">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="9078b-114">一連の[bookingCustomer](bookingcustomer.md)オブジェクト</span><span class="sxs-lookup"><span data-stu-id="9078b-114">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="9078b-115">Bookings REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="9078b-115">Using the Bookings REST API</span></span>

<span data-ttu-id="9078b-116">顧客の予約を初めて受け付ける前に、次の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="9078b-116">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="9078b-117">対応する操作のための適切な[アクセス トークン](/graph/auth-overview)を提供していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9078b-117">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="9078b-118">ビジネスで [Office 365 Business Premium](https://products.office.com/ja-JP/business/office-365-business-premium) サブスクリプションを購入していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9078b-118">Make sure the business has an [Office 365 Business Premium](https://products.office.com/ja-JP/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="9078b-119">エンティティ セットに POST 操作を送信して新しい **bookingBusiness** を作成します。</span><span class="sxs-lookup"><span data-stu-id="9078b-119">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="9078b-120">最小限でも、顧客に対して表示される新しいビジネスの名前を指定してください。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9078b-120">At minimum, you should specify a name for the new business that customers will see: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="9078b-121">POST 応答で返される新しい **bookingBusiness** の **id** プロパティを使用して、ビジネス設定を[カスタマイズ](../api/bookingbusiness-update.md)し、ビジネスのスタッフとサービスを追加します。</span><span class="sxs-lookup"><span data-stu-id="9078b-121">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="9078b-122">ビジネスの個々のスタッフを追加します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9078b-122">Add individual staff members for the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. <span data-ttu-id="9078b-123">ビジネスで提供する各サービスを定義します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9078b-123">Define each service offered by the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="9078b-124">ビジネスのスケジュール ページを公開し、顧客とビジネス運営担当者が予約の受付を開始できるようにします。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9078b-124">Publish the scheduling page for the business, to let customers and business operators start booking appointments: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="9078b-125">一般に、Office 365 テナントの予約ビジネスをすべて一覧表示するには次のようにします。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9078b-125">In general, to list all the booking businesses in the Office 365 tenant: <!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="9078b-126">一般的なユース ケース</span><span class="sxs-lookup"><span data-stu-id="9078b-126">Common use cases</span></span> 

<span data-ttu-id="9078b-127">次の表は、Bookings API でのビジネスの一般的な操作を示します。</span><span class="sxs-lookup"><span data-stu-id="9078b-127">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="9078b-128">ユース ケース</span><span class="sxs-lookup"><span data-stu-id="9078b-128">Use cases</span></span>        | <span data-ttu-id="9078b-129">REST リソース</span><span class="sxs-lookup"><span data-stu-id="9078b-129">REST resources</span></span> | <span data-ttu-id="9078b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="9078b-130">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="9078b-131">ビジネスの作成、取得、更新、または削除</span><span class="sxs-lookup"><span data-stu-id="9078b-131">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="9078b-132">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9078b-132">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="9078b-133">bookingBusiness のメソッド</span><span class="sxs-lookup"><span data-stu-id="9078b-133">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="9078b-134">スケジュール ポリシーの更新</span><span class="sxs-lookup"><span data-stu-id="9078b-134">Update the scheduling policy</span></span> | [<span data-ttu-id="9078b-135">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="9078b-135">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="9078b-136">bookingBusiness を更新する</span><span class="sxs-lookup"><span data-stu-id="9078b-136">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="9078b-137">スタッフの追加、取得、更新、または削除</span><span class="sxs-lookup"><span data-stu-id="9078b-137">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="9078b-138">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="9078b-138">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="9078b-139">bookingStaffMember のメソッド</span><span class="sxs-lookup"><span data-stu-id="9078b-139">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="9078b-140">サービスの追加、取得、更新、または削除</span><span class="sxs-lookup"><span data-stu-id="9078b-140">Add, get, update, or delete services</span></span> | [<span data-ttu-id="9078b-141">bookingService</span><span class="sxs-lookup"><span data-stu-id="9078b-141">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="9078b-142">bookingService のメソッド</span><span class="sxs-lookup"><span data-stu-id="9078b-142">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="9078b-143">スケジュール ページの公開または公開の取り消し</span><span class="sxs-lookup"><span data-stu-id="9078b-143">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="9078b-144">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9078b-144">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="9078b-145">publish</span><span class="sxs-lookup"><span data-stu-id="9078b-145">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="9078b-146">unpublish</span><span class="sxs-lookup"><span data-stu-id="9078b-146">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="9078b-147">予約の作成、取得、更新、削除、またはキャンセル</span><span class="sxs-lookup"><span data-stu-id="9078b-147">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="9078b-148">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="9078b-148">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="9078b-149">bookingAppointment のメソッド</span><span class="sxs-lookup"><span data-stu-id="9078b-149">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="9078b-150">日付範囲内の予約の取得</span><span class="sxs-lookup"><span data-stu-id="9078b-150">Get appointments in a date range</span></span> | [<span data-ttu-id="9078b-151">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9078b-151">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="9078b-152">List Bookings calendarView</span><span class="sxs-lookup"><span data-stu-id="9078b-152">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="9078b-153">通貨の取得</span><span class="sxs-lookup"><span data-stu-id="9078b-153">Get currency</span></span> | [<span data-ttu-id="9078b-154">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="9078b-154">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="9078b-155">bookingCurrency のメソッド</span><span class="sxs-lookup"><span data-stu-id="9078b-155">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="9078b-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="9078b-156">See also</span></span>

- <span data-ttu-id="9078b-157">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。</span><span class="sxs-lookup"><span data-stu-id="9078b-157">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="9078b-158">「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9078b-158">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="9078b-159">Microsoft Graph で[権限](/graph/permissions-reference)を選択する方法を理解してください。</span><span class="sxs-lookup"><span data-stu-id="9078b-159">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/booking-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
