---
title: Microsoft Graph では、Microsoft 予約 API を使用します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 494b13016c20124e1a81f996d332c97c15e46852
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915733"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="e00ac-104">Microsoft Graph では、Microsoft 予約 API を使用します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 > <span data-ttu-id="e00ac-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e00ac-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e00ac-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e00ac-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e00ac-107">Microsoft の予約には、スモール ビジネスの経営者がお客様の予約と最小限の設定で情報を管理することができます。</span><span class="sxs-lookup"><span data-stu-id="e00ac-107">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="e00ac-108">ビジネス所有者は、各業務の一連のサービスを提供することで、1 つまたは複数の企業を作成できます。</span><span class="sxs-lookup"><span data-stu-id="e00ac-108">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="e00ac-109">所有者では、スタッフのメンバーを設定でき、各スタッフ メンバーを実行するサービスを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="e00ac-109">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="e00ac-110">顧客は、オンラインまたはモバイル アプリケーションでは、そのビジネスで特定のサービスの予定を予約することができます。</span><span class="sxs-lookup"><span data-stu-id="e00ac-110">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="e00ac-111">予約する予定の時刻は最新ビジネス、スタッフ、および顧客の関係を保証します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-111">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="e00ac-112">プログラムを使用して、予約 API では、 [bookingBusiness](bookingbusiness.md)には、次のオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e00ac-112">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="e00ac-113">1 つまたは複数の[bookingStaffMember](bookingstaffmember.md)オブジェクト</span><span class="sxs-lookup"><span data-stu-id="e00ac-113">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="e00ac-114">1 つまたは複数の[bookingService](bookingservice.md)オブジェクト</span><span class="sxs-lookup"><span data-stu-id="e00ac-114">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="e00ac-115">[BookingAppointment](bookingappointment.md)のインスタンスのセット</span><span class="sxs-lookup"><span data-stu-id="e00ac-115">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="e00ac-116">一連の[bookingCustomer](bookingcustomer.md)オブジェクト</span><span class="sxs-lookup"><span data-stu-id="e00ac-116">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="e00ac-117">予約 REST API を使用します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-117">Using the Bookings REST API</span></span>

<span data-ttu-id="e00ac-118">最初にビジネスのお客様の予定を予約する前に、次の手順を説明します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-118">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="e00ac-119">対応する操作に対して適切な[アクセス トークン](/graph/auth-overview)を提供することを確認します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-119">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="e00ac-120">ビジネスには、 [Office 365 のビジネス プレミアム](https://products.office.com/en-us/business/office-365-business-premium)サブスクリプションを確認します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-120">Make sure the business has an [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="e00ac-121">新しい**bookingBusiness**を作成するには、POST 操作のエンティティ セットに送信します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-121">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="e00ac-122">最低限、顧客に表示される新しいビジネスの名前を指定する必要があります。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e00ac-122">At minimum, you should specify a name for the new business that customers will see: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="e00ac-123">POST 応答で返される新しい**bookingBusiness**の**id**プロパティを使用して、ビジネスの設定の[カスタマイズ](../api/bookingbusiness-update.md)を続行して、スタッフとのビジネスのサービスを追加します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-123">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="e00ac-124">ビジネスの個々 のスタッフのメンバーを追加します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e00ac-124">Add individual staff members for the business: <!-- { "blockType": "ignored" } --></span></span>
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
4. <span data-ttu-id="e00ac-125">ビジネスによって提供される各サービスを定義します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e00ac-125">Define each service offered by the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="e00ac-126">顧客およびビジネス オペレーターが予約を開始できるようにするのには、ビジネスのスケジュールのページを公開するには。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e00ac-126">Publish the scheduling page for the business, to let customers and business operators start booking appointments: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="e00ac-127">一般で、Office 365 テナント内のすべての予約会社を一覧表示します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e00ac-127">In general, to list all the booking businesses in the Office 365 tenant: <!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="e00ac-128">一般的なユース ケース</span><span class="sxs-lookup"><span data-stu-id="e00ac-128">Common use cases</span></span> 

<span data-ttu-id="e00ac-129">予約 API でのビジネスの一般的な操作を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-129">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="e00ac-130">ユース ケース</span><span class="sxs-lookup"><span data-stu-id="e00ac-130">Use cases</span></span>        | <span data-ttu-id="e00ac-131">REST リソース</span><span class="sxs-lookup"><span data-stu-id="e00ac-131">REST resources</span></span> | <span data-ttu-id="e00ac-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="e00ac-132">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="e00ac-133">ビジネスの作成、取得、更新、削除</span><span class="sxs-lookup"><span data-stu-id="e00ac-133">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="e00ac-134">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="e00ac-134">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="e00ac-135">BookingBusiness の方法</span><span class="sxs-lookup"><span data-stu-id="e00ac-135">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="e00ac-136">スケジュー リング ポリシーを更新します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-136">Update the scheduling policy</span></span> | [<span data-ttu-id="e00ac-137">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="e00ac-137">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="e00ac-138">BookingBusiness を更新します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-138">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="e00ac-139">追加、取得、更新、またはスタッフのメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-139">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="e00ac-140">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="e00ac-140">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="e00ac-141">BookingStaffMember の方法</span><span class="sxs-lookup"><span data-stu-id="e00ac-141">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="e00ac-142">追加、取得、更新、またはサービスを削除します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-142">Add, get, update, or delete services</span></span> | [<span data-ttu-id="e00ac-143">bookingService</span><span class="sxs-lookup"><span data-stu-id="e00ac-143">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="e00ac-144">BookingService の方法</span><span class="sxs-lookup"><span data-stu-id="e00ac-144">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="e00ac-145">公開または公開取り下げのスケジュール ページ</span><span class="sxs-lookup"><span data-stu-id="e00ac-145">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="e00ac-146">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="e00ac-146">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="e00ac-147">発行</span><span class="sxs-lookup"><span data-stu-id="e00ac-147">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="e00ac-148">公開取り下げ</span><span class="sxs-lookup"><span data-stu-id="e00ac-148">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="e00ac-149">作成、取得、更新、削除、または予定をキャンセル</span><span class="sxs-lookup"><span data-stu-id="e00ac-149">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="e00ac-150">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="e00ac-150">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="e00ac-151">BookingAppointment の方法</span><span class="sxs-lookup"><span data-stu-id="e00ac-151">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="e00ac-152">日付の範囲で予定を取得します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-152">Get appointments in a date range</span></span> | [<span data-ttu-id="e00ac-153">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="e00ac-153">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="e00ac-154">予約予定表ビューを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-154">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="e00ac-155">通貨を取得します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-155">Get currency</span></span> | [<span data-ttu-id="e00ac-156">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="e00ac-156">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="e00ac-157">BookingCurrency の方法</span><span class="sxs-lookup"><span data-stu-id="e00ac-157">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="e00ac-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="e00ac-158">See also</span></span>

- <span data-ttu-id="e00ac-159">
  [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。</span><span class="sxs-lookup"><span data-stu-id="e00ac-159">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="e00ac-160">[Microsoft Graph を使ってパートナーのいくつかの方法](https://developer.microsoft.com/graph/graph/examples#partners)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e00ac-160">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="e00ac-161">Graph で[のアクセス許可](/graph/permissions-reference)を選択する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="e00ac-161">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
