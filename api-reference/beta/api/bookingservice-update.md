---
title: Bookingservice を更新する
description: 指定した bookingservice の bookingService オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0225259461c31591df679e50ebd5748e47c004a1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439043"
---
# <a name="update-bookingservice"></a><span data-ttu-id="1ba3b-103">Bookingservice を更新する</span><span class="sxs-lookup"><span data-stu-id="1ba3b-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ba3b-104">指定した[bookingservice](../resources/bookingbusiness.md)の[bookingservice](../resources/bookingservice.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="1ba3b-105">以下に、サービスに対してカスタマイズできる例をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="1ba3b-106">Price</span><span class="sxs-lookup"><span data-stu-id="1ba3b-106">Price</span></span>
- <span data-ttu-id="1ba3b-107">予定の通常の長さ</span><span class="sxs-lookup"><span data-stu-id="1ba3b-107">Typical length of an appointment</span></span>
- <span data-ttu-id="1ba3b-108">Reminders</span><span class="sxs-lookup"><span data-stu-id="1ba3b-108">Reminders</span></span>
- <span data-ttu-id="1ba3b-109">サービスの実行前または完了後にセットアップする任意の時間バッファー</span><span class="sxs-lookup"><span data-stu-id="1ba3b-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="1ba3b-110">予約またはキャンセルするための最小限の通知や、ユーザーが予定に対して特定のスタッフメンバーを選択できるかどうかの[スケジュールポリシー](../resources/bookingschedulingpolicy.md)パラメーター。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ba3b-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ba3b-111">Permissions</span></span>
<span data-ttu-id="1ba3b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ba3b-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ba3b-114">Permission type</span></span>      | <span data-ttu-id="1ba3b-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ba3b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ba3b-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ba3b-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="1ba3b-117">予約します。すべての予約</span><span class="sxs-lookup"><span data-stu-id="1ba3b-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1ba3b-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ba3b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ba3b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-119">Not supported.</span></span>   |
|<span data-ttu-id="1ba3b-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ba3b-120">Application</span></span> | <span data-ttu-id="1ba3b-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1ba3b-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ba3b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1ba3b-123">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ba3b-123">Optional request headers</span></span>
| <span data-ttu-id="1ba3b-124">名前</span><span class="sxs-lookup"><span data-stu-id="1ba3b-124">Name</span></span>       | <span data-ttu-id="1ba3b-125">説明</span><span class="sxs-lookup"><span data-stu-id="1ba3b-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1ba3b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ba3b-126">Authorization</span></span>  | <span data-ttu-id="1ba3b-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1ba3b-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ba3b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ba3b-128">Request body</span></span>
<span data-ttu-id="1ba3b-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1ba3b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ba3b-132">Property</span></span>     | <span data-ttu-id="1ba3b-133">型</span><span class="sxs-lookup"><span data-stu-id="1ba3b-133">Type</span></span>   |<span data-ttu-id="1ba3b-134">説明</span><span class="sxs-lookup"><span data-stu-id="1ba3b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ba3b-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="1ba3b-135">defaultDuration</span></span>|<span data-ttu-id="1ba3b-136">期間</span><span class="sxs-lookup"><span data-stu-id="1ba3b-136">Duration</span></span>|<span data-ttu-id="1ba3b-137">サービスの既定の長さ。日数、時間、分、および秒で表されます。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="1ba3b-138">たとえば、P11D23H59M 59.999999999999 S のようになります。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="1ba3b-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="1ba3b-139">defaultLocation</span></span>|[<span data-ttu-id="1ba3b-140">location</span><span class="sxs-lookup"><span data-stu-id="1ba3b-140">location</span></span>](../resources/location.md)|<span data-ttu-id="1ba3b-141">サービスの既定の物理的な場所。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="1ba3b-142">既定の価格</span><span class="sxs-lookup"><span data-stu-id="1ba3b-142">defaultPrice</span></span>|<span data-ttu-id="1ba3b-143">2 行分</span><span class="sxs-lookup"><span data-stu-id="1ba3b-143">Double</span></span>|<span data-ttu-id="1ba3b-144">サービスの既定の通貨料金。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="1ba3b-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="1ba3b-145">defaultPriceType</span></span>|<span data-ttu-id="1ba3b-146">string</span><span class="sxs-lookup"><span data-stu-id="1ba3b-146">string</span></span>|<span data-ttu-id="1ba3b-147">サービスの既定の課金方法。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-147">The default way the service is charged.</span></span> <span data-ttu-id="1ba3b-148">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="1ba3b-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="1ba3b-149">defaultReminders</span></span>|<span data-ttu-id="1ba3b-150">[Bookingreminder](../resources/bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ba3b-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="1ba3b-151">このサービスの予定に対する既定のアラームのセット。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="1ba3b-152">このプロパティの値は、この**Bookingservice**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="1ba3b-153">description</span><span class="sxs-lookup"><span data-stu-id="1ba3b-153">description</span></span>|<span data-ttu-id="1ba3b-154">String</span><span class="sxs-lookup"><span data-stu-id="1ba3b-154">String</span></span>|<span data-ttu-id="1ba3b-155">サービスのテキストの説明。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-155">A text description for the service.</span></span>|
|<span data-ttu-id="1ba3b-156">displayName</span><span class="sxs-lookup"><span data-stu-id="1ba3b-156">displayName</span></span>|<span data-ttu-id="1ba3b-157">String</span><span class="sxs-lookup"><span data-stu-id="1ba3b-157">String</span></span>|<span data-ttu-id="1ba3b-158">サービス名。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-158">A service name.</span></span>|
|<span data-ttu-id="1ba3b-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1ba3b-159">emailAddress</span></span>|<span data-ttu-id="1ba3b-160">String</span><span class="sxs-lookup"><span data-stu-id="1ba3b-160">String</span></span>|<span data-ttu-id="1ba3b-161">電子メールアドレス</span><span class="sxs-lookup"><span data-stu-id="1ba3b-161">An email address</span></span>|
|<span data-ttu-id="1ba3b-162">id</span><span class="sxs-lookup"><span data-stu-id="1ba3b-162">id</span></span>|<span data-ttu-id="1ba3b-163">String</span><span class="sxs-lookup"><span data-stu-id="1ba3b-163">String</span></span>| <span data-ttu-id="1ba3b-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-164">Read-only.</span></span>|
|<span data-ttu-id="1ba3b-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="1ba3b-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="1ba3b-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ba3b-166">Boolean</span></span>|<span data-ttu-id="1ba3b-167">True は、このサービスを予約にお客様が利用できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="1ba3b-168">notes</span><span class="sxs-lookup"><span data-stu-id="1ba3b-168">notes</span></span>|<span data-ttu-id="1ba3b-169">String</span><span class="sxs-lookup"><span data-stu-id="1ba3b-169">String</span></span>|<span data-ttu-id="1ba3b-170">このサービスに関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-170">Additional information about this service.</span></span>|
|<span data-ttu-id="1ba3b-171">postBuffer</span><span class="sxs-lookup"><span data-stu-id="1ba3b-171">postBuffer</span></span>|<span data-ttu-id="1ba3b-172">期間</span><span class="sxs-lookup"><span data-stu-id="1ba3b-172">Duration</span></span>|<span data-ttu-id="1ba3b-173">このサービスの予定が終了してから、次の顧客の予定が予約されるまでの時間。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="1ba3b-174">preBuffer</span><span class="sxs-lookup"><span data-stu-id="1ba3b-174">preBuffer</span></span>|<span data-ttu-id="1ba3b-175">期間</span><span class="sxs-lookup"><span data-stu-id="1ba3b-175">Duration</span></span>|<span data-ttu-id="1ba3b-176">このサービスの予定を開始できるようになるまでの時間。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="1ba3b-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="1ba3b-177">schedulingPolicy</span></span>|[<span data-ttu-id="1ba3b-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="1ba3b-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="1ba3b-179">この種類のサービスの予定を作成および管理する方法を決定する一連のポリシー。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="1ba3b-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="1ba3b-180">staffMemberIds</span></span>|<span data-ttu-id="1ba3b-181">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1ba3b-181">String collection</span></span>|<span data-ttu-id="1ba3b-182">このサービスを提供する[スタッフメンバー](../resources/bookingstaffmember.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="1ba3b-183">応答</span><span class="sxs-lookup"><span data-stu-id="1ba3b-183">Response</span></span>
<span data-ttu-id="1ba3b-p106">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ba3b-186">例</span><span class="sxs-lookup"><span data-stu-id="1ba3b-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ba3b-187">要求</span><span class="sxs-lookup"><span data-stu-id="1ba3b-187">Request</span></span>
<span data-ttu-id="1ba3b-188">次の使用例は、指定されたサービスの期間を更新します。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-188">The following example updates the duration of the specified service.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1ba3b-189">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1ba3b-189">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ba3b-190">C#</span><span class="sxs-lookup"><span data-stu-id="1ba3b-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ba3b-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ba3b-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1ba3b-192">目的-C</span><span class="sxs-lookup"><span data-stu-id="1ba3b-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1ba3b-193">応答</span><span class="sxs-lookup"><span data-stu-id="1ba3b-193">Response</span></span>
<span data-ttu-id="1ba3b-194">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ba3b-194">The following is an example of the response.</span></span>
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
  ]
}
-->
