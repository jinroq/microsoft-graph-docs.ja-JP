---
title: customTimeZone リソースの種類
description: 標準時から夏時間またはその逆への切り替えが標準となっていないタイム ゾーンを表します。
localization_priority: Normal
ms.openlocfilehash: bad1a190581592d2d9465284bf8ab1c41fe2370a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818276"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="057f1-103">customTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="057f1-103">customTimeZone resource type</span></span>

> <span data-ttu-id="057f1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="057f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="057f1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="057f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="057f1-106">標準時から夏時間またはその逆への切り替えが標準となっていないタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="057f1-106">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="057f1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="057f1-107">Properties</span></span>
| <span data-ttu-id="057f1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="057f1-108">Property</span></span>     | <span data-ttu-id="057f1-109">種類</span><span class="sxs-lookup"><span data-stu-id="057f1-109">Type</span></span>   |<span data-ttu-id="057f1-110">説明</span><span class="sxs-lookup"><span data-stu-id="057f1-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="057f1-111">bias</span><span class="sxs-lookup"><span data-stu-id="057f1-111">bias</span></span> | <span data-ttu-id="057f1-112">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="057f1-112">Edm.Int32</span></span> | <span data-ttu-id="057f1-113">タイム ゾーンの協定世界時 (UTC) からの時間オフセットです。</span><span class="sxs-lookup"><span data-stu-id="057f1-113">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="057f1-114">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="057f1-114">This value is in minutes.</span></span><span data-ttu-id="057f1-115">UTC より時間が進んでいるタイム　ゾーンには正のオフセット、UTC より時間が遅れているタイム ゾーンには負のオフセットを設定します。</span><span class="sxs-lookup"><span data-stu-id="057f1-115"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="057f1-116">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="057f1-116">daylightOffset</span></span> | [<span data-ttu-id="057f1-117">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="057f1-117">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="057f1-118">タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="057f1-118">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="057f1-119">name</span><span class="sxs-lookup"><span data-stu-id="057f1-119">name</span></span> | <span data-ttu-id="057f1-120">文字列</span><span class="sxs-lookup"><span data-stu-id="057f1-120">string</span></span> | <span data-ttu-id="057f1-121">カスタム タイム ゾーンの名前。</span><span class="sxs-lookup"><span data-stu-id="057f1-121">The name of the custom time zone.</span></span> |
| <span data-ttu-id="057f1-122">standardOffset</span><span class="sxs-lookup"><span data-stu-id="057f1-122">standardOffset</span></span> | [<span data-ttu-id="057f1-123">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="057f1-123">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="057f1-124">タイム ゾーンが夏時間から標準時に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="057f1-124">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="057f1-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="057f1-125">JSON representation</span></span>

<span data-ttu-id="057f1-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="057f1-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
