---
title: synchronizationQuarantine リソースの種類
description: SynchronizationJob の検査の状態に関する情報を提供します。
localization_priority: Normal
ms.openlocfilehash: 6d5d5c3cbe96eda6b39833287e8efb6e0771b19a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518815"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="25d87-103">synchronizationQuarantine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25d87-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25d87-104">の[synchronizationJob](synchronization-synchronizationjob.md)の検査の状態に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="25d87-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="25d87-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25d87-105">Properties</span></span>
| <span data-ttu-id="25d87-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25d87-106">Property</span></span>     | <span data-ttu-id="25d87-107">型</span><span class="sxs-lookup"><span data-stu-id="25d87-107">Type</span></span>   |<span data-ttu-id="25d87-108">説明</span><span class="sxs-lookup"><span data-stu-id="25d87-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25d87-109">currentBegan</span><span class="sxs-lookup"><span data-stu-id="25d87-109">currentBegan</span></span>|<span data-ttu-id="25d87-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d87-110">DateTimeOffset</span></span>|<span data-ttu-id="25d87-111">日付と時刻の検査が最後に評価され、課されます。</span><span class="sxs-lookup"><span data-stu-id="25d87-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="25d87-112">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="25d87-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25d87-113">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="25d87-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="25d87-114">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="25d87-114">nextAttempt</span></span>|<span data-ttu-id="25d87-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d87-115">DateTimeOffset</span></span>|<span data-ttu-id="25d87-116">日付と時刻、次が再検査を評価しようとした場合に行われます。</span><span class="sxs-lookup"><span data-stu-id="25d87-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="25d87-117">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="25d87-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25d87-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="25d87-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="25d87-119">理由</span><span class="sxs-lookup"><span data-stu-id="25d87-119">reason</span></span>|<span data-ttu-id="25d87-120">String</span><span class="sxs-lookup"><span data-stu-id="25d87-120">String</span></span>|<span data-ttu-id="25d87-121">検疫が適用された理由を示すコードです。</span><span class="sxs-lookup"><span data-stu-id="25d87-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="25d87-122">可能な値は、`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`Unknown` です。</span><span class="sxs-lookup"><span data-stu-id="25d87-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="25d87-123">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="25d87-123">seriesBegan</span></span>|<span data-ttu-id="25d87-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d87-124">DateTimeOffset</span></span>|<span data-ttu-id="25d87-125">日付と時刻の検査が最初にこのシリーズ (シリーズを開始すると、検疫が最初に適用されると、隔離が解除されると、すぐにリセットされます) に課されます。</span><span class="sxs-lookup"><span data-stu-id="25d87-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="25d87-126">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="25d87-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25d87-127">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="25d87-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="25d87-128">seriesCount</span><span class="sxs-lookup"><span data-stu-id="25d87-128">seriesCount</span></span>|<span data-ttu-id="25d87-129">Int64</span><span class="sxs-lookup"><span data-stu-id="25d87-129">Int64</span></span>|<span data-ttu-id="25d87-130">このシリーズは、検査の回数が再評価し、左 (シリーズ開始と検査は、最初に適用されると、隔離が解除されると、すぐにリセットされます) では有効にします。</span><span class="sxs-lookup"><span data-stu-id="25d87-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25d87-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25d87-131">JSON representation</span></span>

<span data-ttu-id="25d87-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="25d87-132">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-quarantine.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
