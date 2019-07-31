---
title: bookingService リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5f51ec999f0a2048b8dbcbdd533c609eb5a86757
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974130"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="cbfe1-104">bookingService リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbfe1-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="cbfe1-105">通常はサービスを提供しているサービス名、価格、スタッフなど、 [Bookingbusiness](bookingbusiness.md)によって提供される特定のサービスに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="cbfe1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbfe1-106">Methods</span></span>

| <span data-ttu-id="cbfe1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbfe1-107">Method</span></span>           | <span data-ttu-id="cbfe1-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cbfe1-108">Return Type</span></span>    |<span data-ttu-id="cbfe1-109">説明</span><span class="sxs-lookup"><span data-stu-id="cbfe1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbfe1-110">サービスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cbfe1-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="cbfe1-111">[Bookingservice](bookingservice.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfe1-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="cbfe1-112">指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="cbfe1-113">BookingService の作成</span><span class="sxs-lookup"><span data-stu-id="cbfe1-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="cbfe1-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="cbfe1-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="cbfe1-115">指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**を作成します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="cbfe1-116">BookingService を取得する</span><span class="sxs-lookup"><span data-stu-id="cbfe1-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="cbfe1-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="cbfe1-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="cbfe1-118">指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="cbfe1-119">Update</span><span class="sxs-lookup"><span data-stu-id="cbfe1-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="cbfe1-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="cbfe1-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="cbfe1-121">指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="cbfe1-122">Delete</span><span class="sxs-lookup"><span data-stu-id="cbfe1-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="cbfe1-123">None</span><span class="sxs-lookup"><span data-stu-id="cbfe1-123">None</span></span> |<span data-ttu-id="cbfe1-124">指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="cbfe1-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbfe1-125">Properties</span></span>
| <span data-ttu-id="cbfe1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbfe1-126">Property</span></span>     | <span data-ttu-id="cbfe1-127">型</span><span class="sxs-lookup"><span data-stu-id="cbfe1-127">Type</span></span>   |<span data-ttu-id="cbfe1-128">説明</span><span class="sxs-lookup"><span data-stu-id="cbfe1-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbfe1-129">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="cbfe1-129">defaultDuration</span></span>|<span data-ttu-id="cbfe1-130">期間</span><span class="sxs-lookup"><span data-stu-id="cbfe1-130">Duration</span></span>|<span data-ttu-id="cbfe1-131">サービスの既定の長さ。日数、時間、分、および秒で表されます。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="cbfe1-132">たとえば、P11D23H59M 59.999999999999 S のようになります。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="cbfe1-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="cbfe1-133">defaultLocation</span></span>|[<span data-ttu-id="cbfe1-134">location</span><span class="sxs-lookup"><span data-stu-id="cbfe1-134">location</span></span>](location.md)|<span data-ttu-id="cbfe1-135">サービスの既定の物理的な場所。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="cbfe1-136">既定の価格</span><span class="sxs-lookup"><span data-stu-id="cbfe1-136">defaultPrice</span></span>|<span data-ttu-id="cbfe1-137">2 行分</span><span class="sxs-lookup"><span data-stu-id="cbfe1-137">Double</span></span>|<span data-ttu-id="cbfe1-138">サービスの既定の通貨料金。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="cbfe1-139">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="cbfe1-139">defaultPriceType</span></span>|<span data-ttu-id="cbfe1-140">string</span><span class="sxs-lookup"><span data-stu-id="cbfe1-140">string</span></span>|<span data-ttu-id="cbfe1-141">サービスの既定の課金方法。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-141">The default way the service is charged.</span></span> <span data-ttu-id="cbfe1-142">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="cbfe1-143">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="cbfe1-143">defaultReminders</span></span>|<span data-ttu-id="cbfe1-144">[Bookingreminder](bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfe1-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="cbfe1-145">このサービスの予定に対する既定のアラームのセット。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="cbfe1-146">このプロパティの値は、この**Bookingservice**を ID で読み取る場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="cbfe1-147">description</span><span class="sxs-lookup"><span data-stu-id="cbfe1-147">description</span></span>|<span data-ttu-id="cbfe1-148">String</span><span class="sxs-lookup"><span data-stu-id="cbfe1-148">String</span></span>|<span data-ttu-id="cbfe1-149">サービスのテキストの説明。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-149">A text description for the service.</span></span>|
|<span data-ttu-id="cbfe1-150">displayName</span><span class="sxs-lookup"><span data-stu-id="cbfe1-150">displayName</span></span>|<span data-ttu-id="cbfe1-151">String</span><span class="sxs-lookup"><span data-stu-id="cbfe1-151">String</span></span>|<span data-ttu-id="cbfe1-152">サービス名。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-152">A service name.</span></span>|
|<span data-ttu-id="cbfe1-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cbfe1-153">emailAddress</span></span>|<span data-ttu-id="cbfe1-154">String</span><span class="sxs-lookup"><span data-stu-id="cbfe1-154">String</span></span>|<span data-ttu-id="cbfe1-155">電子メールアドレス</span><span class="sxs-lookup"><span data-stu-id="cbfe1-155">An email address</span></span>|
|<span data-ttu-id="cbfe1-156">id</span><span class="sxs-lookup"><span data-stu-id="cbfe1-156">id</span></span>|<span data-ttu-id="cbfe1-157">文字列</span><span class="sxs-lookup"><span data-stu-id="cbfe1-157">String</span></span>|<span data-ttu-id="cbfe1-158">GUID 形式の、そのサービスの ID。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="cbfe1-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-159">Read-only.</span></span>|
|<span data-ttu-id="cbfe1-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="cbfe1-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="cbfe1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbfe1-161">Boolean</span></span>|<span data-ttu-id="cbfe1-162">True は、このサービスを予約にお客様が利用できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="cbfe1-163">notes</span><span class="sxs-lookup"><span data-stu-id="cbfe1-163">notes</span></span>|<span data-ttu-id="cbfe1-164">String</span><span class="sxs-lookup"><span data-stu-id="cbfe1-164">String</span></span>|<span data-ttu-id="cbfe1-165">このサービスに関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-165">Additional information about this service.</span></span>|
|<span data-ttu-id="cbfe1-166">postBuffer</span><span class="sxs-lookup"><span data-stu-id="cbfe1-166">postBuffer</span></span>|<span data-ttu-id="cbfe1-167">期間</span><span class="sxs-lookup"><span data-stu-id="cbfe1-167">Duration</span></span>|<span data-ttu-id="cbfe1-168">このサービスの予定が終了してから、次の顧客の予定が予約されるまでの時間。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="cbfe1-169">preBuffer</span><span class="sxs-lookup"><span data-stu-id="cbfe1-169">preBuffer</span></span>|<span data-ttu-id="cbfe1-170">期間</span><span class="sxs-lookup"><span data-stu-id="cbfe1-170">Duration</span></span>|<span data-ttu-id="cbfe1-171">このサービスの予定を開始できるようになるまでの時間。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="cbfe1-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="cbfe1-172">schedulingPolicy</span></span>|[<span data-ttu-id="cbfe1-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="cbfe1-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="cbfe1-174">この種類のサービスの予定を作成および管理する方法を決定する一連のポリシー。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="cbfe1-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="cbfe1-175">staffMemberIds</span></span>|<span data-ttu-id="cbfe1-176">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="cbfe1-176">String collection</span></span>|<span data-ttu-id="cbfe1-177">このサービスを提供する[スタッフメンバー](bookingstaffmember.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cbfe1-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbfe1-178">Relationships</span></span>
<span data-ttu-id="cbfe1-179">なし</span><span class="sxs-lookup"><span data-stu-id="cbfe1-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cbfe1-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbfe1-180">JSON representation</span></span>

<span data-ttu-id="cbfe1-181">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cbfe1-181">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
