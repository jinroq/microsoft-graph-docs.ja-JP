---
title: Bookingappointment を更新します。
description: 指定された bookingbusiness で、bookingAppointment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cde8a309e3544f5ed5cdf84f7c50d33e95084526
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529237"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="bb7e1-103">Bookingappointment を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb7e1-104">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 [bookingAppointment](../resources/bookingappointment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bb7e1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb7e1-105">Permissions</span></span>
<span data-ttu-id="bb7e1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb7e1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb7e1-108">Permission type</span></span>      | <span data-ttu-id="bb7e1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb7e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb7e1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb7e1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="bb7e1-111">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="bb7e1-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bb7e1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb7e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb7e1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-113">Not supported.</span></span>   |
|<span data-ttu-id="bb7e1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb7e1-114">Application</span></span> | <span data-ttu-id="bb7e1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bb7e1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb7e1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="bb7e1-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb7e1-117">Optional request headers</span></span>
| <span data-ttu-id="bb7e1-118">名前</span><span class="sxs-lookup"><span data-stu-id="bb7e1-118">Name</span></span>       | <span data-ttu-id="bb7e1-119">説明</span><span class="sxs-lookup"><span data-stu-id="bb7e1-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bb7e1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb7e1-120">Authorization</span></span>  | <span data-ttu-id="bb7e1-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bb7e1-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb7e1-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb7e1-122">Request body</span></span>
<span data-ttu-id="bb7e1-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bb7e1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb7e1-126">Property</span></span>     | <span data-ttu-id="bb7e1-127">型</span><span class="sxs-lookup"><span data-stu-id="bb7e1-127">Type</span></span>   |<span data-ttu-id="bb7e1-128">説明</span><span class="sxs-lookup"><span data-stu-id="bb7e1-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb7e1-129">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bb7e1-129">customerEmailAddress</span></span>|<span data-ttu-id="bb7e1-130">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-130">String</span></span>|<span data-ttu-id="bb7e1-131">予定を予約する、 [bookingCustomer](../resources/bookingcustomer.md)の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="bb7e1-132">customerId</span><span class="sxs-lookup"><span data-stu-id="bb7e1-132">customerId</span></span>|<span data-ttu-id="bb7e1-133">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-133">String</span></span>|<span data-ttu-id="bb7e1-134">この予定の[bookingCustomer](../resources/bookingcustomer.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="bb7e1-135">ID が指定されていない場合、予定を作成するとき、新しい**bookingCustomer**オブジェクトが作成されます。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="bb7e1-136">1 回に設定する必要があります **[得意先コード]** 不変です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="bb7e1-137">customerLocation</span><span class="sxs-lookup"><span data-stu-id="bb7e1-137">customerLocation</span></span>|[<span data-ttu-id="bb7e1-138">location</span><span class="sxs-lookup"><span data-stu-id="bb7e1-138">location</span></span>](../resources/location.md)|<span data-ttu-id="bb7e1-139">予定を予約する、 [bookingCustomer](../resources/bookingcustomer.md)の場所の情報を表します。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="bb7e1-140">様</span><span class="sxs-lookup"><span data-stu-id="bb7e1-140">customerName</span></span>|<span data-ttu-id="bb7e1-141">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-141">String</span></span>|<span data-ttu-id="bb7e1-142">お客様の名前です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-142">The customer's name.</span></span>|
|<span data-ttu-id="bb7e1-143">customerNotes</span><span class="sxs-lookup"><span data-stu-id="bb7e1-143">customerNotes</span></span>|<span data-ttu-id="bb7e1-144">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-144">String</span></span>|<span data-ttu-id="bb7e1-145">この予定に関連付けられている顧客からのノート。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="bb7e1-146">その ID ではこの**bookingAppointment**を表示する場合のみ値を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="bb7e1-147">最初に顧客との新しい予定を作成する場合にのみ、このプロパティを設定することができます。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="bb7e1-148">その後も、 **[得意先コード]** で表される顧客からの値が計算されます。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="bb7e1-149">customerPhone</span><span class="sxs-lookup"><span data-stu-id="bb7e1-149">customerPhone</span></span>|<span data-ttu-id="bb7e1-150">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-150">String</span></span>|<span data-ttu-id="bb7e1-151">お客様の電話番号です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-151">The customer's phone number.</span></span>|
|<span data-ttu-id="bb7e1-152">duration</span><span class="sxs-lookup"><span data-stu-id="bb7e1-152">duration</span></span>|<span data-ttu-id="bb7e1-153">Duration</span><span class="sxs-lookup"><span data-stu-id="bb7e1-153">Duration</span></span>|<span data-ttu-id="bb7e1-154">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、予定の長さです。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="bb7e1-155">end</span><span class="sxs-lookup"><span data-stu-id="bb7e1-155">end</span></span>|[<span data-ttu-id="bb7e1-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bb7e1-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bb7e1-157">日付、時刻、およびタイム ゾーンの予定を終了します。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="bb7e1-158">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="bb7e1-158">invoiceAmount</span></span>|<span data-ttu-id="bb7e1-159">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="bb7e1-159">Double</span></span>|<span data-ttu-id="bb7e1-160">請求書の請求金額です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="bb7e1-161">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="bb7e1-161">invoiceDate</span></span>|[<span data-ttu-id="bb7e1-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bb7e1-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bb7e1-163">日付、時刻、および請求書のこの予定のタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="bb7e1-164">invoiceId</span><span class="sxs-lookup"><span data-stu-id="bb7e1-164">invoiceId</span></span>|<span data-ttu-id="bb7e1-165">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-165">String</span></span>|<span data-ttu-id="bb7e1-166">請求書の ID。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="bb7e1-167">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="bb7e1-167">invoiceStatus</span></span>|<span data-ttu-id="bb7e1-168">string</span><span class="sxs-lookup"><span data-stu-id="bb7e1-168">string</span></span>| <span data-ttu-id="bb7e1-169">請求書の状態です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-169">The status of the invoice.</span></span> <span data-ttu-id="bb7e1-170">使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="bb7e1-171">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="bb7e1-171">invoiceUrl</span></span>|<span data-ttu-id="bb7e1-172">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-172">String</span></span>|<span data-ttu-id="bb7e1-173">Microsoft の予約で請求書の URL です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="bb7e1-174">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="bb7e1-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="bb7e1-175">ブール値</span><span class="sxs-lookup"><span data-stu-id="bb7e1-175">Boolean</span></span>|<span data-ttu-id="bb7e1-176">True は、この予定の[bookingCustomer](../resources/bookingcustomer.md)は、この予定の確認メッセージを表示するのには望んでいないことを示します。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="bb7e1-177">事後バッファリング</span><span class="sxs-lookup"><span data-stu-id="bb7e1-177">postBuffer</span></span>|<span data-ttu-id="bb7e1-178">Duration</span><span class="sxs-lookup"><span data-stu-id="bb7e1-178">Duration</span></span>|<span data-ttu-id="bb7e1-179">クリーンアップ、例として、予定が終了した後に予約する時間の量。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="bb7e1-180">値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="bb7e1-181">事前バッファリング</span><span class="sxs-lookup"><span data-stu-id="bb7e1-181">preBuffer</span></span>|<span data-ttu-id="bb7e1-182">Duration</span><span class="sxs-lookup"><span data-stu-id="bb7e1-182">Duration</span></span>|<span data-ttu-id="bb7e1-183">例として、準備のため、予定の開始前に予約する時間の量。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="bb7e1-184">値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="bb7e1-185">Price</span><span class="sxs-lookup"><span data-stu-id="bb7e1-185">price</span></span>|<span data-ttu-id="bb7e1-186">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="bb7e1-186">Double</span></span>|<span data-ttu-id="bb7e1-187">指定された[bookingService](../resources/bookingservice.md)の予定の正規の価格です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="bb7e1-188">priceType</span><span class="sxs-lookup"><span data-stu-id="bb7e1-188">priceType</span></span>|<span data-ttu-id="bb7e1-189">string</span><span class="sxs-lookup"><span data-stu-id="bb7e1-189">string</span></span>| <span data-ttu-id="bb7e1-190">サービスの価格設定構造の柔軟性を提供するように設定します。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="bb7e1-191">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="bb7e1-192">Reminders</span><span class="sxs-lookup"><span data-stu-id="bb7e1-192">reminders</span></span>|<span data-ttu-id="bb7e1-193">[bookingReminder](../resources/bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb7e1-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="bb7e1-194">この予定に送信される顧客の事前通知のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="bb7e1-195">その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="bb7e1-196">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="bb7e1-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="bb7e1-197">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-197">String</span></span>|<span data-ttu-id="bb7e1-198">予定が作成された場合 [スケジュール] ページで、お客様が直接にではなく、お客様の代わりにスタッフのメンバーでは、予定の他の追跡 ID。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="bb7e1-199">serviceId</span><span class="sxs-lookup"><span data-stu-id="bb7e1-199">serviceId</span></span>|<span data-ttu-id="bb7e1-200">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-200">String</span></span>|<span data-ttu-id="bb7e1-201">[BookingService](../resources/bookingservice.md)の ID は、この予定に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="bb7e1-202">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="bb7e1-202">serviceLocation</span></span>|[<span data-ttu-id="bb7e1-203">location</span><span class="sxs-lookup"><span data-stu-id="bb7e1-203">location</span></span>](../resources/location.md)|<span data-ttu-id="bb7e1-204">サービスの配信場所です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="bb7e1-205">serviceName</span><span class="sxs-lookup"><span data-stu-id="bb7e1-205">serviceName</span></span>|<span data-ttu-id="bb7e1-206">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-206">String</span></span>|<span data-ttu-id="bb7e1-207">**BookingService**の名前は、この予定に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="bb7e1-208">新しい予定を作成するとき、このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="bb7e1-209">指定されていない場合は、 **serviceId**プロパティにより、予定に関連付けられたサービスから計算されます。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="bb7e1-210">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="bb7e1-210">serviceNotes</span></span>|<span data-ttu-id="bb7e1-211">String</span><span class="sxs-lookup"><span data-stu-id="bb7e1-211">String</span></span>|<span data-ttu-id="bb7e1-212">の[bookingStaffMember](../resources/bookingstaffmember.md)からのノート。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="bb7e1-213">その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="bb7e1-214">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="bb7e1-214">staffMemberIds</span></span>|<span data-ttu-id="bb7e1-215">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bb7e1-215">String collection</span></span>|<span data-ttu-id="bb7e1-216">この予定にスケジュールされている各[bookingStaffMember](../resources/bookingstaffmember.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="bb7e1-217">start</span><span class="sxs-lookup"><span data-stu-id="bb7e1-217">start</span></span>|[<span data-ttu-id="bb7e1-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bb7e1-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="bb7e1-219">日付、時刻、およびタイム ゾーンの予定の開始をします。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="bb7e1-220">応答</span><span class="sxs-lookup"><span data-stu-id="bb7e1-220">Response</span></span>
<span data-ttu-id="bb7e1-p113">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb7e1-223">例</span><span class="sxs-lookup"><span data-stu-id="bb7e1-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb7e1-224">要求</span><span class="sxs-lookup"><span data-stu-id="bb7e1-224">Request</span></span>
<span data-ttu-id="bb7e1-225">次の例では、サービスが、1 日の日付を変更し、請求書の日付を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
##### <a name="response"></a><span data-ttu-id="bb7e1-226">応答</span><span class="sxs-lookup"><span data-stu-id="bb7e1-226">Response</span></span>
<span data-ttu-id="bb7e1-227">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bb7e1-227">The following is an example of the response.</span></span>
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
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
