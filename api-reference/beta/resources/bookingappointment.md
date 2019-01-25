---
title: bookingAppointment リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c5868788159f0602c1f8a263138c7ce9107c2c94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509841"
---
# <a name="bookingappointment-resource-type"></a><span data-ttu-id="2cc98-104">bookingAppointment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2cc98-104">bookingAppointment resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="2cc98-105">[BookingService](bookingservice.md)Microsoft の予約ビジネスによって提供される、スタッフ メンバーのセットによって実行されるため、顧客の予定を表します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-105">Represents a customer appointment for a [bookingService](bookingservice.md), performed by a set of staff members, provided by a Microsoft Bookings business.</span></span>


## <a name="methods"></a><span data-ttu-id="2cc98-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2cc98-106">Methods</span></span>

| <span data-ttu-id="2cc98-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2cc98-107">Method</span></span>           | <span data-ttu-id="2cc98-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2cc98-108">Return Type</span></span>    |<span data-ttu-id="2cc98-109">説明</span><span class="sxs-lookup"><span data-stu-id="2cc98-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2cc98-110">リストの予定</span><span class="sxs-lookup"><span data-stu-id="2cc98-110">List appointments</span></span>](../api/bookingbusiness-list-appointments.md) |  <span data-ttu-id="2cc98-111">[bookingAppointment](bookingappointment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2cc98-111">[bookingAppointment](bookingappointment.md) collection</span></span> | <span data-ttu-id="2cc98-112">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingAppointment**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-112">Get a list of **bookingAppointment** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="2cc98-113">BookingAppointment を作成します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-113">Create bookingAppointment</span></span>](../api/bookingbusiness-post-appointments.md) |  [<span data-ttu-id="2cc98-114">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="2cc98-114">bookingAppointment</span></span>](bookingappointment.md) | <span data-ttu-id="2cc98-115">指定した[bookingbusiness](../resources/bookingbusiness.md)用の新しい**bookingAppointment**を作成します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-115">Create a new **bookingAppointment** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="2cc98-116">BookingAppointment を取得します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-116">Get bookingAppointment</span></span>](../api/bookingappointment-get.md) | [<span data-ttu-id="2cc98-117">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="2cc98-117">bookingAppointment</span></span>](bookingappointment.md) |<span data-ttu-id="2cc98-118">プロパティと**bookingAppointment**オブジェクトの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cc98-118">Read the properties and relationships of **bookingAppointment** object.</span></span>|
|[<span data-ttu-id="2cc98-119">Update</span><span class="sxs-lookup"><span data-stu-id="2cc98-119">Update</span></span>](../api/bookingappointment-update.md) | [<span data-ttu-id="2cc98-120">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="2cc98-120">bookingAppointment</span></span>](bookingappointment.md)    |<span data-ttu-id="2cc98-121">**BookingAppointment**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-121">Update a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="2cc98-122">Delete</span><span class="sxs-lookup"><span data-stu-id="2cc98-122">Delete</span></span>](../api/bookingappointment-delete.md) | <span data-ttu-id="2cc98-123">なし</span><span class="sxs-lookup"><span data-stu-id="2cc98-123">None</span></span> |<span data-ttu-id="2cc98-124">**BookingAppointment**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-124">Delete a **bookingAppointment** object.</span></span> |
|[<span data-ttu-id="2cc98-125">Cancel</span><span class="sxs-lookup"><span data-stu-id="2cc98-125">Cancel</span></span>](../api/bookingappointment-cancel.md)|<span data-ttu-id="2cc98-126">なし</span><span class="sxs-lookup"><span data-stu-id="2cc98-126">None</span></span>| <span data-ttu-id="2cc98-127">**BookingAppointment**オブジェクトをキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="2cc98-127">Cancel a **bookingAppointment** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2cc98-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cc98-128">Properties</span></span>
| <span data-ttu-id="2cc98-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cc98-129">Property</span></span>     | <span data-ttu-id="2cc98-130">型</span><span class="sxs-lookup"><span data-stu-id="2cc98-130">Type</span></span>   |<span data-ttu-id="2cc98-131">説明</span><span class="sxs-lookup"><span data-stu-id="2cc98-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cc98-132">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2cc98-132">customerEmailAddress</span></span>|<span data-ttu-id="2cc98-133">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-133">String</span></span>|<span data-ttu-id="2cc98-134">予定を予約する、 [bookingCustomer](bookingcustomer.md)の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="2cc98-134">The SMTP address of the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="2cc98-135">customerId</span><span class="sxs-lookup"><span data-stu-id="2cc98-135">customerId</span></span>|<span data-ttu-id="2cc98-136">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-136">String</span></span>|<span data-ttu-id="2cc98-137">この予定の[bookingCustomer](bookingcustomer.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-137">The ID of the [bookingCustomer](bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="2cc98-138">ID が指定されていない場合、予定を作成するとき、新しい**bookingCustomer**オブジェクトが作成されます。</span><span class="sxs-lookup"><span data-stu-id="2cc98-138">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="2cc98-139">1 回に設定する必要があります **[得意先コード]** 不変です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-139">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="2cc98-140">customerLocation</span><span class="sxs-lookup"><span data-stu-id="2cc98-140">customerLocation</span></span>|[<span data-ttu-id="2cc98-141">location</span><span class="sxs-lookup"><span data-stu-id="2cc98-141">location</span></span>](location.md)|<span data-ttu-id="2cc98-142">予定を予約する、 [bookingCustomer](bookingcustomer.md)の場所の情報を表します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-142">Represents location information for the [bookingCustomer](bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="2cc98-143">様</span><span class="sxs-lookup"><span data-stu-id="2cc98-143">customerName</span></span>|<span data-ttu-id="2cc98-144">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-144">String</span></span>|<span data-ttu-id="2cc98-145">お客様の名前です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-145">The customer's name.</span></span>|
|<span data-ttu-id="2cc98-146">customerNotes</span><span class="sxs-lookup"><span data-stu-id="2cc98-146">customerNotes</span></span>|<span data-ttu-id="2cc98-147">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-147">String</span></span>|<span data-ttu-id="2cc98-148">この予定に関連付けられている顧客からのノート。</span><span class="sxs-lookup"><span data-stu-id="2cc98-148">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="2cc98-149">その ID ではこの**bookingAppointment**を表示する場合のみ値を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="2cc98-149">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="2cc98-150">最初に顧客との新しい予定を作成する場合にのみ、このプロパティを設定することができます。</span><span class="sxs-lookup"><span data-stu-id="2cc98-150">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="2cc98-151">その後も、 **[得意先コード]** で表される顧客からの値が計算されます。</span><span class="sxs-lookup"><span data-stu-id="2cc98-151">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="2cc98-152">customerPhone</span><span class="sxs-lookup"><span data-stu-id="2cc98-152">customerPhone</span></span>|<span data-ttu-id="2cc98-153">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-153">String</span></span>|<span data-ttu-id="2cc98-154">お客様の電話番号です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-154">The customer's phone number.</span></span>|
|<span data-ttu-id="2cc98-155">duration</span><span class="sxs-lookup"><span data-stu-id="2cc98-155">duration</span></span>|<span data-ttu-id="2cc98-156">Duration</span><span class="sxs-lookup"><span data-stu-id="2cc98-156">Duration</span></span>|<span data-ttu-id="2cc98-157">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、予定の長さです。</span><span class="sxs-lookup"><span data-stu-id="2cc98-157">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="2cc98-158">end</span><span class="sxs-lookup"><span data-stu-id="2cc98-158">end</span></span>|[<span data-ttu-id="2cc98-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2cc98-159">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2cc98-160">日付、時刻、およびタイム ゾーンの予定を終了します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-160">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="2cc98-161">id</span><span class="sxs-lookup"><span data-stu-id="2cc98-161">id</span></span>|<span data-ttu-id="2cc98-162">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-162">String</span></span>| <span data-ttu-id="2cc98-163">**BookingAppointment**の ID です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-163">The ID of the **bookingAppointment**.</span></span> <span data-ttu-id="2cc98-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-164">Read-only.</span></span>|
|<span data-ttu-id="2cc98-165">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="2cc98-165">invoiceAmount</span></span>|<span data-ttu-id="2cc98-166">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="2cc98-166">Double</span></span>|<span data-ttu-id="2cc98-167">請求書の請求金額です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-167">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="2cc98-168">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="2cc98-168">invoiceDate</span></span>|[<span data-ttu-id="2cc98-169">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2cc98-169">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2cc98-170">日付、時刻、および請求書のこの予定のタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="2cc98-170">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="2cc98-171">invoiceId</span><span class="sxs-lookup"><span data-stu-id="2cc98-171">invoiceId</span></span>|<span data-ttu-id="2cc98-172">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-172">String</span></span>|<span data-ttu-id="2cc98-173">請求書の ID。</span><span class="sxs-lookup"><span data-stu-id="2cc98-173">The ID of the invoice.</span></span>|
|<span data-ttu-id="2cc98-174">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="2cc98-174">invoiceStatus</span></span>|<span data-ttu-id="2cc98-175">string</span><span class="sxs-lookup"><span data-stu-id="2cc98-175">string</span></span>| <span data-ttu-id="2cc98-176">請求書の状態です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-176">The status of the invoice.</span></span> <span data-ttu-id="2cc98-177">使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="2cc98-177">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="2cc98-178">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="2cc98-178">invoiceUrl</span></span>|<span data-ttu-id="2cc98-179">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-179">String</span></span>|<span data-ttu-id="2cc98-180">Microsoft の予約で請求書の URL です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-180">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="2cc98-181">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="2cc98-181">optOutOfCustomerEmail</span></span>|<span data-ttu-id="2cc98-182">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cc98-182">Boolean</span></span>|<span data-ttu-id="2cc98-183">True は、この予定の[bookingCustomer](bookingcustomer.md)は、この予定の確認メッセージを表示するのには望んでいないことを示します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-183">True indicates that the [bookingCustomer](bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="2cc98-184">事後バッファリング</span><span class="sxs-lookup"><span data-stu-id="2cc98-184">postBuffer</span></span>|<span data-ttu-id="2cc98-185">Duration</span><span class="sxs-lookup"><span data-stu-id="2cc98-185">Duration</span></span>|<span data-ttu-id="2cc98-186">クリーンアップ、例として、予定が終了した後に予約する時間の量。</span><span class="sxs-lookup"><span data-stu-id="2cc98-186">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="2cc98-187">値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="2cc98-187">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="2cc98-188">事前バッファリング</span><span class="sxs-lookup"><span data-stu-id="2cc98-188">preBuffer</span></span>|<span data-ttu-id="2cc98-189">Duration</span><span class="sxs-lookup"><span data-stu-id="2cc98-189">Duration</span></span>|<span data-ttu-id="2cc98-190">例として、準備のため、予定の開始前に予約する時間の量。</span><span class="sxs-lookup"><span data-stu-id="2cc98-190">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="2cc98-191">値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="2cc98-191">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="2cc98-192">Price</span><span class="sxs-lookup"><span data-stu-id="2cc98-192">price</span></span>|<span data-ttu-id="2cc98-193">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="2cc98-193">Double</span></span>|<span data-ttu-id="2cc98-194">指定された[bookingService](bookingservice.md)の予定の正規の価格です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-194">The regular price for an appointment for the specified [bookingService](bookingservice.md).</span></span>|
|<span data-ttu-id="2cc98-195">priceType</span><span class="sxs-lookup"><span data-stu-id="2cc98-195">priceType</span></span>|<span data-ttu-id="2cc98-196">string</span><span class="sxs-lookup"><span data-stu-id="2cc98-196">string</span></span>| <span data-ttu-id="2cc98-197">サービスの価格設定構造の柔軟性を提供するように設定します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-197">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="2cc98-198">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-198">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="2cc98-199">Reminders</span><span class="sxs-lookup"><span data-stu-id="2cc98-199">reminders</span></span>|<span data-ttu-id="2cc98-200">[bookingReminder](bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2cc98-200">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="2cc98-201">この予定に送信される顧客の事前通知のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2cc98-201">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="2cc98-202">その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="2cc98-202">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="2cc98-203">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="2cc98-203">selfServiceAppointmentId</span></span>|<span data-ttu-id="2cc98-204">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-204">String</span></span>|<span data-ttu-id="2cc98-205">予定が作成された場合 [スケジュール] ページで、お客様が直接にではなく、お客様の代わりにスタッフのメンバーでは、予定の他の追跡 ID。</span><span class="sxs-lookup"><span data-stu-id="2cc98-205">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="2cc98-206">serviceId</span><span class="sxs-lookup"><span data-stu-id="2cc98-206">serviceId</span></span>|<span data-ttu-id="2cc98-207">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-207">String</span></span>|<span data-ttu-id="2cc98-208">[BookingService](bookingservice.md)の ID は、この予定に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="2cc98-208">The ID of the [bookingService](bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="2cc98-209">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="2cc98-209">serviceLocation</span></span>|[<span data-ttu-id="2cc98-210">location</span><span class="sxs-lookup"><span data-stu-id="2cc98-210">location</span></span>](location.md)|<span data-ttu-id="2cc98-211">サービスの配信場所です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-211">The location where the service is delivered.</span></span>|
|<span data-ttu-id="2cc98-212">serviceName</span><span class="sxs-lookup"><span data-stu-id="2cc98-212">serviceName</span></span>|<span data-ttu-id="2cc98-213">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-213">String</span></span>|<span data-ttu-id="2cc98-214">**BookingService**の名前は、この予定に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="2cc98-214">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="2cc98-215">新しい予定を作成するとき、このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-215">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="2cc98-216">指定されていない場合は、 **serviceId**プロパティにより、予定に関連付けられたサービスから計算されます。</span><span class="sxs-lookup"><span data-stu-id="2cc98-216">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="2cc98-217">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="2cc98-217">serviceNotes</span></span>|<span data-ttu-id="2cc98-218">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-218">String</span></span>|<span data-ttu-id="2cc98-219">の[bookingStaffMember](bookingstaffmember.md)からのノート。</span><span class="sxs-lookup"><span data-stu-id="2cc98-219">Notes from a [bookingStaffMember](bookingstaffmember.md).</span></span> <span data-ttu-id="2cc98-220">その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="2cc98-220">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="2cc98-221">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="2cc98-221">staffMemberIds</span></span>|<span data-ttu-id="2cc98-222">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2cc98-222">String collection</span></span>|<span data-ttu-id="2cc98-223">この予定にスケジュールされている各[bookingStaffMember](bookingstaffmember.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="2cc98-223">The ID of each [bookingStaffMember](bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="2cc98-224">start</span><span class="sxs-lookup"><span data-stu-id="2cc98-224">start</span></span>|[<span data-ttu-id="2cc98-225">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2cc98-225">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2cc98-226">日付、時刻、およびタイム ゾーンの予定の開始をします。</span><span class="sxs-lookup"><span data-stu-id="2cc98-226">The date, time, and time zone that the appointment begins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cc98-227">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2cc98-227">Relationships</span></span>
<span data-ttu-id="2cc98-228">なし</span><span class="sxs-lookup"><span data-stu-id="2cc98-228">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2cc98-229">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cc98-229">JSON representation</span></span>

<span data-ttu-id="2cc98-230">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2cc98-230">The following is a JSON representation of the resource.</span></span>

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
