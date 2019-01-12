---
title: bookingService リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 790adf49cfda1f787665a48e1b06bd77da27e1f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925162"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="9bfff-104">bookingService リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9bfff-104">bookingService resource type</span></span>

 > <span data-ttu-id="9bfff-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9bfff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bfff-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9bfff-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="9bfff-107">[BookingBusiness](bookingbusiness.md)サービス名、価格、通常このようなサービスを提供するスタッフなどによって提供される特定のサービスに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-107">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="9bfff-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9bfff-108">Methods</span></span>

| <span data-ttu-id="9bfff-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9bfff-109">Method</span></span>           | <span data-ttu-id="9bfff-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9bfff-110">Return Type</span></span>    |<span data-ttu-id="9bfff-111">説明</span><span class="sxs-lookup"><span data-stu-id="9bfff-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9bfff-112">サービスの一覧</span><span class="sxs-lookup"><span data-stu-id="9bfff-112">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="9bfff-113">[bookingService](bookingservice.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9bfff-113">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="9bfff-114">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingService**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-114">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="9bfff-115">BookingService を作成します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-115">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="9bfff-116">bookingService</span><span class="sxs-lookup"><span data-stu-id="9bfff-116">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="9bfff-117">指定した[bookingbusiness](../resources/bookingbusiness.md)用の**bookingService**を作成します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-117">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="9bfff-118">BookingService を取得します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-118">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="9bfff-119">bookingService</span><span class="sxs-lookup"><span data-stu-id="9bfff-119">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="9bfff-120">指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 **bookingService**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-120">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="9bfff-121">Update</span><span class="sxs-lookup"><span data-stu-id="9bfff-121">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="9bfff-122">bookingService</span><span class="sxs-lookup"><span data-stu-id="9bfff-122">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="9bfff-123">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 **bookingService**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-123">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="9bfff-124">Delete</span><span class="sxs-lookup"><span data-stu-id="9bfff-124">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="9bfff-125">なし</span><span class="sxs-lookup"><span data-stu-id="9bfff-125">None</span></span> |<span data-ttu-id="9bfff-126">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 **bookingService**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-126">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="9bfff-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9bfff-127">Properties</span></span>
| <span data-ttu-id="9bfff-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9bfff-128">Property</span></span>     | <span data-ttu-id="9bfff-129">種類</span><span class="sxs-lookup"><span data-stu-id="9bfff-129">Type</span></span>   |<span data-ttu-id="9bfff-130">説明</span><span class="sxs-lookup"><span data-stu-id="9bfff-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bfff-131">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="9bfff-131">defaultDuration</span></span>|<span data-ttu-id="9bfff-132">Duration</span><span class="sxs-lookup"><span data-stu-id="9bfff-132">Duration</span></span>|<span data-ttu-id="9bfff-133">日、時間、分、秒単位の数値で表される、サービスの既定の長さです。</span><span class="sxs-lookup"><span data-stu-id="9bfff-133">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="9bfff-134">たとえば、P11D23H59M59.999999999999S です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-134">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="9bfff-135">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="9bfff-135">defaultLocation</span></span>|[<span data-ttu-id="9bfff-136">location</span><span class="sxs-lookup"><span data-stu-id="9bfff-136">location</span></span>](location.md)|<span data-ttu-id="9bfff-137">サービスの既定の物理的な場所です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-137">The default physical location for the service.</span></span>|
|<span data-ttu-id="9bfff-138">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="9bfff-138">defaultPrice</span></span>|<span data-ttu-id="9bfff-139">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="9bfff-139">Double</span></span>|<span data-ttu-id="9bfff-140">サービスの既定通貨の価格です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-140">The default monetary price for the service.</span></span>|
|<span data-ttu-id="9bfff-141">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="9bfff-141">defaultPriceType</span></span>|<span data-ttu-id="9bfff-142">文字列</span><span class="sxs-lookup"><span data-stu-id="9bfff-142">string</span></span>|<span data-ttu-id="9bfff-143">サービスの既定の方法に請求されます。</span><span class="sxs-lookup"><span data-stu-id="9bfff-143">The default way the service is charged.</span></span> <span data-ttu-id="9bfff-144">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-144">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="9bfff-145">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="9bfff-145">defaultReminders</span></span>|<span data-ttu-id="9bfff-146">[bookingReminder](bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9bfff-146">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="9bfff-147">このサービスの予定に対するアラームの既定値を設定します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-147">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="9bfff-148">その ID ではこの**bookingService**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="9bfff-148">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="9bfff-149">説明</span><span class="sxs-lookup"><span data-stu-id="9bfff-149">description</span></span>|<span data-ttu-id="9bfff-150">String</span><span class="sxs-lookup"><span data-stu-id="9bfff-150">String</span></span>|<span data-ttu-id="9bfff-151">サービスの説明です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-151">A text description for the service.</span></span>|
|<span data-ttu-id="9bfff-152">displayName</span><span class="sxs-lookup"><span data-stu-id="9bfff-152">displayName</span></span>|<span data-ttu-id="9bfff-153">String</span><span class="sxs-lookup"><span data-stu-id="9bfff-153">String</span></span>|<span data-ttu-id="9bfff-154">サービスの名前です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-154">A service name.</span></span>|
|<span data-ttu-id="9bfff-155">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9bfff-155">emailAddress</span></span>|<span data-ttu-id="9bfff-156">String</span><span class="sxs-lookup"><span data-stu-id="9bfff-156">String</span></span>|<span data-ttu-id="9bfff-157">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="9bfff-157">An email address</span></span>|
|<span data-ttu-id="9bfff-158">id</span><span class="sxs-lookup"><span data-stu-id="9bfff-158">id</span></span>|<span data-ttu-id="9bfff-159">String</span><span class="sxs-lookup"><span data-stu-id="9bfff-159">String</span></span>|<span data-ttu-id="9bfff-160">GUID 形式で、そのサービスの ID です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-160">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="9bfff-161">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-161">Read-only.</span></span>|
|<span data-ttu-id="9bfff-162">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="9bfff-162">isHiddenFromCustomers</span></span>|<span data-ttu-id="9bfff-163">ブール型</span><span class="sxs-lookup"><span data-stu-id="9bfff-163">Boolean</span></span>|<span data-ttu-id="9bfff-164">True は、このサービスは予約のお客様に利用できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-164">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="9bfff-165">notes</span><span class="sxs-lookup"><span data-stu-id="9bfff-165">notes</span></span>|<span data-ttu-id="9bfff-166">String</span><span class="sxs-lookup"><span data-stu-id="9bfff-166">String</span></span>|<span data-ttu-id="9bfff-167">このサービスに関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="9bfff-167">Additional information about this service.</span></span>|
|<span data-ttu-id="9bfff-168">事後バッファリング</span><span class="sxs-lookup"><span data-stu-id="9bfff-168">postBuffer</span></span>|<span data-ttu-id="9bfff-169">Duration</span><span class="sxs-lookup"><span data-stu-id="9bfff-169">Duration</span></span>|<span data-ttu-id="9bfff-170">このサービスの予定の後のバッファーに時間が終了して、次の前に顧客の予定が予約できます。</span><span class="sxs-lookup"><span data-stu-id="9bfff-170">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="9bfff-171">事前バッファリング</span><span class="sxs-lookup"><span data-stu-id="9bfff-171">preBuffer</span></span>|<span data-ttu-id="9bfff-172">Duration</span><span class="sxs-lookup"><span data-stu-id="9bfff-172">Duration</span></span>|<span data-ttu-id="9bfff-173">このサービスに対する予定を開始する前に、バッファーに格納する時間です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-173">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="9bfff-174">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="9bfff-174">schedulingPolicy</span></span>|[<span data-ttu-id="9bfff-175">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="9bfff-175">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="9bfff-176">この種類のサービスの予定を作成および管理する方法を決定するポリシーのセットです。</span><span class="sxs-lookup"><span data-stu-id="9bfff-176">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="9bfff-177">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="9bfff-177">staffMemberIds</span></span>|<span data-ttu-id="9bfff-178">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9bfff-178">String collection</span></span>|<span data-ttu-id="9bfff-179">このサービスを提供している[スタッフのメンバー](bookingstaffmember.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-179">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9bfff-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9bfff-180">Relationships</span></span>
<span data-ttu-id="9bfff-181">なし</span><span class="sxs-lookup"><span data-stu-id="9bfff-181">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9bfff-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9bfff-182">JSON representation</span></span>

<span data-ttu-id="9bfff-183">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-183">The following is a JSON representation of the resource.</span></span>

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
