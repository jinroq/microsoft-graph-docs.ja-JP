---
title: bookingAppointment リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 1956ddac829a2921aba6ebf438ae4815ca56b8d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013130"
---
# <a name="bookingappointment-resource-type"></a><span data-ttu-id="e42fc-104">bookingAppointment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e42fc-104">bookingAppointment resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="e42fc-105">Microsoft の予約ビジネスによって提供される、一連のスタッフメンバーによって実行される、 [Bookingservice](bookingservice.md)の顧客の予定を表します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-105">Represents a customer appointment for a [bookingService](bookingservice.md), performed by a set of staff members, provided by a Microsoft Bookings business.</span></span>


## <a name="methods"></a><span data-ttu-id="e42fc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e42fc-106">Methods</span></span>

| <span data-ttu-id="e42fc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e42fc-107">Method</span></span>           | <span data-ttu-id="e42fc-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e42fc-108">Return Type</span></span>    |<span data-ttu-id="e42fc-109">説明</span><span class="sxs-lookup"><span data-stu-id="e42fc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e42fc-110">予定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e42fc-110">List appointments</span></span>](../api/bookingbusiness-list-appointments.md) |  <span data-ttu-id="e42fc-111">[Bookingappointment](bookingappointment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e42fc-111">[bookingAppointment](bookingappointment.md) collection</span></span> | <span data-ttu-id="e42fc-112">指定した[bookingappointment](../resources/bookingbusiness.md)の**bookingappointment**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-112">Get a list of **bookingAppointment** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="e42fc-113">BookingAppointment の作成</span><span class="sxs-lookup"><span data-stu-id="e42fc-113">Create bookingAppointment</span></span>](../api/bookingbusiness-post-appointments.md) |  [<span data-ttu-id="e42fc-114">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="e42fc-114">bookingAppointment</span></span>](bookingappointment.md) | <span data-ttu-id="e42fc-115">指定した[bookingappointment](../resources/bookingbusiness.md)の新しい**ブック**を作成します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-115">Create a new **bookingAppointment** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="e42fc-116">BookingAppointment を取得する</span><span class="sxs-lookup"><span data-stu-id="e42fc-116">Get bookingAppointment</span></span>](../api/bookingappointment-get.md) | [<span data-ttu-id="e42fc-117">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="e42fc-117">bookingAppointment</span></span>](bookingappointment.md) |<span data-ttu-id="e42fc-118">**Bookingappointment**オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e42fc-118">Read the properties and relationships of **bookingAppointment** object.</span></span>|
|[<span data-ttu-id="e42fc-119">Update</span><span class="sxs-lookup"><span data-stu-id="e42fc-119">Update</span></span>](../api/bookingappointment-update.md) | [<span data-ttu-id="e42fc-120">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="e42fc-120">bookingAppointment</span></span>](bookingappointment.md)    |<span data-ttu-id="e42fc-121">**Bookingappointment**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-121">Update a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="e42fc-122">Delete</span><span class="sxs-lookup"><span data-stu-id="e42fc-122">Delete</span></span>](../api/bookingappointment-delete.md) | <span data-ttu-id="e42fc-123">None</span><span class="sxs-lookup"><span data-stu-id="e42fc-123">None</span></span> |<span data-ttu-id="e42fc-124">**Bookingappointment**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-124">Delete a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="e42fc-125">Cancel</span><span class="sxs-lookup"><span data-stu-id="e42fc-125">Cancel</span></span>](../api/bookingappointment-cancel.md)|<span data-ttu-id="e42fc-126">None</span><span class="sxs-lookup"><span data-stu-id="e42fc-126">None</span></span>| <span data-ttu-id="e42fc-127">**Bookingappointment**オブジェクトを取り消します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-127">Cancel a **bookingAppointment** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e42fc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e42fc-128">Properties</span></span>
| <span data-ttu-id="e42fc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e42fc-129">Property</span></span>     | <span data-ttu-id="e42fc-130">型</span><span class="sxs-lookup"><span data-stu-id="e42fc-130">Type</span></span>   |<span data-ttu-id="e42fc-131">説明</span><span class="sxs-lookup"><span data-stu-id="e42fc-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e42fc-132">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e42fc-132">customerEmailAddress</span></span>|<span data-ttu-id="e42fc-133">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-133">String</span></span>|<span data-ttu-id="e42fc-134">予定を予約している[Bookingcustomer](bookingcustomer.md)の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="e42fc-134">The SMTP address of the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="e42fc-135">Id</span><span class="sxs-lookup"><span data-stu-id="e42fc-135">customerId</span></span>|<span data-ttu-id="e42fc-136">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-136">String</span></span>|<span data-ttu-id="e42fc-137">この予定の[Bookingcustomer](bookingcustomer.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="e42fc-137">The ID of the [bookingCustomer](bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="e42fc-138">予定の作成時に ID が指定されていない場合は、新しい**Bookingcustomer**オブジェクトが作成されます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-138">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="e42fc-139">設定すると、 **customerId**を不変にすることを考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e42fc-139">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="e42fc-140">顧客の所在地</span><span class="sxs-lookup"><span data-stu-id="e42fc-140">customerLocation</span></span>|[<span data-ttu-id="e42fc-141">location</span><span class="sxs-lookup"><span data-stu-id="e42fc-141">location</span></span>](location.md)|<span data-ttu-id="e42fc-142">予定を予約している[Bookingcustomer](bookingcustomer.md)の場所情報を表します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-142">Represents location information for the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="e42fc-143">おける</span><span class="sxs-lookup"><span data-stu-id="e42fc-143">customerName</span></span>|<span data-ttu-id="e42fc-144">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-144">String</span></span>|<span data-ttu-id="e42fc-145">顧客の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-145">The customer's name.</span></span>|
|<span data-ttu-id="e42fc-146">顧客メモ</span><span class="sxs-lookup"><span data-stu-id="e42fc-146">customerNotes</span></span>|<span data-ttu-id="e42fc-147">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-147">String</span></span>|<span data-ttu-id="e42fc-148">この予定に関連付けられている顧客からのメモ。</span><span class="sxs-lookup"><span data-stu-id="e42fc-148">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="e42fc-149">ID でこの**Bookingappointment**を読み取る場合にのみ、値を取得できます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-149">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="e42fc-150">このプロパティは、最初に新しい顧客を使用して予定を作成するときにのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-150">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="e42fc-151">その時点で、その値は**customerId**で表される顧客から計算されます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-151">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="e42fc-152">顧客電話</span><span class="sxs-lookup"><span data-stu-id="e42fc-152">customerPhone</span></span>|<span data-ttu-id="e42fc-153">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-153">String</span></span>|<span data-ttu-id="e42fc-154">お客様の電話番号。</span><span class="sxs-lookup"><span data-stu-id="e42fc-154">The customer's phone number.</span></span>|
|<span data-ttu-id="e42fc-155">duration</span><span class="sxs-lookup"><span data-stu-id="e42fc-155">duration</span></span>|<span data-ttu-id="e42fc-156">期間</span><span class="sxs-lookup"><span data-stu-id="e42fc-156">Duration</span></span>|<span data-ttu-id="e42fc-157">「文字形式」で示されて[](https://www.iso.org/iso-8601-date-and-time-format.html)いる予定の長さ。</span><span class="sxs-lookup"><span data-stu-id="e42fc-157">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="e42fc-158">end</span><span class="sxs-lookup"><span data-stu-id="e42fc-158">end</span></span>|[<span data-ttu-id="e42fc-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e42fc-159">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e42fc-160">予定が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="e42fc-160">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="e42fc-161">id</span><span class="sxs-lookup"><span data-stu-id="e42fc-161">id</span></span>|<span data-ttu-id="e42fc-162">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-162">String</span></span>| <span data-ttu-id="e42fc-163">**Bookingappointment**の ID。</span><span class="sxs-lookup"><span data-stu-id="e42fc-163">The ID of the **bookingAppointment**.</span></span> <span data-ttu-id="e42fc-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e42fc-164">Read-only.</span></span>|
|<span data-ttu-id="e42fc-165">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="e42fc-165">invoiceAmount</span></span>|<span data-ttu-id="e42fc-166">2 行分</span><span class="sxs-lookup"><span data-stu-id="e42fc-166">Double</span></span>|<span data-ttu-id="e42fc-167">請求書の請求金額。</span><span class="sxs-lookup"><span data-stu-id="e42fc-167">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="e42fc-168">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="e42fc-168">invoiceDate</span></span>|[<span data-ttu-id="e42fc-169">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e42fc-169">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e42fc-170">この予定の請求書の日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="e42fc-170">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="e42fc-171">invoiceId</span><span class="sxs-lookup"><span data-stu-id="e42fc-171">invoiceId</span></span>|<span data-ttu-id="e42fc-172">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-172">String</span></span>|<span data-ttu-id="e42fc-173">請求書の ID。</span><span class="sxs-lookup"><span data-stu-id="e42fc-173">The ID of the invoice.</span></span>|
|<span data-ttu-id="e42fc-174">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="e42fc-174">invoiceStatus</span></span>|<span data-ttu-id="e42fc-175">string</span><span class="sxs-lookup"><span data-stu-id="e42fc-175">string</span></span>| <span data-ttu-id="e42fc-176">請求書の状態。</span><span class="sxs-lookup"><span data-stu-id="e42fc-176">The status of the invoice.</span></span> <span data-ttu-id="e42fc-177">使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="e42fc-177">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="e42fc-178">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="e42fc-178">invoiceUrl</span></span>|<span data-ttu-id="e42fc-179">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-179">String</span></span>|<span data-ttu-id="e42fc-180">Microsoft 予約の請求書の URL。</span><span class="sxs-lookup"><span data-stu-id="e42fc-180">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="e42fc-181">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="e42fc-181">optOutOfCustomerEmail</span></span>|<span data-ttu-id="e42fc-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e42fc-182">Boolean</span></span>|<span data-ttu-id="e42fc-183">True は、この予定の[Bookingcustomer](bookingcustomer.md)が、この予定の確認を受信したくないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-183">True indicates that the [bookingCustomer](bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="e42fc-184">postBuffer</span><span class="sxs-lookup"><span data-stu-id="e42fc-184">postBuffer</span></span>|<span data-ttu-id="e42fc-185">期間</span><span class="sxs-lookup"><span data-stu-id="e42fc-185">Duration</span></span>|<span data-ttu-id="e42fc-186">予定が終了した後に、クリーンアップのために確保する時間の長さを例として示します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-186">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="e42fc-187">この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-187">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="e42fc-188">preBuffer</span><span class="sxs-lookup"><span data-stu-id="e42fc-188">preBuffer</span></span>|<span data-ttu-id="e42fc-189">期間</span><span class="sxs-lookup"><span data-stu-id="e42fc-189">Duration</span></span>|<span data-ttu-id="e42fc-190">準備のために予定が開始されるまでの時間を例として示します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-190">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="e42fc-191">この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-191">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="e42fc-192">代金</span><span class="sxs-lookup"><span data-stu-id="e42fc-192">price</span></span>|<span data-ttu-id="e42fc-193">2 行分</span><span class="sxs-lookup"><span data-stu-id="e42fc-193">Double</span></span>|<span data-ttu-id="e42fc-194">指定した[Bookingservice](bookingservice.md)の予定に対する正規の価格。</span><span class="sxs-lookup"><span data-stu-id="e42fc-194">The regular price for an appointment for the specified [bookingService](bookingservice.md).</span></span>|
|<span data-ttu-id="e42fc-195">priceType</span><span class="sxs-lookup"><span data-stu-id="e42fc-195">priceType</span></span>|<span data-ttu-id="e42fc-196">string</span><span class="sxs-lookup"><span data-stu-id="e42fc-196">string</span></span>| <span data-ttu-id="e42fc-197">サービスの価格構造を柔軟に提供するための設定。</span><span class="sxs-lookup"><span data-stu-id="e42fc-197">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="e42fc-198">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="e42fc-198">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="e42fc-199">isp</span><span class="sxs-lookup"><span data-stu-id="e42fc-199">reminders</span></span>|<span data-ttu-id="e42fc-200">[Bookingreminder](bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e42fc-200">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="e42fc-201">この予定に対して送信された顧客のアラームのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e42fc-201">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="e42fc-202">このプロパティの値は、この**Bookingappointment**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-202">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="e42fc-203">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="e42fc-203">selfServiceAppointmentId</span></span>|<span data-ttu-id="e42fc-204">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-204">String</span></span>|<span data-ttu-id="e42fc-205">顧客に代わってスタッフメンバーではなく、顧客が [スケジュール] ページで直接作成された予定の場合は、予定の追加の追跡 ID。</span><span class="sxs-lookup"><span data-stu-id="e42fc-205">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="e42fc-206">serviceId</span><span class="sxs-lookup"><span data-stu-id="e42fc-206">serviceId</span></span>|<span data-ttu-id="e42fc-207">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-207">String</span></span>|<span data-ttu-id="e42fc-208">この予定に関連付けられている[Bookingservice](bookingservice.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="e42fc-208">The ID of the [bookingService](bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="e42fc-209">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="e42fc-209">serviceLocation</span></span>|[<span data-ttu-id="e42fc-210">location</span><span class="sxs-lookup"><span data-stu-id="e42fc-210">location</span></span>](location.md)|<span data-ttu-id="e42fc-211">サービスが配信される場所。</span><span class="sxs-lookup"><span data-stu-id="e42fc-211">The location where the service is delivered.</span></span>|
|<span data-ttu-id="e42fc-212">serviceName</span><span class="sxs-lookup"><span data-stu-id="e42fc-212">serviceName</span></span>|<span data-ttu-id="e42fc-213">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-213">String</span></span>|<span data-ttu-id="e42fc-214">この予定に関連付けられている**Bookingservice**の名前です。</span><span class="sxs-lookup"><span data-stu-id="e42fc-214">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="e42fc-215">新しい予定を作成するときは、このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="e42fc-215">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="e42fc-216">指定しない場合、 **serviceId**プロパティによって、予定に関連付けられているサービスから計算されます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-216">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="e42fc-217">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="e42fc-217">serviceNotes</span></span>|<span data-ttu-id="e42fc-218">String</span><span class="sxs-lookup"><span data-stu-id="e42fc-218">String</span></span>|<span data-ttu-id="e42fc-219">[BookingStaffMember](bookingstaffmember.md)からのメモ。</span><span class="sxs-lookup"><span data-stu-id="e42fc-219">Notes from a [bookingStaffMember](bookingstaffmember.md).</span></span> <span data-ttu-id="e42fc-220">このプロパティの値は、この**Bookingappointment**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="e42fc-220">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="e42fc-221">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="e42fc-221">staffMemberIds</span></span>|<span data-ttu-id="e42fc-222">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e42fc-222">String collection</span></span>|<span data-ttu-id="e42fc-223">この予定でスケジュールされている各[bookingStaffMember](bookingstaffmember.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="e42fc-223">The ID of each [bookingStaffMember](bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="e42fc-224">開始</span><span class="sxs-lookup"><span data-stu-id="e42fc-224">start</span></span>|[<span data-ttu-id="e42fc-225">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e42fc-225">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e42fc-226">予定が開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="e42fc-226">The date, time, and time zone that the appointment begins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e42fc-227">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e42fc-227">Relationships</span></span>
<span data-ttu-id="e42fc-228">なし</span><span class="sxs-lookup"><span data-stu-id="e42fc-228">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e42fc-229">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e42fc-229">JSON representation</span></span>

<span data-ttu-id="e42fc-230">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e42fc-230">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingAppointment"
}-->

```json
{
  "customerEmailAddress": "String",
  "customerId": "String",
  "customerLocation": {"@odata.type": "microsoft.graph.location"},
  "customerName": "String",
  "customerNotes": "String",
  "customerPhone": "String",
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "optOutOfCustomerEmail": true,
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": "string",
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
