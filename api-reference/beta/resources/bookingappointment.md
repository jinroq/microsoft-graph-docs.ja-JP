---
title: bookingappointment リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c5868788159f0602c1f8a263138c7ce9107c2c94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535523"
---
# <a name="bookingappointment-resource-type"></a><span data-ttu-id="06985-104">bookingappointment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06985-104">bookingAppointment resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="06985-105">Microsoft の予約ビジネスによって提供される、一連のスタッフメンバーによって実行される、 [bookingservice](bookingservice.md)の顧客の予定を表します。</span><span class="sxs-lookup"><span data-stu-id="06985-105">Represents a customer appointment for a [bookingService](bookingservice.md), performed by a set of staff members, provided by a Microsoft Bookings business.</span></span>


## <a name="methods"></a><span data-ttu-id="06985-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="06985-106">Methods</span></span>

| <span data-ttu-id="06985-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="06985-107">Method</span></span>           | <span data-ttu-id="06985-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06985-108">Return Type</span></span>    |<span data-ttu-id="06985-109">説明</span><span class="sxs-lookup"><span data-stu-id="06985-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06985-110">予定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="06985-110">List appointments</span></span>](../api/bookingbusiness-list-appointments.md) |  <span data-ttu-id="06985-111">[bookingappointment](bookingappointment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="06985-111">[bookingAppointment](bookingappointment.md) collection</span></span> | <span data-ttu-id="06985-112">指定した[bookingappointment](../resources/bookingbusiness.md)の**bookingappointment**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="06985-112">Get a list of **bookingAppointment** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="06985-113">bookingappointment の作成</span><span class="sxs-lookup"><span data-stu-id="06985-113">Create bookingAppointment</span></span>](../api/bookingbusiness-post-appointments.md) |  [<span data-ttu-id="06985-114">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="06985-114">bookingAppointment</span></span>](bookingappointment.md) | <span data-ttu-id="06985-115">指定した[bookingappointment](../resources/bookingbusiness.md)の新しい**ブック**を作成します。</span><span class="sxs-lookup"><span data-stu-id="06985-115">Create a new **bookingAppointment** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="06985-116">bookingappointment を取得する</span><span class="sxs-lookup"><span data-stu-id="06985-116">Get bookingAppointment</span></span>](../api/bookingappointment-get.md) | [<span data-ttu-id="06985-117">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="06985-117">bookingAppointment</span></span>](bookingappointment.md) |<span data-ttu-id="06985-118">**bookingappointment**オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="06985-118">Read the properties and relationships of **bookingAppointment** object.</span></span>|
|[<span data-ttu-id="06985-119">更新</span><span class="sxs-lookup"><span data-stu-id="06985-119">Update</span></span>](../api/bookingappointment-update.md) | [<span data-ttu-id="06985-120">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="06985-120">bookingAppointment</span></span>](bookingappointment.md)    |<span data-ttu-id="06985-121">**bookingappointment**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="06985-121">Update a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="06985-122">削除</span><span class="sxs-lookup"><span data-stu-id="06985-122">Delete</span></span>](../api/bookingappointment-delete.md) | <span data-ttu-id="06985-123">なし</span><span class="sxs-lookup"><span data-stu-id="06985-123">None</span></span> |<span data-ttu-id="06985-124">**bookingappointment**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="06985-124">Delete a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="06985-125">Cancel</span><span class="sxs-lookup"><span data-stu-id="06985-125">Cancel</span></span>](../api/bookingappointment-cancel.md)|<span data-ttu-id="06985-126">なし</span><span class="sxs-lookup"><span data-stu-id="06985-126">None</span></span>| <span data-ttu-id="06985-127">**bookingappointment**オブジェクトを取り消します。</span><span class="sxs-lookup"><span data-stu-id="06985-127">Cancel a **bookingAppointment** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06985-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06985-128">Properties</span></span>
| <span data-ttu-id="06985-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06985-129">Property</span></span>     | <span data-ttu-id="06985-130">型</span><span class="sxs-lookup"><span data-stu-id="06985-130">Type</span></span>   |<span data-ttu-id="06985-131">説明</span><span class="sxs-lookup"><span data-stu-id="06985-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06985-132">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="06985-132">customerEmailAddress</span></span>|<span data-ttu-id="06985-133">String</span><span class="sxs-lookup"><span data-stu-id="06985-133">String</span></span>|<span data-ttu-id="06985-134">予定を予約している[bookingcustomer](bookingcustomer.md)の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="06985-134">The SMTP address of the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="06985-135">id</span><span class="sxs-lookup"><span data-stu-id="06985-135">customerId</span></span>|<span data-ttu-id="06985-136">String</span><span class="sxs-lookup"><span data-stu-id="06985-136">String</span></span>|<span data-ttu-id="06985-137">この予定の[bookingcustomer](bookingcustomer.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="06985-137">The ID of the [bookingCustomer](bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="06985-138">予定の作成時に ID が指定されていない場合は、新しい**bookingcustomer**オブジェクトが作成されます。</span><span class="sxs-lookup"><span data-stu-id="06985-138">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="06985-139">設定すると、 **customerId**を不変にすることを考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="06985-139">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="06985-140">顧客の所在地</span><span class="sxs-lookup"><span data-stu-id="06985-140">customerLocation</span></span>|[<span data-ttu-id="06985-141">location</span><span class="sxs-lookup"><span data-stu-id="06985-141">location</span></span>](location.md)|<span data-ttu-id="06985-142">予定を予約している[bookingcustomer](bookingcustomer.md)の場所情報を表します。</span><span class="sxs-lookup"><span data-stu-id="06985-142">Represents location information for the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="06985-143">おける</span><span class="sxs-lookup"><span data-stu-id="06985-143">customerName</span></span>|<span data-ttu-id="06985-144">String</span><span class="sxs-lookup"><span data-stu-id="06985-144">String</span></span>|<span data-ttu-id="06985-145">顧客の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="06985-145">The customer's name.</span></span>|
|<span data-ttu-id="06985-146">顧客メモ</span><span class="sxs-lookup"><span data-stu-id="06985-146">customerNotes</span></span>|<span data-ttu-id="06985-147">String</span><span class="sxs-lookup"><span data-stu-id="06985-147">String</span></span>|<span data-ttu-id="06985-148">この予定に関連付けられている顧客からのメモ。</span><span class="sxs-lookup"><span data-stu-id="06985-148">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="06985-149">ID でこの**bookingappointment**を読み取る場合にのみ、値を取得できます。</span><span class="sxs-lookup"><span data-stu-id="06985-149">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="06985-150">このプロパティは、最初に新しい顧客を使用して予定を作成するときにのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="06985-150">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="06985-151">その時点で、その値は**customerId**で表される顧客から計算されます。</span><span class="sxs-lookup"><span data-stu-id="06985-151">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="06985-152">顧客電話</span><span class="sxs-lookup"><span data-stu-id="06985-152">customerPhone</span></span>|<span data-ttu-id="06985-153">String</span><span class="sxs-lookup"><span data-stu-id="06985-153">String</span></span>|<span data-ttu-id="06985-154">お客様の電話番号。</span><span class="sxs-lookup"><span data-stu-id="06985-154">The customer's phone number.</span></span>|
|<span data-ttu-id="06985-155">duration</span><span class="sxs-lookup"><span data-stu-id="06985-155">duration</span></span>|<span data-ttu-id="06985-156">期間</span><span class="sxs-lookup"><span data-stu-id="06985-156">Duration</span></span>|<span data-ttu-id="06985-157">「文字形式」で示されて[](https://www.iso.org/iso-8601-date-and-time-format.html)いる予定の長さ。</span><span class="sxs-lookup"><span data-stu-id="06985-157">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="06985-158">end</span><span class="sxs-lookup"><span data-stu-id="06985-158">end</span></span>|[<span data-ttu-id="06985-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="06985-159">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="06985-160">予定が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="06985-160">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="06985-161">id</span><span class="sxs-lookup"><span data-stu-id="06985-161">id</span></span>|<span data-ttu-id="06985-162">String</span><span class="sxs-lookup"><span data-stu-id="06985-162">String</span></span>| <span data-ttu-id="06985-163">**bookingappointment**の ID。</span><span class="sxs-lookup"><span data-stu-id="06985-163">The ID of the **bookingAppointment**.</span></span> <span data-ttu-id="06985-164">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="06985-164">Read-only.</span></span>|
|<span data-ttu-id="06985-165">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="06985-165">invoiceAmount</span></span>|<span data-ttu-id="06985-166">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="06985-166">Double</span></span>|<span data-ttu-id="06985-167">請求書の請求金額。</span><span class="sxs-lookup"><span data-stu-id="06985-167">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="06985-168">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="06985-168">invoiceDate</span></span>|[<span data-ttu-id="06985-169">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="06985-169">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="06985-170">この予定の請求書の日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="06985-170">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="06985-171">invoiceId</span><span class="sxs-lookup"><span data-stu-id="06985-171">invoiceId</span></span>|<span data-ttu-id="06985-172">String</span><span class="sxs-lookup"><span data-stu-id="06985-172">String</span></span>|<span data-ttu-id="06985-173">請求書の ID。</span><span class="sxs-lookup"><span data-stu-id="06985-173">The ID of the invoice.</span></span>|
|<span data-ttu-id="06985-174">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="06985-174">invoiceStatus</span></span>|<span data-ttu-id="06985-175">string</span><span class="sxs-lookup"><span data-stu-id="06985-175">string</span></span>| <span data-ttu-id="06985-176">請求書の状態。</span><span class="sxs-lookup"><span data-stu-id="06985-176">The status of the invoice.</span></span> <span data-ttu-id="06985-177">可能な値は `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective` です。</span><span class="sxs-lookup"><span data-stu-id="06985-177">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="06985-178">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="06985-178">invoiceUrl</span></span>|<span data-ttu-id="06985-179">String</span><span class="sxs-lookup"><span data-stu-id="06985-179">String</span></span>|<span data-ttu-id="06985-180">Microsoft 予約の請求書の URL。</span><span class="sxs-lookup"><span data-stu-id="06985-180">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="06985-181">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="06985-181">optOutOfCustomerEmail</span></span>|<span data-ttu-id="06985-182">ブール値</span><span class="sxs-lookup"><span data-stu-id="06985-182">Boolean</span></span>|<span data-ttu-id="06985-183">True は、この予定の[bookingcustomer](bookingcustomer.md)が、この予定の確認を受信したくないことを示します。</span><span class="sxs-lookup"><span data-stu-id="06985-183">True indicates that the [bookingCustomer](bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="06985-184">postbuffer</span><span class="sxs-lookup"><span data-stu-id="06985-184">postBuffer</span></span>|<span data-ttu-id="06985-185">期間</span><span class="sxs-lookup"><span data-stu-id="06985-185">Duration</span></span>|<span data-ttu-id="06985-186">予定が終了した後に、クリーンアップのために確保する時間の長さを例として示します。</span><span class="sxs-lookup"><span data-stu-id="06985-186">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="06985-187">この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="06985-187">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="06985-188">prebuffer</span><span class="sxs-lookup"><span data-stu-id="06985-188">preBuffer</span></span>|<span data-ttu-id="06985-189">期間</span><span class="sxs-lookup"><span data-stu-id="06985-189">Duration</span></span>|<span data-ttu-id="06985-190">準備のために予定が開始されるまでの時間を例として示します。</span><span class="sxs-lookup"><span data-stu-id="06985-190">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="06985-191">この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="06985-191">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="06985-192">代金</span><span class="sxs-lookup"><span data-stu-id="06985-192">price</span></span>|<span data-ttu-id="06985-193">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="06985-193">Double</span></span>|<span data-ttu-id="06985-194">指定した[bookingservice](bookingservice.md)の予定に対する正規の価格。</span><span class="sxs-lookup"><span data-stu-id="06985-194">The regular price for an appointment for the specified [bookingService](bookingservice.md).</span></span>|
|<span data-ttu-id="06985-195">priceType</span><span class="sxs-lookup"><span data-stu-id="06985-195">priceType</span></span>|<span data-ttu-id="06985-196">string</span><span class="sxs-lookup"><span data-stu-id="06985-196">string</span></span>| <span data-ttu-id="06985-197">サービスの価格構造を柔軟に提供するための設定。</span><span class="sxs-lookup"><span data-stu-id="06985-197">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="06985-198">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="06985-198">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="06985-199">isp</span><span class="sxs-lookup"><span data-stu-id="06985-199">reminders</span></span>|<span data-ttu-id="06985-200">[bookingreminder](bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="06985-200">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="06985-201">この予定に対して送信された顧客のアラームのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="06985-201">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="06985-202">このプロパティの値は、この**bookingappointment**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="06985-202">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="06985-203">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="06985-203">selfServiceAppointmentId</span></span>|<span data-ttu-id="06985-204">String</span><span class="sxs-lookup"><span data-stu-id="06985-204">String</span></span>|<span data-ttu-id="06985-205">顧客に代わってスタッフメンバーではなく、顧客が [スケジュール] ページで直接作成された予定の場合は、予定の追加の追跡 ID。</span><span class="sxs-lookup"><span data-stu-id="06985-205">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="06985-206">serviceId</span><span class="sxs-lookup"><span data-stu-id="06985-206">serviceId</span></span>|<span data-ttu-id="06985-207">String</span><span class="sxs-lookup"><span data-stu-id="06985-207">String</span></span>|<span data-ttu-id="06985-208">この予定に関連付けられている[bookingservice](bookingservice.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="06985-208">The ID of the [bookingService](bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="06985-209">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="06985-209">serviceLocation</span></span>|[<span data-ttu-id="06985-210">location</span><span class="sxs-lookup"><span data-stu-id="06985-210">location</span></span>](location.md)|<span data-ttu-id="06985-211">サービスが配信される場所。</span><span class="sxs-lookup"><span data-stu-id="06985-211">The location where the service is delivered.</span></span>|
|<span data-ttu-id="06985-212">serviceName</span><span class="sxs-lookup"><span data-stu-id="06985-212">serviceName</span></span>|<span data-ttu-id="06985-213">String</span><span class="sxs-lookup"><span data-stu-id="06985-213">String</span></span>|<span data-ttu-id="06985-214">この予定に関連付けられている**bookingservice**の名前です。</span><span class="sxs-lookup"><span data-stu-id="06985-214">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="06985-215">新しい予定を作成するときは、このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="06985-215">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="06985-216">指定しない場合、 **serviceId**プロパティによって、予定に関連付けられているサービスから計算されます。</span><span class="sxs-lookup"><span data-stu-id="06985-216">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="06985-217">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="06985-217">serviceNotes</span></span>|<span data-ttu-id="06985-218">String</span><span class="sxs-lookup"><span data-stu-id="06985-218">String</span></span>|<span data-ttu-id="06985-219">[bookingStaffMember](bookingstaffmember.md)からのメモ。</span><span class="sxs-lookup"><span data-stu-id="06985-219">Notes from a [bookingStaffMember](bookingstaffmember.md).</span></span> <span data-ttu-id="06985-220">このプロパティの値は、この**bookingappointment**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="06985-220">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="06985-221">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="06985-221">staffMemberIds</span></span>|<span data-ttu-id="06985-222">String collection</span><span class="sxs-lookup"><span data-stu-id="06985-222">String collection</span></span>|<span data-ttu-id="06985-223">この予定でスケジュールされている各[bookingStaffMember](bookingstaffmember.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="06985-223">The ID of each [bookingStaffMember](bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="06985-224">start</span><span class="sxs-lookup"><span data-stu-id="06985-224">start</span></span>|[<span data-ttu-id="06985-225">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="06985-225">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="06985-226">予定が開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="06985-226">The date, time, and time zone that the appointment begins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06985-227">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06985-227">Relationships</span></span>
<span data-ttu-id="06985-228">なし</span><span class="sxs-lookup"><span data-stu-id="06985-228">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="06985-229">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06985-229">JSON representation</span></span>

<span data-ttu-id="06985-230">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06985-230">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingappointment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
