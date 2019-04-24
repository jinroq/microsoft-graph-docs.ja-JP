---
title: bookingappointment の更新
description: 指定した bookingappointment の bookingappointment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cde8a309e3544f5ed5cdf84f7c50d33e95084526
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462425"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="1a139-103">bookingappointment の更新</span><span class="sxs-lookup"><span data-stu-id="1a139-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a139-104">指定した[bookingappointment](../resources/bookingbusiness.md)の[bookingappointment](../resources/bookingappointment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a139-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1a139-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a139-105">Permissions</span></span>
<span data-ttu-id="1a139-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a139-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a139-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a139-108">Permission type</span></span>      | <span data-ttu-id="1a139-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a139-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a139-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a139-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1a139-111">bookingsappointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="1a139-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1a139-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a139-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a139-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a139-113">Not supported.</span></span>   |
|<span data-ttu-id="1a139-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a139-114">Application</span></span> | <span data-ttu-id="1a139-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a139-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1a139-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a139-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1a139-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a139-117">Optional request headers</span></span>
| <span data-ttu-id="1a139-118">名前</span><span class="sxs-lookup"><span data-stu-id="1a139-118">Name</span></span>       | <span data-ttu-id="1a139-119">説明</span><span class="sxs-lookup"><span data-stu-id="1a139-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1a139-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a139-120">Authorization</span></span>  | <span data-ttu-id="1a139-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1a139-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a139-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a139-122">Request body</span></span>
<span data-ttu-id="1a139-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1a139-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1a139-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a139-126">Property</span></span>     | <span data-ttu-id="1a139-127">型</span><span class="sxs-lookup"><span data-stu-id="1a139-127">Type</span></span>   |<span data-ttu-id="1a139-128">説明</span><span class="sxs-lookup"><span data-stu-id="1a139-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a139-129">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1a139-129">customerEmailAddress</span></span>|<span data-ttu-id="1a139-130">String</span><span class="sxs-lookup"><span data-stu-id="1a139-130">String</span></span>|<span data-ttu-id="1a139-131">予定を予約している[bookingcustomer](../resources/bookingcustomer.md)の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="1a139-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="1a139-132">id</span><span class="sxs-lookup"><span data-stu-id="1a139-132">customerId</span></span>|<span data-ttu-id="1a139-133">String</span><span class="sxs-lookup"><span data-stu-id="1a139-133">String</span></span>|<span data-ttu-id="1a139-134">この予定の[bookingcustomer](../resources/bookingcustomer.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="1a139-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="1a139-135">予定の作成時に ID が指定されていない場合は、新しい**bookingcustomer**オブジェクトが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1a139-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="1a139-136">設定すると、 **customerId**を不変にすることを考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a139-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="1a139-137">顧客の所在地</span><span class="sxs-lookup"><span data-stu-id="1a139-137">customerLocation</span></span>|[<span data-ttu-id="1a139-138">location</span><span class="sxs-lookup"><span data-stu-id="1a139-138">location</span></span>](../resources/location.md)|<span data-ttu-id="1a139-139">予定を予約している[bookingcustomer](../resources/bookingcustomer.md)の場所情報を表します。</span><span class="sxs-lookup"><span data-stu-id="1a139-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="1a139-140">おける</span><span class="sxs-lookup"><span data-stu-id="1a139-140">customerName</span></span>|<span data-ttu-id="1a139-141">String</span><span class="sxs-lookup"><span data-stu-id="1a139-141">String</span></span>|<span data-ttu-id="1a139-142">顧客の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a139-142">The customer's name.</span></span>|
|<span data-ttu-id="1a139-143">顧客メモ</span><span class="sxs-lookup"><span data-stu-id="1a139-143">customerNotes</span></span>|<span data-ttu-id="1a139-144">String</span><span class="sxs-lookup"><span data-stu-id="1a139-144">String</span></span>|<span data-ttu-id="1a139-145">この予定に関連付けられている顧客からのメモ。</span><span class="sxs-lookup"><span data-stu-id="1a139-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="1a139-146">ID でこの**bookingappointment**を読み取る場合にのみ、値を取得できます。</span><span class="sxs-lookup"><span data-stu-id="1a139-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="1a139-147">このプロパティは、最初に新しい顧客を使用して予定を作成するときにのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="1a139-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="1a139-148">その時点で、その値は**customerId**で表される顧客から計算されます。</span><span class="sxs-lookup"><span data-stu-id="1a139-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="1a139-149">顧客電話</span><span class="sxs-lookup"><span data-stu-id="1a139-149">customerPhone</span></span>|<span data-ttu-id="1a139-150">String</span><span class="sxs-lookup"><span data-stu-id="1a139-150">String</span></span>|<span data-ttu-id="1a139-151">お客様の電話番号。</span><span class="sxs-lookup"><span data-stu-id="1a139-151">The customer's phone number.</span></span>|
|<span data-ttu-id="1a139-152">duration</span><span class="sxs-lookup"><span data-stu-id="1a139-152">duration</span></span>|<span data-ttu-id="1a139-153">期間</span><span class="sxs-lookup"><span data-stu-id="1a139-153">Duration</span></span>|<span data-ttu-id="1a139-154">「文字形式」で示されて[](https://www.iso.org/iso-8601-date-and-time-format.html)いる予定の長さ。</span><span class="sxs-lookup"><span data-stu-id="1a139-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="1a139-155">end</span><span class="sxs-lookup"><span data-stu-id="1a139-155">end</span></span>|[<span data-ttu-id="1a139-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1a139-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1a139-157">予定が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="1a139-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="1a139-158">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="1a139-158">invoiceAmount</span></span>|<span data-ttu-id="1a139-159">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="1a139-159">Double</span></span>|<span data-ttu-id="1a139-160">請求書の請求金額。</span><span class="sxs-lookup"><span data-stu-id="1a139-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="1a139-161">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="1a139-161">invoiceDate</span></span>|[<span data-ttu-id="1a139-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1a139-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1a139-163">この予定の請求書の日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="1a139-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="1a139-164">invoiceId</span><span class="sxs-lookup"><span data-stu-id="1a139-164">invoiceId</span></span>|<span data-ttu-id="1a139-165">String</span><span class="sxs-lookup"><span data-stu-id="1a139-165">String</span></span>|<span data-ttu-id="1a139-166">請求書の ID。</span><span class="sxs-lookup"><span data-stu-id="1a139-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="1a139-167">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="1a139-167">invoiceStatus</span></span>|<span data-ttu-id="1a139-168">string</span><span class="sxs-lookup"><span data-stu-id="1a139-168">string</span></span>| <span data-ttu-id="1a139-169">請求書の状態。</span><span class="sxs-lookup"><span data-stu-id="1a139-169">The status of the invoice.</span></span> <span data-ttu-id="1a139-170">可能な値は `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective` です。</span><span class="sxs-lookup"><span data-stu-id="1a139-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="1a139-171">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="1a139-171">invoiceUrl</span></span>|<span data-ttu-id="1a139-172">String</span><span class="sxs-lookup"><span data-stu-id="1a139-172">String</span></span>|<span data-ttu-id="1a139-173">Microsoft 予約の請求書の URL。</span><span class="sxs-lookup"><span data-stu-id="1a139-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="1a139-174">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="1a139-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="1a139-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a139-175">Boolean</span></span>|<span data-ttu-id="1a139-176">True は、この予定の[bookingcustomer](../resources/bookingcustomer.md)が、この予定の確認を受信したくないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1a139-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="1a139-177">postbuffer</span><span class="sxs-lookup"><span data-stu-id="1a139-177">postBuffer</span></span>|<span data-ttu-id="1a139-178">期間</span><span class="sxs-lookup"><span data-stu-id="1a139-178">Duration</span></span>|<span data-ttu-id="1a139-179">予定が終了した後に、クリーンアップのために確保する時間の長さを例として示します。</span><span class="sxs-lookup"><span data-stu-id="1a139-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="1a139-180">この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="1a139-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="1a139-181">prebuffer</span><span class="sxs-lookup"><span data-stu-id="1a139-181">preBuffer</span></span>|<span data-ttu-id="1a139-182">期間</span><span class="sxs-lookup"><span data-stu-id="1a139-182">Duration</span></span>|<span data-ttu-id="1a139-183">準備のために予定が開始されるまでの時間を例として示します。</span><span class="sxs-lookup"><span data-stu-id="1a139-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="1a139-184">この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="1a139-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="1a139-185">代金</span><span class="sxs-lookup"><span data-stu-id="1a139-185">price</span></span>|<span data-ttu-id="1a139-186">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="1a139-186">Double</span></span>|<span data-ttu-id="1a139-187">指定した[bookingservice](../resources/bookingservice.md)の予定に対する正規の価格。</span><span class="sxs-lookup"><span data-stu-id="1a139-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="1a139-188">priceType</span><span class="sxs-lookup"><span data-stu-id="1a139-188">priceType</span></span>|<span data-ttu-id="1a139-189">string</span><span class="sxs-lookup"><span data-stu-id="1a139-189">string</span></span>| <span data-ttu-id="1a139-190">サービスの価格構造を柔軟に提供するための設定。</span><span class="sxs-lookup"><span data-stu-id="1a139-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="1a139-191">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="1a139-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="1a139-192">isp</span><span class="sxs-lookup"><span data-stu-id="1a139-192">reminders</span></span>|<span data-ttu-id="1a139-193">[bookingreminder](../resources/bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a139-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="1a139-194">この予定に対して送信された顧客のアラームのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1a139-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="1a139-195">このプロパティの値は、この**bookingappointment**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1a139-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="1a139-196">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="1a139-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="1a139-197">String</span><span class="sxs-lookup"><span data-stu-id="1a139-197">String</span></span>|<span data-ttu-id="1a139-198">顧客に代わってスタッフメンバーではなく、顧客が [スケジュール] ページで直接作成された予定の場合は、予定の追加の追跡 ID。</span><span class="sxs-lookup"><span data-stu-id="1a139-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="1a139-199">serviceId</span><span class="sxs-lookup"><span data-stu-id="1a139-199">serviceId</span></span>|<span data-ttu-id="1a139-200">String</span><span class="sxs-lookup"><span data-stu-id="1a139-200">String</span></span>|<span data-ttu-id="1a139-201">この予定に関連付けられている[bookingservice](../resources/bookingservice.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="1a139-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="1a139-202">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="1a139-202">serviceLocation</span></span>|[<span data-ttu-id="1a139-203">location</span><span class="sxs-lookup"><span data-stu-id="1a139-203">location</span></span>](../resources/location.md)|<span data-ttu-id="1a139-204">サービスが配信される場所。</span><span class="sxs-lookup"><span data-stu-id="1a139-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="1a139-205">serviceName</span><span class="sxs-lookup"><span data-stu-id="1a139-205">serviceName</span></span>|<span data-ttu-id="1a139-206">String</span><span class="sxs-lookup"><span data-stu-id="1a139-206">String</span></span>|<span data-ttu-id="1a139-207">この予定に関連付けられている**bookingservice**の名前です。</span><span class="sxs-lookup"><span data-stu-id="1a139-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="1a139-208">新しい予定を作成するときは、このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="1a139-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="1a139-209">指定しない場合、 **serviceId**プロパティによって、予定に関連付けられているサービスから計算されます。</span><span class="sxs-lookup"><span data-stu-id="1a139-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="1a139-210">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="1a139-210">serviceNotes</span></span>|<span data-ttu-id="1a139-211">String</span><span class="sxs-lookup"><span data-stu-id="1a139-211">String</span></span>|<span data-ttu-id="1a139-212">[bookingStaffMember](../resources/bookingstaffmember.md)からのメモ。</span><span class="sxs-lookup"><span data-stu-id="1a139-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="1a139-213">このプロパティの値は、この**bookingappointment**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1a139-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="1a139-214">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="1a139-214">staffMemberIds</span></span>|<span data-ttu-id="1a139-215">String collection</span><span class="sxs-lookup"><span data-stu-id="1a139-215">String collection</span></span>|<span data-ttu-id="1a139-216">この予定でスケジュールされている各[bookingStaffMember](../resources/bookingstaffmember.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="1a139-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="1a139-217">start</span><span class="sxs-lookup"><span data-stu-id="1a139-217">start</span></span>|[<span data-ttu-id="1a139-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1a139-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1a139-219">予定が開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="1a139-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="1a139-220">応答</span><span class="sxs-lookup"><span data-stu-id="1a139-220">Response</span></span>
<span data-ttu-id="1a139-p113">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1a139-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a139-223">例</span><span class="sxs-lookup"><span data-stu-id="1a139-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a139-224">要求</span><span class="sxs-lookup"><span data-stu-id="1a139-224">Request</span></span>
<span data-ttu-id="1a139-225">次の例では、サービスの日付を日単位に変更し、請求日も更新しました。</span><span class="sxs-lookup"><span data-stu-id="1a139-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1a139-226">応答</span><span class="sxs-lookup"><span data-stu-id="1a139-226">Response</span></span>
<span data-ttu-id="1a139-227">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a139-227">The following is an example of the response.</span></span>
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
