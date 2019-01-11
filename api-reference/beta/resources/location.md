---
title: Location リソースの種類
description: イベントの場所の情報を表します。
localization_priority: Normal
ms.openlocfilehash: 650876596e2cf9336054957cfd4c95bf4dad16b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879402"
---
# <a name="location-resource-type"></a><span data-ttu-id="eb4a0-103">Location リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb4a0-103">Location resource type</span></span>

> <span data-ttu-id="eb4a0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb4a0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb4a0-106">[イベント](event.md)の場所の情報を表します。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-106">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="eb4a0-107">カレンダー内にイベントを作成するには、複数の方法があります。たとえば、アプリで[イベント作成](../api/user-post-events.md) REST API を使用するという方法、Outlook ユーザー インターフェイスを手動で使用するという方法などです。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-107">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="eb4a0-108">ユーザー インターフェイスを使用してイベントを作成する場合は、場所をプレーン テキストとして指定することも、Outlook、[Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/)、または [Bing ローカル検索](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/)で提供される会議室リストから選択して指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-108">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="eb4a0-109">イベントの作成方法によって、Outlook は読み取り専用の **locationType** プロパティを異なる方法で設定します。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-109">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="eb4a0-110">イベントの作成方法</span><span class="sxs-lookup"><span data-stu-id="eb4a0-110">How event was created</span></span>  | <span data-ttu-id="eb4a0-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb4a0-111">Property</span></span>   | <span data-ttu-id="eb4a0-112">予期される値</span><span class="sxs-lookup"><span data-stu-id="eb4a0-112">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="eb4a0-113">[イベント作成](../api/user-post-events.md) REST API</span><span class="sxs-lookup"><span data-stu-id="eb4a0-113">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="eb4a0-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="eb4a0-114">**locationType**</span></span> | `default` |
| <span data-ttu-id="eb4a0-115">Outlook のユーザー インターフェイス</span><span class="sxs-lookup"><span data-stu-id="eb4a0-115">User interface in Outlook</span></span> | <span data-ttu-id="eb4a0-116">**locationType**</span><span class="sxs-lookup"><span data-stu-id="eb4a0-116">**locationType**</span></span> | <span data-ttu-id="eb4a0-117">以下のいずれか:</span><span class="sxs-lookup"><span data-stu-id="eb4a0-117">One of the following:</span></span> <ul><li><span data-ttu-id="eb4a0-118">プレーン テキストとして入力された場所の場合は `default`。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-118">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="eb4a0-119">Outlook の会議室リストで提供された会議室の場合は `conferenceRoom`。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-119">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="eb4a0-120">Bing Autosuggest または Bing ローカル検索による場所の場合は、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress` のいずれか。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-120">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="eb4a0-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb4a0-121">Properties</span></span>
| <span data-ttu-id="eb4a0-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb4a0-122">Property</span></span>  | <span data-ttu-id="eb4a0-123">種類</span><span class="sxs-lookup"><span data-stu-id="eb4a0-123">Type</span></span>   | <span data-ttu-id="eb4a0-124">説明</span><span class="sxs-lookup"><span data-stu-id="eb4a0-124">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="eb4a0-125">address</span><span class="sxs-lookup"><span data-stu-id="eb4a0-125">address</span></span> | [<span data-ttu-id="eb4a0-126">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="eb4a0-126">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="eb4a0-127">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-127">The street address of the location.</span></span> |
| <span data-ttu-id="eb4a0-128">coordinates</span><span class="sxs-lookup"><span data-stu-id="eb4a0-128">coordinates</span></span> | [<span data-ttu-id="eb4a0-129">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="eb4a0-129">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="eb4a0-130">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-130">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="eb4a0-131">displayName</span><span class="sxs-lookup"><span data-stu-id="eb4a0-131">displayName</span></span>  | <span data-ttu-id="eb4a0-132">String</span><span class="sxs-lookup"><span data-stu-id="eb4a0-132">String</span></span> | <span data-ttu-id="eb4a0-133">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-133">The name associated with the location.</span></span>                       |
| <span data-ttu-id="eb4a0-134">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="eb4a0-134">locationEmailAddress</span></span> | <span data-ttu-id="eb4a0-135">String</span><span class="sxs-lookup"><span data-stu-id="eb4a0-135">String</span></span> | <span data-ttu-id="eb4a0-136">場所のメール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-136">Optional email address of the location.</span></span> |
| <span data-ttu-id="eb4a0-137">locationUri</span><span class="sxs-lookup"><span data-stu-id="eb4a0-137">locationUri</span></span> | <span data-ttu-id="eb4a0-138">String</span><span class="sxs-lookup"><span data-stu-id="eb4a0-138">String</span></span> | <span data-ttu-id="eb4a0-139">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-139">Optional URI representing the location.</span></span> |
| <span data-ttu-id="eb4a0-140">locationType</span><span class="sxs-lookup"><span data-stu-id="eb4a0-140">locationType</span></span> | <span data-ttu-id="eb4a0-141">String</span><span class="sxs-lookup"><span data-stu-id="eb4a0-141">String</span></span> | <span data-ttu-id="eb4a0-142">場所の種類。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-142">The type of location.</span></span> <span data-ttu-id="eb4a0-143">可能な値は、`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress` です。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-143">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="eb4a0-144">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-144">Read-only.</span></span>|
| <span data-ttu-id="eb4a0-145">uniqueId</span><span class="sxs-lookup"><span data-stu-id="eb4a0-145">uniqueId</span></span> | <span data-ttu-id="eb4a0-146">String</span><span class="sxs-lookup"><span data-stu-id="eb4a0-146">String</span></span> | <span data-ttu-id="eb4a0-147">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-147">For internal use only.</span></span>|
| <span data-ttu-id="eb4a0-148">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="eb4a0-148">uniqueIdType</span></span> | <span data-ttu-id="eb4a0-149">String</span><span class="sxs-lookup"><span data-stu-id="eb4a0-149">String</span></span> | <span data-ttu-id="eb4a0-150">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="eb4a0-150">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="eb4a0-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb4a0-151">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
