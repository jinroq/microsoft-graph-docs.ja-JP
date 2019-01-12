---
title: Bookingappointment を更新します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c36f7033cb9a8f884436b4315399c794516a93ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917259"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="1e0c9-104">Bookingappointment を更新します。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-104">Update bookingappointment</span></span>

 > <span data-ttu-id="1e0c9-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e0c9-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1e0c9-107">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 [bookingAppointment](../resources/bookingappointment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-107">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1e0c9-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e0c9-108">Permissions</span></span>
<span data-ttu-id="1e0c9-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e0c9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e0c9-111">Permission type</span></span>      | <span data-ttu-id="1e0c9-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e0c9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e0c9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e0c9-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="1e0c9-114">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="1e0c9-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1e0c9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e0c9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e0c9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-116">Not supported.</span></span>   |
|<span data-ttu-id="1e0c9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e0c9-117">Application</span></span> | <span data-ttu-id="1e0c9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1e0c9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e0c9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1e0c9-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e0c9-120">Optional request headers</span></span>
| <span data-ttu-id="1e0c9-121">名前</span><span class="sxs-lookup"><span data-stu-id="1e0c9-121">Name</span></span>       | <span data-ttu-id="1e0c9-122">説明</span><span class="sxs-lookup"><span data-stu-id="1e0c9-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1e0c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e0c9-123">Authorization</span></span>  | <span data-ttu-id="1e0c9-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1e0c9-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e0c9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e0c9-125">Request body</span></span>
<span data-ttu-id="1e0c9-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1e0c9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e0c9-129">Property</span></span>     | <span data-ttu-id="1e0c9-130">種類</span><span class="sxs-lookup"><span data-stu-id="1e0c9-130">Type</span></span>   |<span data-ttu-id="1e0c9-131">説明</span><span class="sxs-lookup"><span data-stu-id="1e0c9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e0c9-132">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1e0c9-132">customerEmailAddress</span></span>|<span data-ttu-id="1e0c9-133">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-133">String</span></span>|<span data-ttu-id="1e0c9-134">予定を予約する、 [bookingCustomer](../resources/bookingcustomer.md)の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-134">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="1e0c9-135">customerId</span><span class="sxs-lookup"><span data-stu-id="1e0c9-135">customerId</span></span>|<span data-ttu-id="1e0c9-136">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-136">String</span></span>|<span data-ttu-id="1e0c9-137">この予定の[bookingCustomer](../resources/bookingcustomer.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-137">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="1e0c9-138">ID が指定されていない場合、予定を作成するとき、新しい**bookingCustomer**オブジェクトが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-138">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="1e0c9-139">1 回に設定する必要があります **[得意先コード]** 不変です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-139">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="1e0c9-140">customerLocation</span><span class="sxs-lookup"><span data-stu-id="1e0c9-140">customerLocation</span></span>|[<span data-ttu-id="1e0c9-141">location</span><span class="sxs-lookup"><span data-stu-id="1e0c9-141">location</span></span>](../resources/location.md)|<span data-ttu-id="1e0c9-142">予定を予約する、 [bookingCustomer](../resources/bookingcustomer.md)の場所の情報を表します。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-142">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="1e0c9-143">様</span><span class="sxs-lookup"><span data-stu-id="1e0c9-143">customerName</span></span>|<span data-ttu-id="1e0c9-144">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-144">String</span></span>|<span data-ttu-id="1e0c9-145">お客様の名前です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-145">The customer's name.</span></span>|
|<span data-ttu-id="1e0c9-146">customerNotes</span><span class="sxs-lookup"><span data-stu-id="1e0c9-146">customerNotes</span></span>|<span data-ttu-id="1e0c9-147">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-147">String</span></span>|<span data-ttu-id="1e0c9-148">この予定に関連付けられている顧客からのノート。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-148">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="1e0c9-149">その ID ではこの**bookingAppointment**を表示する場合のみ値を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-149">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="1e0c9-150">最初に顧客との新しい予定を作成する場合にのみ、このプロパティを設定することができます。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-150">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="1e0c9-151">その後も、 **[得意先コード]** で表される顧客からの値が計算されます。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-151">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="1e0c9-152">customerPhone</span><span class="sxs-lookup"><span data-stu-id="1e0c9-152">customerPhone</span></span>|<span data-ttu-id="1e0c9-153">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-153">String</span></span>|<span data-ttu-id="1e0c9-154">お客様の電話番号です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-154">The customer's phone number.</span></span>|
|<span data-ttu-id="1e0c9-155">duration</span><span class="sxs-lookup"><span data-stu-id="1e0c9-155">duration</span></span>|<span data-ttu-id="1e0c9-156">Duration</span><span class="sxs-lookup"><span data-stu-id="1e0c9-156">Duration</span></span>|<span data-ttu-id="1e0c9-157">[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、予定の長さです。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-157">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="1e0c9-158">end</span><span class="sxs-lookup"><span data-stu-id="1e0c9-158">end</span></span>|[<span data-ttu-id="1e0c9-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1e0c9-159">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1e0c9-160">日付、時刻、およびタイム ゾーンの予定を終了します。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-160">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="1e0c9-161">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="1e0c9-161">invoiceAmount</span></span>|<span data-ttu-id="1e0c9-162">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="1e0c9-162">Double</span></span>|<span data-ttu-id="1e0c9-163">請求書の請求金額です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-163">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="1e0c9-164">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="1e0c9-164">invoiceDate</span></span>|[<span data-ttu-id="1e0c9-165">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1e0c9-165">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1e0c9-166">日付、時刻、および請求書のこの予定のタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-166">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="1e0c9-167">invoiceId</span><span class="sxs-lookup"><span data-stu-id="1e0c9-167">invoiceId</span></span>|<span data-ttu-id="1e0c9-168">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-168">String</span></span>|<span data-ttu-id="1e0c9-169">請求書の ID。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-169">The ID of the invoice.</span></span>|
|<span data-ttu-id="1e0c9-170">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="1e0c9-170">invoiceStatus</span></span>|<span data-ttu-id="1e0c9-171">文字列</span><span class="sxs-lookup"><span data-stu-id="1e0c9-171">string</span></span>| <span data-ttu-id="1e0c9-172">請求書の状態です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-172">The status of the invoice.</span></span> <span data-ttu-id="1e0c9-173">使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-173">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="1e0c9-174">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="1e0c9-174">invoiceUrl</span></span>|<span data-ttu-id="1e0c9-175">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-175">String</span></span>|<span data-ttu-id="1e0c9-176">Microsoft の予約で請求書の URL です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-176">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="1e0c9-177">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="1e0c9-177">optOutOfCustomerEmail</span></span>|<span data-ttu-id="1e0c9-178">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e0c9-178">Boolean</span></span>|<span data-ttu-id="1e0c9-179">True は、この予定の[bookingCustomer](../resources/bookingcustomer.md)は、この予定の確認メッセージを表示するのには望んでいないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-179">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="1e0c9-180">事後バッファリング</span><span class="sxs-lookup"><span data-stu-id="1e0c9-180">postBuffer</span></span>|<span data-ttu-id="1e0c9-181">Duration</span><span class="sxs-lookup"><span data-stu-id="1e0c9-181">Duration</span></span>|<span data-ttu-id="1e0c9-182">クリーンアップ、例として、予定が終了した後に予約する時間の量。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-182">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="1e0c9-183">値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-183">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="1e0c9-184">事前バッファリング</span><span class="sxs-lookup"><span data-stu-id="1e0c9-184">preBuffer</span></span>|<span data-ttu-id="1e0c9-185">Duration</span><span class="sxs-lookup"><span data-stu-id="1e0c9-185">Duration</span></span>|<span data-ttu-id="1e0c9-186">例として、準備のため、予定の開始前に予約する時間の量。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-186">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="1e0c9-187">値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-187">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="1e0c9-188">価格</span><span class="sxs-lookup"><span data-stu-id="1e0c9-188">price</span></span>|<span data-ttu-id="1e0c9-189">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="1e0c9-189">Double</span></span>|<span data-ttu-id="1e0c9-190">指定された[bookingService](../resources/bookingservice.md)の予定の正規の価格です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-190">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="1e0c9-191">priceType</span><span class="sxs-lookup"><span data-stu-id="1e0c9-191">priceType</span></span>|<span data-ttu-id="1e0c9-192">文字列</span><span class="sxs-lookup"><span data-stu-id="1e0c9-192">string</span></span>| <span data-ttu-id="1e0c9-193">サービスの価格設定構造の柔軟性を提供するように設定します。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-193">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="1e0c9-194">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-194">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="1e0c9-195">アラーム</span><span class="sxs-lookup"><span data-stu-id="1e0c9-195">reminders</span></span>|<span data-ttu-id="1e0c9-196">[bookingReminder](../resources/bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1e0c9-196">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="1e0c9-197">この予定に送信される顧客の事前通知のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-197">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="1e0c9-198">その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-198">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="1e0c9-199">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="1e0c9-199">selfServiceAppointmentId</span></span>|<span data-ttu-id="1e0c9-200">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-200">String</span></span>|<span data-ttu-id="1e0c9-201">予定が作成された場合 [スケジュール] ページで、お客様が直接にではなく、お客様の代わりにスタッフのメンバーでは、予定の他の追跡 ID。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-201">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="1e0c9-202">serviceId</span><span class="sxs-lookup"><span data-stu-id="1e0c9-202">serviceId</span></span>|<span data-ttu-id="1e0c9-203">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-203">String</span></span>|<span data-ttu-id="1e0c9-204">[BookingService](../resources/bookingservice.md)の ID は、この予定に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-204">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="1e0c9-205">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="1e0c9-205">serviceLocation</span></span>|[<span data-ttu-id="1e0c9-206">location</span><span class="sxs-lookup"><span data-stu-id="1e0c9-206">location</span></span>](../resources/location.md)|<span data-ttu-id="1e0c9-207">サービスの配信場所です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-207">The location where the service is delivered.</span></span>|
|<span data-ttu-id="1e0c9-208">serviceName</span><span class="sxs-lookup"><span data-stu-id="1e0c9-208">serviceName</span></span>|<span data-ttu-id="1e0c9-209">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-209">String</span></span>|<span data-ttu-id="1e0c9-210">**BookingService**の名前は、この予定に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-210">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="1e0c9-211">新しい予定を作成するとき、このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-211">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="1e0c9-212">指定されていない場合は、 **serviceId**プロパティにより、予定に関連付けられたサービスから計算されます。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-212">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="1e0c9-213">serviceNotes</span><span class="sxs-lookup"><span data-stu-id="1e0c9-213">serviceNotes</span></span>|<span data-ttu-id="1e0c9-214">String</span><span class="sxs-lookup"><span data-stu-id="1e0c9-214">String</span></span>|<span data-ttu-id="1e0c9-215">の[bookingStaffMember](../resources/bookingstaffmember.md)からのノート。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-215">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="1e0c9-216">その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-216">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="1e0c9-217">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="1e0c9-217">staffMemberIds</span></span>|<span data-ttu-id="1e0c9-218">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1e0c9-218">String collection</span></span>|<span data-ttu-id="1e0c9-219">この予定にスケジュールされている各[bookingStaffMember](../resources/bookingstaffmember.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-219">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="1e0c9-220">start</span><span class="sxs-lookup"><span data-stu-id="1e0c9-220">start</span></span>|[<span data-ttu-id="1e0c9-221">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1e0c9-221">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="1e0c9-222">日付、時刻、およびタイム ゾーンの予定の開始をします。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-222">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="1e0c9-223">応答</span><span class="sxs-lookup"><span data-stu-id="1e0c9-223">Response</span></span>
<span data-ttu-id="1e0c9-p115">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-p115">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e0c9-226">例</span><span class="sxs-lookup"><span data-stu-id="1e0c9-226">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e0c9-227">要求</span><span class="sxs-lookup"><span data-stu-id="1e0c9-227">Request</span></span>
<span data-ttu-id="1e0c9-228">次の例では、サービスが、1 日の日付を変更し、請求書の日付を更新します。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-228">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1e0c9-229">応答</span><span class="sxs-lookup"><span data-stu-id="1e0c9-229">Response</span></span>
<span data-ttu-id="1e0c9-230">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e0c9-230">The following is an example of the response.</span></span>
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
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
