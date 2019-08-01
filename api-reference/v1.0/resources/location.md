---
title: Location リソースの種類
description: イベントの場所の情報を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bb975753e838d273c8d516472f1963d92413a367
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036429"
---
# <a name="location-resource-type"></a><span data-ttu-id="02f37-103">Location リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02f37-103">Location resource type</span></span>

<span data-ttu-id="02f37-104">[イベント](event.md)の場所の情報を表します。</span><span class="sxs-lookup"><span data-stu-id="02f37-104">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="02f37-105">カレンダー内にイベントを作成するには、複数の方法があります。たとえば、アプリで[イベント作成](../api/user-post-events.md) REST API を使用するという方法、Outlook ユーザー インターフェイスを手動で使用するという方法などです。</span><span class="sxs-lookup"><span data-stu-id="02f37-105">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="02f37-106">ユーザー インターフェイスを使用してイベントを作成する場合は、場所をプレーン テキストとして指定することも、Outlook、[Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/)、または [Bing ローカル検索](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/)で提供される会議室リストから選択して指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="02f37-106">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="02f37-107">イベントの作成方法によって、Outlook は読み取り専用の **locationType** プロパティを異なる方法で設定します。</span><span class="sxs-lookup"><span data-stu-id="02f37-107">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="02f37-108">イベントの作成方法</span><span class="sxs-lookup"><span data-stu-id="02f37-108">How event was created</span></span>  | <span data-ttu-id="02f37-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02f37-109">Property</span></span>   | <span data-ttu-id="02f37-110">予期される値</span><span class="sxs-lookup"><span data-stu-id="02f37-110">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="02f37-111">[イベント作成](../api/user-post-events.md) REST API</span><span class="sxs-lookup"><span data-stu-id="02f37-111">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="02f37-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="02f37-112">**locationType**</span></span> | `default` |
| <span data-ttu-id="02f37-113">Outlook のユーザー インターフェイス</span><span class="sxs-lookup"><span data-stu-id="02f37-113">User interface in Outlook</span></span> | <span data-ttu-id="02f37-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="02f37-114">**locationType**</span></span> | <span data-ttu-id="02f37-115">以下のいずれか:</span><span class="sxs-lookup"><span data-stu-id="02f37-115">One of the following:</span></span> <ul><li><span data-ttu-id="02f37-116">プレーン テキストとして入力された場所の場合は `default`。</span><span class="sxs-lookup"><span data-stu-id="02f37-116">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="02f37-117">Outlook の会議室リストで提供された会議室の場合は `conferenceRoom`。</span><span class="sxs-lookup"><span data-stu-id="02f37-117">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="02f37-118">Bing Autosuggest または Bing ローカル検索による場所の場合は、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress` のいずれか。</span><span class="sxs-lookup"><span data-stu-id="02f37-118">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="02f37-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02f37-119">Properties</span></span>
| <span data-ttu-id="02f37-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02f37-120">Property</span></span>  | <span data-ttu-id="02f37-121">型</span><span class="sxs-lookup"><span data-stu-id="02f37-121">Type</span></span>   | <span data-ttu-id="02f37-122">説明</span><span class="sxs-lookup"><span data-stu-id="02f37-122">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="02f37-123">address</span><span class="sxs-lookup"><span data-stu-id="02f37-123">address</span></span> | [<span data-ttu-id="02f37-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="02f37-124">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="02f37-125">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="02f37-125">The street address of the location.</span></span> |
| <span data-ttu-id="02f37-126">coordinates</span><span class="sxs-lookup"><span data-stu-id="02f37-126">coordinates</span></span> | [<span data-ttu-id="02f37-127">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="02f37-127">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="02f37-128">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="02f37-128">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="02f37-129">displayName</span><span class="sxs-lookup"><span data-stu-id="02f37-129">displayName</span></span>  | <span data-ttu-id="02f37-130">String</span><span class="sxs-lookup"><span data-stu-id="02f37-130">String</span></span> | <span data-ttu-id="02f37-131">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="02f37-131">The name associated with the location.</span></span>                       |
| <span data-ttu-id="02f37-132">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="02f37-132">locationEmailAddress</span></span> | <span data-ttu-id="02f37-133">String</span><span class="sxs-lookup"><span data-stu-id="02f37-133">String</span></span> | <span data-ttu-id="02f37-134">場所のメール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="02f37-134">Optional email address of the location.</span></span>              |
| <span data-ttu-id="02f37-135">locationUri</span><span class="sxs-lookup"><span data-stu-id="02f37-135">locationUri</span></span> | <span data-ttu-id="02f37-136">String</span><span class="sxs-lookup"><span data-stu-id="02f37-136">String</span></span> | <span data-ttu-id="02f37-137">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="02f37-137">Optional URI representing the location.</span></span> |
| <span data-ttu-id="02f37-138">locationType</span><span class="sxs-lookup"><span data-stu-id="02f37-138">locationType</span></span> | <span data-ttu-id="02f37-139">locationType</span><span class="sxs-lookup"><span data-stu-id="02f37-139">locationType</span></span> | <span data-ttu-id="02f37-140">場所の種類。</span><span class="sxs-lookup"><span data-stu-id="02f37-140">The type of location.</span></span> <span data-ttu-id="02f37-141">使用可能な値は`default`、 `conferenceRoom`、 `homeAddress` `businessAddress``geoCoordinates` `streetAddress` `hotel` `restaurant`、、、、、、、 `postalAddress`、です。 `localBusiness`</span><span class="sxs-lookup"><span data-stu-id="02f37-141">The possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="02f37-142">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="02f37-142">Read-only.</span></span>|
| <span data-ttu-id="02f37-143">uniqueId</span><span class="sxs-lookup"><span data-stu-id="02f37-143">uniqueId</span></span> | <span data-ttu-id="02f37-144">String</span><span class="sxs-lookup"><span data-stu-id="02f37-144">String</span></span> | <span data-ttu-id="02f37-145">内部使用のために用意されています。</span><span class="sxs-lookup"><span data-stu-id="02f37-145">For internal use only.</span></span>|
| <span data-ttu-id="02f37-146">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="02f37-146">uniqueIdType</span></span> | <span data-ttu-id="02f37-147">locationUniqueIdType</span><span class="sxs-lookup"><span data-stu-id="02f37-147">locationUniqueIdType</span></span> | <span data-ttu-id="02f37-148">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="02f37-148">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02f37-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02f37-149">JSON representation</span></span>

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
