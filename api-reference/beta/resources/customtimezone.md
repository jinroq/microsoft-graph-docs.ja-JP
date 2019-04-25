---
title: customTimeZone リソースの種類
description: 標準時から夏時間またはその逆への切り替えが標準となっていないタイム ゾーンを表します。
localization_priority: Normal
ms.openlocfilehash: 0bb961e213956ef3142df1f3d55a83918a14fa78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543260"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="15c6c-103">customTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15c6c-103">customTimeZone resource type</span></span>

<span data-ttu-id="15c6c-104">標準時から夏時間またはその逆への切り替えが標準となっていないタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="15c6c-104">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="15c6c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15c6c-105">Properties</span></span>
| <span data-ttu-id="15c6c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15c6c-106">Property</span></span>     | <span data-ttu-id="15c6c-107">型</span><span class="sxs-lookup"><span data-stu-id="15c6c-107">Type</span></span>   |<span data-ttu-id="15c6c-108">説明</span><span class="sxs-lookup"><span data-stu-id="15c6c-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15c6c-109">bias</span><span class="sxs-lookup"><span data-stu-id="15c6c-109">bias</span></span> | <span data-ttu-id="15c6c-110">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="15c6c-110">Edm.Int32</span></span> | <span data-ttu-id="15c6c-111">タイム ゾーンの協定世界時 (UTC) からの時間オフセットです。</span><span class="sxs-lookup"><span data-stu-id="15c6c-111">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="15c6c-112">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="15c6c-112">This value is in minutes.</span></span><span data-ttu-id="15c6c-113">UTC より時間が進んでいるタイム　ゾーンには正のオフセット、UTC より時間が遅れているタイム ゾーンには負のオフセットを設定します。</span><span class="sxs-lookup"><span data-stu-id="15c6c-113"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="15c6c-114">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="15c6c-114">daylightOffset</span></span> | [<span data-ttu-id="15c6c-115">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="15c6c-115">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="15c6c-116">タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="15c6c-116">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="15c6c-117">name</span><span class="sxs-lookup"><span data-stu-id="15c6c-117">name</span></span> | <span data-ttu-id="15c6c-118">string</span><span class="sxs-lookup"><span data-stu-id="15c6c-118">string</span></span> | <span data-ttu-id="15c6c-119">カスタム タイム ゾーンの名前。</span><span class="sxs-lookup"><span data-stu-id="15c6c-119">The name of the custom time zone.</span></span> |
| <span data-ttu-id="15c6c-120">standardOffset</span><span class="sxs-lookup"><span data-stu-id="15c6c-120">standardOffset</span></span> | [<span data-ttu-id="15c6c-121">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="15c6c-121">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="15c6c-122">タイム ゾーンが夏時間から標準時に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="15c6c-122">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="15c6c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15c6c-123">JSON representation</span></span>

<span data-ttu-id="15c6c-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15c6c-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
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
