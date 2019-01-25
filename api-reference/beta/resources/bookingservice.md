---
title: bookingService リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519886"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="fb9e9-104">bookingService リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb9e9-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="fb9e9-105">[BookingBusiness](bookingbusiness.md)サービス名、価格、通常このようなサービスを提供するスタッフなどによって提供される特定のサービスに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="fb9e9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="fb9e9-106">Methods</span></span>

| <span data-ttu-id="fb9e9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fb9e9-107">Method</span></span>           | <span data-ttu-id="fb9e9-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fb9e9-108">Return Type</span></span>    |<span data-ttu-id="fb9e9-109">説明</span><span class="sxs-lookup"><span data-stu-id="fb9e9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb9e9-110">サービスの一覧</span><span class="sxs-lookup"><span data-stu-id="fb9e9-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="fb9e9-111">[bookingService](bookingservice.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fb9e9-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="fb9e9-112">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingService**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="fb9e9-113">BookingService を作成します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="fb9e9-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="fb9e9-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="fb9e9-115">指定した[bookingbusiness](../resources/bookingbusiness.md)用の**bookingService**を作成します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="fb9e9-116">BookingService を取得します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="fb9e9-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="fb9e9-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="fb9e9-118">指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 **bookingService**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="fb9e9-119">Update</span><span class="sxs-lookup"><span data-stu-id="fb9e9-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="fb9e9-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="fb9e9-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="fb9e9-121">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 **bookingService**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="fb9e9-122">Delete</span><span class="sxs-lookup"><span data-stu-id="fb9e9-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="fb9e9-123">なし</span><span class="sxs-lookup"><span data-stu-id="fb9e9-123">None</span></span> |<span data-ttu-id="fb9e9-124">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 **bookingService**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="fb9e9-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb9e9-125">Properties</span></span>
| <span data-ttu-id="fb9e9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb9e9-126">Property</span></span>     | <span data-ttu-id="fb9e9-127">型</span><span class="sxs-lookup"><span data-stu-id="fb9e9-127">Type</span></span>   |<span data-ttu-id="fb9e9-128">説明</span><span class="sxs-lookup"><span data-stu-id="fb9e9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb9e9-129">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="fb9e9-129">defaultDuration</span></span>|<span data-ttu-id="fb9e9-130">Duration</span><span class="sxs-lookup"><span data-stu-id="fb9e9-130">Duration</span></span>|<span data-ttu-id="fb9e9-131">日、時間、分、秒単位の数値で表される、サービスの既定の長さです。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="fb9e9-132">たとえば、P11D23H59M59.999999999999S です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="fb9e9-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="fb9e9-133">defaultLocation</span></span>|[<span data-ttu-id="fb9e9-134">location</span><span class="sxs-lookup"><span data-stu-id="fb9e9-134">location</span></span>](location.md)|<span data-ttu-id="fb9e9-135">サービスの既定の物理的な場所です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="fb9e9-136">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="fb9e9-136">defaultPrice</span></span>|<span data-ttu-id="fb9e9-137">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="fb9e9-137">Double</span></span>|<span data-ttu-id="fb9e9-138">サービスの既定通貨の価格です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="fb9e9-139">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="fb9e9-139">defaultPriceType</span></span>|<span data-ttu-id="fb9e9-140">string</span><span class="sxs-lookup"><span data-stu-id="fb9e9-140">string</span></span>|<span data-ttu-id="fb9e9-141">サービスの既定の方法に請求されます。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-141">The default way the service is charged.</span></span> <span data-ttu-id="fb9e9-142">可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="fb9e9-143">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="fb9e9-143">defaultReminders</span></span>|<span data-ttu-id="fb9e9-144">[bookingReminder](bookingreminder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fb9e9-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="fb9e9-145">このサービスの予定に対するアラームの既定値を設定します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="fb9e9-146">その ID ではこの**bookingService**を読み取るときにのみ、このプロパティの値があります。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="fb9e9-147">説明</span><span class="sxs-lookup"><span data-stu-id="fb9e9-147">description</span></span>|<span data-ttu-id="fb9e9-148">文字列</span><span class="sxs-lookup"><span data-stu-id="fb9e9-148">String</span></span>|<span data-ttu-id="fb9e9-149">サービスの説明です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-149">A text description for the service.</span></span>|
|<span data-ttu-id="fb9e9-150">displayName</span><span class="sxs-lookup"><span data-stu-id="fb9e9-150">displayName</span></span>|<span data-ttu-id="fb9e9-151">String</span><span class="sxs-lookup"><span data-stu-id="fb9e9-151">String</span></span>|<span data-ttu-id="fb9e9-152">サービスの名前です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-152">A service name.</span></span>|
|<span data-ttu-id="fb9e9-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fb9e9-153">emailAddress</span></span>|<span data-ttu-id="fb9e9-154">String</span><span class="sxs-lookup"><span data-stu-id="fb9e9-154">String</span></span>|<span data-ttu-id="fb9e9-155">電子メール アドレス:  </span><span class="sxs-lookup"><span data-stu-id="fb9e9-155">An email address</span></span>|
|<span data-ttu-id="fb9e9-156">id</span><span class="sxs-lookup"><span data-stu-id="fb9e9-156">id</span></span>|<span data-ttu-id="fb9e9-157">文字列</span><span class="sxs-lookup"><span data-stu-id="fb9e9-157">String</span></span>|<span data-ttu-id="fb9e9-158">GUID 形式で、そのサービスの ID です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="fb9e9-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-159">Read-only.</span></span>|
|<span data-ttu-id="fb9e9-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="fb9e9-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="fb9e9-161">ブール値</span><span class="sxs-lookup"><span data-stu-id="fb9e9-161">Boolean</span></span>|<span data-ttu-id="fb9e9-162">True は、このサービスは予約のお客様に利用できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="fb9e9-163">notes</span><span class="sxs-lookup"><span data-stu-id="fb9e9-163">notes</span></span>|<span data-ttu-id="fb9e9-164">String</span><span class="sxs-lookup"><span data-stu-id="fb9e9-164">String</span></span>|<span data-ttu-id="fb9e9-165">このサービスに関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-165">Additional information about this service.</span></span>|
|<span data-ttu-id="fb9e9-166">事後バッファリング</span><span class="sxs-lookup"><span data-stu-id="fb9e9-166">postBuffer</span></span>|<span data-ttu-id="fb9e9-167">Duration</span><span class="sxs-lookup"><span data-stu-id="fb9e9-167">Duration</span></span>|<span data-ttu-id="fb9e9-168">このサービスの予定の後のバッファーに時間が終了して、次の前に顧客の予定が予約できます。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="fb9e9-169">事前バッファリング</span><span class="sxs-lookup"><span data-stu-id="fb9e9-169">preBuffer</span></span>|<span data-ttu-id="fb9e9-170">Duration</span><span class="sxs-lookup"><span data-stu-id="fb9e9-170">Duration</span></span>|<span data-ttu-id="fb9e9-171">このサービスに対する予定を開始する前に、バッファーに格納する時間です。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="fb9e9-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="fb9e9-172">schedulingPolicy</span></span>|[<span data-ttu-id="fb9e9-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="fb9e9-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="fb9e9-174">この種類のサービスの予定を作成および管理する方法を決定するポリシーのセットです。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="fb9e9-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="fb9e9-175">staffMemberIds</span></span>|<span data-ttu-id="fb9e9-176">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fb9e9-176">String collection</span></span>|<span data-ttu-id="fb9e9-177">このサービスを提供している[スタッフのメンバー](bookingstaffmember.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fb9e9-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fb9e9-178">Relationships</span></span>
<span data-ttu-id="fb9e9-179">なし</span><span class="sxs-lookup"><span data-stu-id="fb9e9-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fb9e9-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb9e9-180">JSON representation</span></span>

<span data-ttu-id="fb9e9-181">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb9e9-181">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
