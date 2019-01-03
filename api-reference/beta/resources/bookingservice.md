---
title: bookingService リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: bb42768cb913abca7c17e6d617670a3a035ec16a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067822"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="90268-104">bookingService リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90268-104">bookingService resource type</span></span>

 > <span data-ttu-id="90268-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90268-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90268-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90268-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="90268-107">[BookingBusiness](bookingbusiness.md)サービス名、価格、通常このようなサービスを提供するスタッフなどによって提供される特定のサービスに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="90268-107">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="90268-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="90268-108">Methods</span></span>

| <span data-ttu-id="90268-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="90268-109">Method</span></span>           | <span data-ttu-id="90268-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="90268-110">Return Type</span></span>    |<span data-ttu-id="90268-111">説明</span><span class="sxs-lookup"><span data-stu-id="90268-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90268-112">サービスの一覧</span><span class="sxs-lookup"><span data-stu-id="90268-112">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="90268-113">[bookingService](bookingservice.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="90268-113">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="90268-114">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingService**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="90268-114">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="90268-115">BookingService を作成します。</span><span class="sxs-lookup"><span data-stu-id="90268-115">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="90268-116">bookingService</span><span class="sxs-lookup"><span data-stu-id="90268-116">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="90268-117">指定した[bookingbusiness](../resources/bookingbusiness.md)用の**bookingService**を作成します。</span><span class="sxs-lookup"><span data-stu-id="90268-117">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="90268-118">BookingService を取得します。</span><span class="sxs-lookup"><span data-stu-id="90268-118">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="90268-119">bookingService</span><span class="sxs-lookup"><span data-stu-id="90268-119">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="90268-120">指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 **bookingService**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="90268-120">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="90268-121">Update</span><span class="sxs-lookup"><span data-stu-id="90268-121">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="90268-122">bookingService</span><span class="sxs-lookup"><span data-stu-id="90268-122">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="90268-123">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 **bookingService**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="90268-123">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="90268-124">削除</span><span class="sxs-lookup"><span data-stu-id="90268-124">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="90268-125">なし</span><span class="sxs-lookup"><span data-stu-id="90268-125">None</span></span> |<span data-ttu-id="90268-126">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 **bookingService**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="90268-126">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="90268-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90268-127">Properties</span></span>
| <span data-ttu-id="90268-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90268-128">Property</span></span>     | <span data-ttu-id="90268-129">型</span><span class="sxs-lookup"><span data-stu-id="90268-129">Type</span></span>   |<span data-ttu-id="90268-130">説明</span><span class="sxs-lookup"><span data-stu-id="90268-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90268-131">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="90268-131">defaultDuration</span></span>|<span data-ttu-id="90268-132">Duration</span><span class="sxs-lookup"><span data-stu-id="90268-132">Duration</span></span>|<span data-ttu-id="90268-133">日、時間、分、秒単位の数値で表される、サービスの既定の長さです。</span><span class="sxs-lookup"><span data-stu-id="90268-133">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="90268-134">たとえば、P11D23H59M59.999999999999S です。</span><span class="sxs-lookup"><span data-stu-id="90268-134">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="90268-135">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="90268-135">defaultLocation</span></span>|[<span data-ttu-id="90268-136">location</span><span class="sxs-lookup"><span data-stu-id="90268-136">location</span></span>](location.md)|<span data-ttu-id="90268-137">サービスの既定の物理的な場所です。</span><span class="sxs-lookup"><span data-stu-id="90268-137">The default physical location for the service.</span></span>|
|<span data-ttu-id="90268-138">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="90268-138">defaultPrice</span></span>|<span data-ttu-id="90268-139">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="90268-139">Double</span></span>|<span data-ttu-id="90268-140">サービスの既定通貨の価格です。</span><span class="sxs-lookup"><span data-stu-id="90268-140">The default monetary price for the service.</span></span>|
|<span data-ttu-id="90268-141">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="90268-141">defaultPriceType</span></span>|<span data-ttu-id="90268-142">文字列</span><span class="sxs-lookup"><span data-stu-id="90268-142">string</span></span>|<span data-ttu-id="90268-143">サービスの既定の方法に請求されます。</span><span class="sxs-lookup"><span data-stu-id="90268-143">The default way the service is charged.</span></span> <span data-ttu-id="90268-144">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="90268-144">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="90268-145">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="90268-145">defaultReminders</span></span>|<span data-ttu-id="90268-146">[bookingReminder](bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="90268-146">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="90268-147">このサービスの予定に対するアラームの既定値を設定します。</span><span class="sxs-lookup"><span data-stu-id="90268-147">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="90268-148">その ID ではこの**bookingService**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="90268-148">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="90268-149">説明</span><span class="sxs-lookup"><span data-stu-id="90268-149">description</span></span>|<span data-ttu-id="90268-150">String</span><span class="sxs-lookup"><span data-stu-id="90268-150">String</span></span>|<span data-ttu-id="90268-151">サービスの説明です。</span><span class="sxs-lookup"><span data-stu-id="90268-151">A text description for the service.</span></span>|
|<span data-ttu-id="90268-152">displayName</span><span class="sxs-lookup"><span data-stu-id="90268-152">displayName</span></span>|<span data-ttu-id="90268-153">String</span><span class="sxs-lookup"><span data-stu-id="90268-153">String</span></span>|<span data-ttu-id="90268-154">サービスの名前です。</span><span class="sxs-lookup"><span data-stu-id="90268-154">A service name.</span></span>|
|<span data-ttu-id="90268-155">emailAddress</span><span class="sxs-lookup"><span data-stu-id="90268-155">emailAddress</span></span>|<span data-ttu-id="90268-156">String</span><span class="sxs-lookup"><span data-stu-id="90268-156">String</span></span>|<span data-ttu-id="90268-157">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="90268-157">An email address</span></span>|
|<span data-ttu-id="90268-158">id</span><span class="sxs-lookup"><span data-stu-id="90268-158">id</span></span>|<span data-ttu-id="90268-159">String</span><span class="sxs-lookup"><span data-stu-id="90268-159">String</span></span>|<span data-ttu-id="90268-160">GUID 形式で、そのサービスの ID です。</span><span class="sxs-lookup"><span data-stu-id="90268-160">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="90268-161">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="90268-161">Read-only.</span></span>|
|<span data-ttu-id="90268-162">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="90268-162">isHiddenFromCustomers</span></span>|<span data-ttu-id="90268-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="90268-163">Boolean</span></span>|<span data-ttu-id="90268-164">True は、このサービスは予約のお客様に利用できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="90268-164">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="90268-165">notes</span><span class="sxs-lookup"><span data-stu-id="90268-165">notes</span></span>|<span data-ttu-id="90268-166">String</span><span class="sxs-lookup"><span data-stu-id="90268-166">String</span></span>|<span data-ttu-id="90268-167">このサービスに関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="90268-167">Additional information about this service.</span></span>|
|<span data-ttu-id="90268-168">事後バッファリング</span><span class="sxs-lookup"><span data-stu-id="90268-168">postBuffer</span></span>|<span data-ttu-id="90268-169">Duration</span><span class="sxs-lookup"><span data-stu-id="90268-169">Duration</span></span>|<span data-ttu-id="90268-170">このサービスの予定の後のバッファーに時間が終了して、次の前に顧客の予定が予約できます。</span><span class="sxs-lookup"><span data-stu-id="90268-170">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="90268-171">事前バッファリング</span><span class="sxs-lookup"><span data-stu-id="90268-171">preBuffer</span></span>|<span data-ttu-id="90268-172">Duration</span><span class="sxs-lookup"><span data-stu-id="90268-172">Duration</span></span>|<span data-ttu-id="90268-173">このサービスに対する予定を開始する前に、バッファーに格納する時間です。</span><span class="sxs-lookup"><span data-stu-id="90268-173">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="90268-174">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="90268-174">schedulingPolicy</span></span>|[<span data-ttu-id="90268-175">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="90268-175">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="90268-176">この種類のサービスの予定を作成および管理する方法を決定するポリシーのセットです。</span><span class="sxs-lookup"><span data-stu-id="90268-176">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="90268-177">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="90268-177">staffMemberIds</span></span>|<span data-ttu-id="90268-178">String コレクション</span><span class="sxs-lookup"><span data-stu-id="90268-178">String collection</span></span>|<span data-ttu-id="90268-179">このサービスを提供している[スタッフのメンバー](bookingstaffmember.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="90268-179">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="90268-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="90268-180">Relationships</span></span>
<span data-ttu-id="90268-181">なし</span><span class="sxs-lookup"><span data-stu-id="90268-181">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="90268-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90268-182">JSON representation</span></span>

<span data-ttu-id="90268-183">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="90268-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->