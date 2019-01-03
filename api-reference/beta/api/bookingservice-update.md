---
title: Bookingservice を更新します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: e39ad73b7f9acf2337db517e67895bc4601598a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068684"
---
# <a name="update-bookingservice"></a><span data-ttu-id="4818f-104">Bookingservice を更新します。</span><span class="sxs-lookup"><span data-stu-id="4818f-104">Update bookingservice</span></span>

 > <span data-ttu-id="4818f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4818f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4818f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4818f-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="4818f-107">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 [bookingService](../resources/bookingservice.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4818f-107">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="4818f-108">サービスをカスタマイズすることができます例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4818f-108">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="4818f-109">Price</span><span class="sxs-lookup"><span data-stu-id="4818f-109">Price</span></span>
- <span data-ttu-id="4818f-110">予定の標準的な長さ</span><span class="sxs-lookup"><span data-stu-id="4818f-110">Typical length of an appointment</span></span>
- <span data-ttu-id="4818f-111">Reminders</span><span class="sxs-lookup"><span data-stu-id="4818f-111">Reminders</span></span>
- <span data-ttu-id="4818f-112">バッファーを設定する前にまたはサービス終了するたび</span><span class="sxs-lookup"><span data-stu-id="4818f-112">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="4818f-113">予約を取り消すには、最低限の通知などのパラメーターの[ポリシーのスケジュールを設定](../resources/bookingschedulingpolicy.md)し、お客様が予定の特定のスタッフのメンバーを選択するかどうか。</span><span class="sxs-lookup"><span data-stu-id="4818f-113">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="4818f-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4818f-114">Permissions</span></span>
<span data-ttu-id="4818f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4818f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4818f-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4818f-117">Permission type</span></span>      | <span data-ttu-id="4818f-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4818f-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4818f-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4818f-119">Delegated (work or school account)</span></span> |  <span data-ttu-id="4818f-120">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4818f-120">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4818f-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4818f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4818f-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4818f-122">Not supported.</span></span>   |
|<span data-ttu-id="4818f-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4818f-123">Application</span></span> | <span data-ttu-id="4818f-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4818f-124">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4818f-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4818f-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4818f-126">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4818f-126">Optional request headers</span></span>
| <span data-ttu-id="4818f-127">名前</span><span class="sxs-lookup"><span data-stu-id="4818f-127">Name</span></span>       | <span data-ttu-id="4818f-128">説明</span><span class="sxs-lookup"><span data-stu-id="4818f-128">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4818f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4818f-129">Authorization</span></span>  | <span data-ttu-id="4818f-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4818f-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4818f-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="4818f-131">Request body</span></span>
<span data-ttu-id="4818f-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4818f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4818f-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4818f-135">Property</span></span>     | <span data-ttu-id="4818f-136">型</span><span class="sxs-lookup"><span data-stu-id="4818f-136">Type</span></span>   |<span data-ttu-id="4818f-137">説明</span><span class="sxs-lookup"><span data-stu-id="4818f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4818f-138">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="4818f-138">defaultDuration</span></span>|<span data-ttu-id="4818f-139">Duration</span><span class="sxs-lookup"><span data-stu-id="4818f-139">Duration</span></span>|<span data-ttu-id="4818f-140">日、時間、分、秒単位の数値で表される、サービスの既定の長さです。</span><span class="sxs-lookup"><span data-stu-id="4818f-140">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="4818f-141">たとえば、P11D23H59M59.999999999999S です。</span><span class="sxs-lookup"><span data-stu-id="4818f-141">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="4818f-142">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="4818f-142">defaultLocation</span></span>|[<span data-ttu-id="4818f-143">location</span><span class="sxs-lookup"><span data-stu-id="4818f-143">location</span></span>](../resources/location.md)|<span data-ttu-id="4818f-144">サービスの既定の物理的な場所です。</span><span class="sxs-lookup"><span data-stu-id="4818f-144">The default physical location for the service.</span></span>|
|<span data-ttu-id="4818f-145">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="4818f-145">defaultPrice</span></span>|<span data-ttu-id="4818f-146">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="4818f-146">Double</span></span>|<span data-ttu-id="4818f-147">サービスの既定通貨の価格です。</span><span class="sxs-lookup"><span data-stu-id="4818f-147">The default monetary price for the service.</span></span>|
|<span data-ttu-id="4818f-148">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="4818f-148">defaultPriceType</span></span>|<span data-ttu-id="4818f-149">文字列</span><span class="sxs-lookup"><span data-stu-id="4818f-149">string</span></span>|<span data-ttu-id="4818f-150">サービスの既定の方法に請求されます。</span><span class="sxs-lookup"><span data-stu-id="4818f-150">The default way the service is charged.</span></span> <span data-ttu-id="4818f-151">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="4818f-151">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="4818f-152">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="4818f-152">defaultReminders</span></span>|<span data-ttu-id="4818f-153">[bookingReminder](../resources/bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4818f-153">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="4818f-154">このサービスの予定に対するアラームの既定値を設定します。</span><span class="sxs-lookup"><span data-stu-id="4818f-154">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="4818f-155">その ID ではこの**bookingService**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="4818f-155">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="4818f-156">説明</span><span class="sxs-lookup"><span data-stu-id="4818f-156">description</span></span>|<span data-ttu-id="4818f-157">String</span><span class="sxs-lookup"><span data-stu-id="4818f-157">String</span></span>|<span data-ttu-id="4818f-158">サービスの説明です。</span><span class="sxs-lookup"><span data-stu-id="4818f-158">A text description for the service.</span></span>|
|<span data-ttu-id="4818f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4818f-159">displayName</span></span>|<span data-ttu-id="4818f-160">String</span><span class="sxs-lookup"><span data-stu-id="4818f-160">String</span></span>|<span data-ttu-id="4818f-161">サービスの名前です。</span><span class="sxs-lookup"><span data-stu-id="4818f-161">A service name.</span></span>|
|<span data-ttu-id="4818f-162">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4818f-162">emailAddress</span></span>|<span data-ttu-id="4818f-163">String</span><span class="sxs-lookup"><span data-stu-id="4818f-163">String</span></span>|<span data-ttu-id="4818f-164">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="4818f-164">An email address</span></span>|
|<span data-ttu-id="4818f-165">id</span><span class="sxs-lookup"><span data-stu-id="4818f-165">id</span></span>|<span data-ttu-id="4818f-166">String</span><span class="sxs-lookup"><span data-stu-id="4818f-166">String</span></span>| <span data-ttu-id="4818f-167">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4818f-167">Read-only.</span></span>|
|<span data-ttu-id="4818f-168">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="4818f-168">isHiddenFromCustomers</span></span>|<span data-ttu-id="4818f-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="4818f-169">Boolean</span></span>|<span data-ttu-id="4818f-170">True は、このサービスは予約のお客様に利用できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="4818f-170">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="4818f-171">notes</span><span class="sxs-lookup"><span data-stu-id="4818f-171">notes</span></span>|<span data-ttu-id="4818f-172">String</span><span class="sxs-lookup"><span data-stu-id="4818f-172">String</span></span>|<span data-ttu-id="4818f-173">このサービスに関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="4818f-173">Additional information about this service.</span></span>|
|<span data-ttu-id="4818f-174">事後バッファリング</span><span class="sxs-lookup"><span data-stu-id="4818f-174">postBuffer</span></span>|<span data-ttu-id="4818f-175">Duration</span><span class="sxs-lookup"><span data-stu-id="4818f-175">Duration</span></span>|<span data-ttu-id="4818f-176">このサービスの予定の後のバッファーに時間が終了して、次の前に顧客の予定が予約できます。</span><span class="sxs-lookup"><span data-stu-id="4818f-176">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="4818f-177">事前バッファリング</span><span class="sxs-lookup"><span data-stu-id="4818f-177">preBuffer</span></span>|<span data-ttu-id="4818f-178">Duration</span><span class="sxs-lookup"><span data-stu-id="4818f-178">Duration</span></span>|<span data-ttu-id="4818f-179">このサービスに対する予定を開始する前に、バッファーに格納する時間です。</span><span class="sxs-lookup"><span data-stu-id="4818f-179">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="4818f-180">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4818f-180">schedulingPolicy</span></span>|[<span data-ttu-id="4818f-181">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4818f-181">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="4818f-182">この種類のサービスの予定を作成および管理する方法を決定するポリシーのセットです。</span><span class="sxs-lookup"><span data-stu-id="4818f-182">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="4818f-183">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="4818f-183">staffMemberIds</span></span>|<span data-ttu-id="4818f-184">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4818f-184">String collection</span></span>|<span data-ttu-id="4818f-185">このサービスを提供している[スタッフのメンバー](../resources/bookingstaffmember.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="4818f-185">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="4818f-186">応答</span><span class="sxs-lookup"><span data-stu-id="4818f-186">Response</span></span>
<span data-ttu-id="4818f-p108">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4818f-p108">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4818f-189">例</span><span class="sxs-lookup"><span data-stu-id="4818f-189">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4818f-190">要求</span><span class="sxs-lookup"><span data-stu-id="4818f-190">Request</span></span>
<span data-ttu-id="4818f-191">次の例では、指定されたサービスの期間を更新します。</span><span class="sxs-lookup"><span data-stu-id="4818f-191">The following example updates the duration of the specified service.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a><span data-ttu-id="4818f-192">応答</span><span class="sxs-lookup"><span data-stu-id="4818f-192">Response</span></span>
<span data-ttu-id="4818f-193">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4818f-193">The following is an example of the response.</span></span> 
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->