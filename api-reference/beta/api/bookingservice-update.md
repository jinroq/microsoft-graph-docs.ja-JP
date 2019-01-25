---
title: Bookingservice を更新します。
description: 指定された bookingbusiness で、bookingService オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519718"
---
# <a name="update-bookingservice"></a><span data-ttu-id="c7bf2-103">Bookingservice を更新します。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7bf2-104">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 [bookingService](../resources/bookingservice.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="c7bf2-105">サービスをカスタマイズすることができます例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="c7bf2-106">Price</span><span class="sxs-lookup"><span data-stu-id="c7bf2-106">Price</span></span>
- <span data-ttu-id="c7bf2-107">予定の標準的な長さ</span><span class="sxs-lookup"><span data-stu-id="c7bf2-107">Typical length of an appointment</span></span>
- <span data-ttu-id="c7bf2-108">Reminders</span><span class="sxs-lookup"><span data-stu-id="c7bf2-108">Reminders</span></span>
- <span data-ttu-id="c7bf2-109">バッファーを設定する前にまたはサービス終了するたび</span><span class="sxs-lookup"><span data-stu-id="c7bf2-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="c7bf2-110">予約を取り消すには、最低限の通知などのパラメーターの[ポリシーのスケジュールを設定](../resources/bookingschedulingpolicy.md)し、お客様が予定の特定のスタッフのメンバーを選択するかどうか。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7bf2-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c7bf2-111">Permissions</span></span>
<span data-ttu-id="c7bf2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7bf2-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7bf2-114">Permission type</span></span>      | <span data-ttu-id="c7bf2-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7bf2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7bf2-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7bf2-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="c7bf2-117">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c7bf2-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c7bf2-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7bf2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7bf2-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-119">Not supported.</span></span>   |
|<span data-ttu-id="c7bf2-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7bf2-120">Application</span></span> | <span data-ttu-id="c7bf2-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c7bf2-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7bf2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c7bf2-123">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7bf2-123">Optional request headers</span></span>
| <span data-ttu-id="c7bf2-124">名前</span><span class="sxs-lookup"><span data-stu-id="c7bf2-124">Name</span></span>       | <span data-ttu-id="c7bf2-125">説明</span><span class="sxs-lookup"><span data-stu-id="c7bf2-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c7bf2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7bf2-126">Authorization</span></span>  | <span data-ttu-id="c7bf2-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c7bf2-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7bf2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7bf2-128">Request body</span></span>
<span data-ttu-id="c7bf2-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c7bf2-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7bf2-132">Property</span></span>     | <span data-ttu-id="c7bf2-133">型</span><span class="sxs-lookup"><span data-stu-id="c7bf2-133">Type</span></span>   |<span data-ttu-id="c7bf2-134">説明</span><span class="sxs-lookup"><span data-stu-id="c7bf2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7bf2-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="c7bf2-135">defaultDuration</span></span>|<span data-ttu-id="c7bf2-136">Duration</span><span class="sxs-lookup"><span data-stu-id="c7bf2-136">Duration</span></span>|<span data-ttu-id="c7bf2-137">日、時間、分、秒単位の数値で表される、サービスの既定の長さです。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="c7bf2-138">たとえば、P11D23H59M59.999999999999S です。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="c7bf2-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="c7bf2-139">defaultLocation</span></span>|[<span data-ttu-id="c7bf2-140">location</span><span class="sxs-lookup"><span data-stu-id="c7bf2-140">location</span></span>](../resources/location.md)|<span data-ttu-id="c7bf2-141">サービスの既定の物理的な場所です。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="c7bf2-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="c7bf2-142">defaultPrice</span></span>|<span data-ttu-id="c7bf2-143">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="c7bf2-143">Double</span></span>|<span data-ttu-id="c7bf2-144">サービスの既定通貨の価格です。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="c7bf2-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="c7bf2-145">defaultPriceType</span></span>|<span data-ttu-id="c7bf2-146">string</span><span class="sxs-lookup"><span data-stu-id="c7bf2-146">string</span></span>|<span data-ttu-id="c7bf2-147">サービスの既定の方法に請求されます。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-147">The default way the service is charged.</span></span> <span data-ttu-id="c7bf2-148">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="c7bf2-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="c7bf2-149">defaultReminders</span></span>|<span data-ttu-id="c7bf2-150">[bookingReminder](../resources/bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c7bf2-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="c7bf2-151">このサービスの予定に対するアラームの既定値を設定します。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="c7bf2-152">その ID ではこの**bookingService**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="c7bf2-153">説明</span><span class="sxs-lookup"><span data-stu-id="c7bf2-153">description</span></span>|<span data-ttu-id="c7bf2-154">文字列</span><span class="sxs-lookup"><span data-stu-id="c7bf2-154">String</span></span>|<span data-ttu-id="c7bf2-155">サービスの説明です。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-155">A text description for the service.</span></span>|
|<span data-ttu-id="c7bf2-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c7bf2-156">displayName</span></span>|<span data-ttu-id="c7bf2-157">String</span><span class="sxs-lookup"><span data-stu-id="c7bf2-157">String</span></span>|<span data-ttu-id="c7bf2-158">サービスの名前です。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-158">A service name.</span></span>|
|<span data-ttu-id="c7bf2-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c7bf2-159">emailAddress</span></span>|<span data-ttu-id="c7bf2-160">String</span><span class="sxs-lookup"><span data-stu-id="c7bf2-160">String</span></span>|<span data-ttu-id="c7bf2-161">電子メール アドレス:  </span><span class="sxs-lookup"><span data-stu-id="c7bf2-161">An email address</span></span>|
|<span data-ttu-id="c7bf2-162">id</span><span class="sxs-lookup"><span data-stu-id="c7bf2-162">id</span></span>|<span data-ttu-id="c7bf2-163">文字列</span><span class="sxs-lookup"><span data-stu-id="c7bf2-163">String</span></span>| <span data-ttu-id="c7bf2-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-164">Read-only.</span></span>|
|<span data-ttu-id="c7bf2-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="c7bf2-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="c7bf2-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="c7bf2-166">Boolean</span></span>|<span data-ttu-id="c7bf2-167">True は、このサービスは予約のお客様に利用できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="c7bf2-168">notes</span><span class="sxs-lookup"><span data-stu-id="c7bf2-168">notes</span></span>|<span data-ttu-id="c7bf2-169">String</span><span class="sxs-lookup"><span data-stu-id="c7bf2-169">String</span></span>|<span data-ttu-id="c7bf2-170">このサービスに関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-170">Additional information about this service.</span></span>|
|<span data-ttu-id="c7bf2-171">事後バッファリング</span><span class="sxs-lookup"><span data-stu-id="c7bf2-171">postBuffer</span></span>|<span data-ttu-id="c7bf2-172">Duration</span><span class="sxs-lookup"><span data-stu-id="c7bf2-172">Duration</span></span>|<span data-ttu-id="c7bf2-173">このサービスの予定の後のバッファーに時間が終了して、次の前に顧客の予定が予約できます。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="c7bf2-174">事前バッファリング</span><span class="sxs-lookup"><span data-stu-id="c7bf2-174">preBuffer</span></span>|<span data-ttu-id="c7bf2-175">Duration</span><span class="sxs-lookup"><span data-stu-id="c7bf2-175">Duration</span></span>|<span data-ttu-id="c7bf2-176">このサービスに対する予定を開始する前に、バッファーに格納する時間です。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="c7bf2-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="c7bf2-177">schedulingPolicy</span></span>|[<span data-ttu-id="c7bf2-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="c7bf2-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="c7bf2-179">この種類のサービスの予定を作成および管理する方法を決定するポリシーのセットです。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="c7bf2-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="c7bf2-180">staffMemberIds</span></span>|<span data-ttu-id="c7bf2-181">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c7bf2-181">String collection</span></span>|<span data-ttu-id="c7bf2-182">このサービスを提供している[スタッフのメンバー](../resources/bookingstaffmember.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="c7bf2-183">応答</span><span class="sxs-lookup"><span data-stu-id="c7bf2-183">Response</span></span>
<span data-ttu-id="c7bf2-p106">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7bf2-186">例</span><span class="sxs-lookup"><span data-stu-id="c7bf2-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7bf2-187">要求</span><span class="sxs-lookup"><span data-stu-id="c7bf2-187">Request</span></span>
<span data-ttu-id="c7bf2-188">次の例では、指定されたサービスの期間を更新します。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-188">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c7bf2-189">応答</span><span class="sxs-lookup"><span data-stu-id="c7bf2-189">Response</span></span>
<span data-ttu-id="c7bf2-190">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7bf2-190">The following is an example of the response.</span></span>
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
