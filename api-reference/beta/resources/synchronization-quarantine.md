---
title: 同期検疫リソースの種類
description: 同期ジョブの検疫状態に関する情報を提供します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d63082dbe4e8e952d41032a74467cd4c301a857b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964705"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="37ee6-103">同期検疫リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37ee6-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37ee6-104">[同期ジョブ](synchronization-synchronizationjob.md)の検疫状態に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="37ee6-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="37ee6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37ee6-105">Properties</span></span>
| <span data-ttu-id="37ee6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37ee6-106">Property</span></span>     | <span data-ttu-id="37ee6-107">型</span><span class="sxs-lookup"><span data-stu-id="37ee6-107">Type</span></span>   |<span data-ttu-id="37ee6-108">説明</span><span class="sxs-lookup"><span data-stu-id="37ee6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37ee6-109">currentBegan</span><span class="sxs-lookup"><span data-stu-id="37ee6-109">currentBegan</span></span>|<span data-ttu-id="37ee6-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37ee6-110">DateTimeOffset</span></span>|<span data-ttu-id="37ee6-111">検疫が最後に評価および適用された日時。</span><span class="sxs-lookup"><span data-stu-id="37ee6-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="37ee6-112">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="37ee6-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37ee6-113">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="37ee6-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="37ee6-114">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="37ee6-114">nextAttempt</span></span>|<span data-ttu-id="37ee6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37ee6-115">DateTimeOffset</span></span>|<span data-ttu-id="37ee6-116">検疫を再評価する次の試行が行われた日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="37ee6-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="37ee6-117">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="37ee6-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37ee6-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="37ee6-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="37ee6-119">したがっ</span><span class="sxs-lookup"><span data-stu-id="37ee6-119">reason</span></span>|<span data-ttu-id="37ee6-120">String</span><span class="sxs-lookup"><span data-stu-id="37ee6-120">String</span></span>|<span data-ttu-id="37ee6-121">検疫が適用された理由を示すコード。</span><span class="sxs-lookup"><span data-stu-id="37ee6-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="37ee6-122">可能な値は、`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`Unknown` です。</span><span class="sxs-lookup"><span data-stu-id="37ee6-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="37ee6-123">系列の開始</span><span class="sxs-lookup"><span data-stu-id="37ee6-123">seriesBegan</span></span>|<span data-ttu-id="37ee6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37ee6-124">DateTimeOffset</span></span>|<span data-ttu-id="37ee6-125">このシリーズで最初に検疫が行われた日時です (一連の検疫が最初に実行されたときにシリーズが開始され、検疫がリフトされるとすぐにリセットされます)。</span><span class="sxs-lookup"><span data-stu-id="37ee6-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="37ee6-126">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="37ee6-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37ee6-127">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="37ee6-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="37ee6-128">系列数</span><span class="sxs-lookup"><span data-stu-id="37ee6-128">seriesCount</span></span>|<span data-ttu-id="37ee6-129">Int64</span><span class="sxs-lookup"><span data-stu-id="37ee6-129">Int64</span></span>|<span data-ttu-id="37ee6-130">このシリーズ内の回数再評価され、有効になっています (検疫が最初に行われたときにシリーズが開始され、検疫が解除されると直ちにリセットされます)。</span><span class="sxs-lookup"><span data-stu-id="37ee6-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37ee6-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37ee6-131">JSON representation</span></span>

<span data-ttu-id="37ee6-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="37ee6-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
