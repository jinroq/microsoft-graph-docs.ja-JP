---
title: Bookingappointment の更新
description: 指定した bookingappointment の bookingAppointment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 5ccb03b1dc2d84721c3d2ecb366c05992c443d6b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865973"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="1ccdc-103">Bookingappointment の更新</span><span class="sxs-lookup"><span data-stu-id="1ccdc-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ccdc-104">指定した[bookingappointment](../resources/bookingbusiness.md)の[bookingappointment](../resources/bookingappointment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1ccdc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ccdc-105">Permissions</span></span>
<span data-ttu-id="1ccdc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ccdc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ccdc-108">Permission type</span></span>      | <span data-ttu-id="1ccdc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ccdc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ccdc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ccdc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1ccdc-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="1ccdc-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1ccdc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ccdc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ccdc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-113">Not supported.</span></span>   |
|<span data-ttu-id="1ccdc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ccdc-114">Application</span></span> | <span data-ttu-id="1ccdc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1ccdc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ccdc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1ccdc-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ccdc-117">Optional request headers</span></span>
| <span data-ttu-id="1ccdc-118">名前</span><span class="sxs-lookup"><span data-stu-id="1ccdc-118">Name</span></span>       | <span data-ttu-id="1ccdc-119">説明</span><span class="sxs-lookup"><span data-stu-id="1ccdc-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1ccdc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ccdc-120">Authorization</span></span>  | <span data-ttu-id="1ccdc-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1ccdc-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ccdc-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ccdc-122">Request body</span></span>
<span data-ttu-id="1ccdc-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1ccdc-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ccdc-126">Property</span></span>     | <span data-ttu-id="1ccdc-127">型</span><span class="sxs-lookup"><span data-stu-id="1ccdc-127">Type</span></span>   |<span data-ttu-id="1ccdc-128">説明</span><span class="sxs-lookup"><span data-stu-id="1ccdc-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ccdc-129">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1ccdc-129">customerEmailAddress</span></span>|<span data-ttu-id="1ccdc-130">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-130">String</span></span>|<span data-ttu-id="1ccdc-131">予定を予約している[Bookingcustomer](../resources/bookingcustomer.md)の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="1ccdc-132">Id</span><span class="sxs-lookup"><span data-stu-id="1ccdc-132">customerId</span></span>|<span data-ttu-id="1ccdc-133">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-133">String</span></span>|<span data-ttu-id="1ccdc-134">この予定の[Bookingcustomer](../resources/bookingcustomer.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="1ccdc-135">予定の作成時に ID が指定されていない場合は、新しい**Bookingcustomer**オブジェクトが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="1ccdc-136">設定すると、 **customerId**を不変にすることを考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="1ccdc-137">顧客の所在地</span><span class="sxs-lookup"><span data-stu-id="1ccdc-137">customerLocation</span></span>|[<span data-ttu-id="1ccdc-138">location</span><span class="sxs-lookup"><span data-stu-id="1ccdc-138">location</span></span>](../resources/location.md)|<span data-ttu-id="1ccdc-139">予定を予約している[Bookingcustomer](../resources/bookingcustomer.md)の場所情報を表します。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="1ccdc-140">おける</span><span class="sxs-lookup"><span data-stu-id="1ccdc-140">customerName</span></span>|<span data-ttu-id="1ccdc-141">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-141">String</span></span>|<span data-ttu-id="1ccdc-142">顧客の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-142">The customer's name.</span></span>|
|<span data-ttu-id="1ccdc-143">顧客メモ</span><span class="sxs-lookup"><span data-stu-id="1ccdc-143">customerNotes</span></span>|<span data-ttu-id="1ccdc-144">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-144">String</span></span>|<span data-ttu-id="1ccdc-145">この予定に関連付けられている顧客からのメモ。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="1ccdc-146">ID でこの**Bookingappointment**を読み取る場合にのみ、値を取得できます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="1ccdc-147">このプロパティは、最初に新しい顧客を使用して予定を作成するときにのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="1ccdc-148">その時点で、その値は**customerId**で表される顧客から計算されます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="1ccdc-149">顧客電話</span><span class="sxs-lookup"><span data-stu-id="1ccdc-149">customerPhone</span></span>|<span data-ttu-id="1ccdc-150">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-150">String</span></span>|<span data-ttu-id="1ccdc-151">お客様の電話番号。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-151">The customer's phone number.</span></span>|
|<span data-ttu-id="1ccdc-152">duration</span><span class="sxs-lookup"><span data-stu-id="1ccdc-152">duration</span></span>|<span data-ttu-id="1ccdc-153">期間</span><span class="sxs-lookup"><span data-stu-id="1ccdc-153">Duration</span></span>|<span data-ttu-id="1ccdc-154">「文字形式」で示されて[](https://www.iso.org/iso-8601-date-and-time-format.html)いる予定の長さ。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="1ccdc-155">end</span><span class="sxs-lookup"><span data-stu-id="1ccdc-155">end</span></span>|[<span data-ttu-id="1ccdc-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1ccdc-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1ccdc-157">予定が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="1ccdc-158">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="1ccdc-158">invoiceAmount</span></span>|<span data-ttu-id="1ccdc-159">2 行分</span><span class="sxs-lookup"><span data-stu-id="1ccdc-159">Double</span></span>|<span data-ttu-id="1ccdc-160">請求書の請求金額。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="1ccdc-161">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="1ccdc-161">invoiceDate</span></span>|[<span data-ttu-id="1ccdc-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1ccdc-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1ccdc-163">この予定の請求書の日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="1ccdc-164">invoiceId</span><span class="sxs-lookup"><span data-stu-id="1ccdc-164">invoiceId</span></span>|<span data-ttu-id="1ccdc-165">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-165">String</span></span>|<span data-ttu-id="1ccdc-166">請求書の ID。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="1ccdc-167">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="1ccdc-167">invoiceStatus</span></span>|<span data-ttu-id="1ccdc-168">string</span><span class="sxs-lookup"><span data-stu-id="1ccdc-168">string</span></span>| <span data-ttu-id="1ccdc-169">請求書の状態。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-169">The status of the invoice.</span></span> <span data-ttu-id="1ccdc-170">使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="1ccdc-171">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="1ccdc-171">invoiceUrl</span></span>|<span data-ttu-id="1ccdc-172">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-172">String</span></span>|<span data-ttu-id="1ccdc-173">Microsoft 予約の請求書の URL。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="1ccdc-174">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="1ccdc-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="1ccdc-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ccdc-175">Boolean</span></span>|<span data-ttu-id="1ccdc-176">True は、この予定の[Bookingcustomer](../resources/bookingcustomer.md)が、この予定の確認を受信したくないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="1ccdc-177">postBuffer</span><span class="sxs-lookup"><span data-stu-id="1ccdc-177">postBuffer</span></span>|<span data-ttu-id="1ccdc-178">期間</span><span class="sxs-lookup"><span data-stu-id="1ccdc-178">Duration</span></span>|<span data-ttu-id="1ccdc-179">予定が終了した後に、クリーンアップのために確保する時間の長さを例として示します。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="1ccdc-180">この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="1ccdc-181">preBuffer</span><span class="sxs-lookup"><span data-stu-id="1ccdc-181">preBuffer</span></span>|<span data-ttu-id="1ccdc-182">期間</span><span class="sxs-lookup"><span data-stu-id="1ccdc-182">Duration</span></span>|<span data-ttu-id="1ccdc-183">準備のために予定が開始されるまでの時間を例として示します。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="1ccdc-184">この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="1ccdc-185">代金</span><span class="sxs-lookup"><span data-stu-id="1ccdc-185">price</span></span>|<span data-ttu-id="1ccdc-186">2 行分</span><span class="sxs-lookup"><span data-stu-id="1ccdc-186">Double</span></span>|<span data-ttu-id="1ccdc-187">指定した[Bookingservice](../resources/bookingservice.md)の予定に対する正規の価格。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="1ccdc-188">priceType</span><span class="sxs-lookup"><span data-stu-id="1ccdc-188">priceType</span></span>|<span data-ttu-id="1ccdc-189">string</span><span class="sxs-lookup"><span data-stu-id="1ccdc-189">string</span></span>| <span data-ttu-id="1ccdc-190">サービスの価格構造を柔軟に提供するための設定。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="1ccdc-191">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="1ccdc-192">isp</span><span class="sxs-lookup"><span data-stu-id="1ccdc-192">reminders</span></span>|<span data-ttu-id="1ccdc-193">[Bookingreminder](../resources/bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ccdc-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="1ccdc-194">この予定に対して送信された顧客のアラームのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="1ccdc-195">このプロパティの値は、この**Bookingappointment**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="1ccdc-196">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="1ccdc-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="1ccdc-197">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-197">String</span></span>|<span data-ttu-id="1ccdc-198">顧客に代わってスタッフメンバーではなく、顧客が [スケジュール] ページで直接作成された予定の場合は、予定の追加の追跡 ID。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="1ccdc-199">serviceId</span><span class="sxs-lookup"><span data-stu-id="1ccdc-199">serviceId</span></span>|<span data-ttu-id="1ccdc-200">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-200">String</span></span>|<span data-ttu-id="1ccdc-201">この予定に関連付けられている[Bookingservice](../resources/bookingservice.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="1ccdc-202">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="1ccdc-202">serviceLocation</span></span>|[<span data-ttu-id="1ccdc-203">location</span><span class="sxs-lookup"><span data-stu-id="1ccdc-203">location</span></span>](../resources/location.md)|<span data-ttu-id="1ccdc-204">サービスが配信される場所。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="1ccdc-205">serviceName</span><span class="sxs-lookup"><span data-stu-id="1ccdc-205">serviceName</span></span>|<span data-ttu-id="1ccdc-206">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-206">String</span></span>|<span data-ttu-id="1ccdc-207">この予定に関連付けられている**Bookingservice**の名前です。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="1ccdc-208">新しい予定を作成するときは、このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="1ccdc-209">指定しない場合、 **serviceId**プロパティによって、予定に関連付けられているサービスから計算されます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="1ccdc-210">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="1ccdc-210">serviceNotes</span></span>|<span data-ttu-id="1ccdc-211">String</span><span class="sxs-lookup"><span data-stu-id="1ccdc-211">String</span></span>|<span data-ttu-id="1ccdc-212">[BookingStaffMember](../resources/bookingstaffmember.md)からのメモ。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="1ccdc-213">このプロパティの値は、この**Bookingappointment**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="1ccdc-214">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="1ccdc-214">staffMemberIds</span></span>|<span data-ttu-id="1ccdc-215">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1ccdc-215">String collection</span></span>|<span data-ttu-id="1ccdc-216">この予定でスケジュールされている各[bookingStaffMember](../resources/bookingstaffmember.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="1ccdc-217">開始</span><span class="sxs-lookup"><span data-stu-id="1ccdc-217">start</span></span>|[<span data-ttu-id="1ccdc-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1ccdc-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1ccdc-219">予定が開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="1ccdc-220">応答</span><span class="sxs-lookup"><span data-stu-id="1ccdc-220">Response</span></span>
<span data-ttu-id="1ccdc-p113">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ccdc-223">例</span><span class="sxs-lookup"><span data-stu-id="1ccdc-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ccdc-224">要求</span><span class="sxs-lookup"><span data-stu-id="1ccdc-224">Request</span></span>
<span data-ttu-id="1ccdc-225">次の例では、サービスの日付を日単位に変更し、請求日も更新しました。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1ccdc-226">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1ccdc-226">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ccdc-227">C#</span><span class="sxs-lookup"><span data-stu-id="1ccdc-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ccdc-228">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ccdc-228">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1ccdc-229">目的-C</span><span class="sxs-lookup"><span data-stu-id="1ccdc-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1ccdc-230">Java</span><span class="sxs-lookup"><span data-stu-id="1ccdc-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1ccdc-231">応答</span><span class="sxs-lookup"><span data-stu-id="1ccdc-231">Response</span></span>
<span data-ttu-id="1ccdc-232">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ccdc-232">The following is an example of the response.</span></span>
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
  ]
}
-->
