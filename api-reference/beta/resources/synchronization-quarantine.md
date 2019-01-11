---
title: synchronizationQuarantine リソースの種類
description: SynchronizationJob の検査の状態に関する情報を提供します。
localization_priority: Normal
ms.openlocfilehash: fba0077d48e69ed4c2c190d0b50a6fcfc1749626
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849729"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="78be8-103">synchronizationQuarantine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78be8-103">synchronizationQuarantine resource type</span></span>

> <span data-ttu-id="78be8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78be8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78be8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78be8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78be8-106">の[synchronizationJob](synchronization-synchronizationjob.md)の検査の状態に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="78be8-106">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="78be8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78be8-107">Properties</span></span>
| <span data-ttu-id="78be8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78be8-108">Property</span></span>     | <span data-ttu-id="78be8-109">種類</span><span class="sxs-lookup"><span data-stu-id="78be8-109">Type</span></span>   |<span data-ttu-id="78be8-110">説明</span><span class="sxs-lookup"><span data-stu-id="78be8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78be8-111">currentBegan</span><span class="sxs-lookup"><span data-stu-id="78be8-111">currentBegan</span></span>|<span data-ttu-id="78be8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78be8-112">DateTimeOffset</span></span>|<span data-ttu-id="78be8-113">日付と時刻の検査が最後に評価され、課されます。</span><span class="sxs-lookup"><span data-stu-id="78be8-113">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="78be8-114">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="78be8-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="78be8-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78be8-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="78be8-116">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="78be8-116">nextAttempt</span></span>|<span data-ttu-id="78be8-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78be8-117">DateTimeOffset</span></span>|<span data-ttu-id="78be8-118">日付と時刻、次が再検査を評価しようとした場合に行われます。</span><span class="sxs-lookup"><span data-stu-id="78be8-118">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="78be8-119">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="78be8-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="78be8-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78be8-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="78be8-121">理由</span><span class="sxs-lookup"><span data-stu-id="78be8-121">reason</span></span>|<span data-ttu-id="78be8-122">String</span><span class="sxs-lookup"><span data-stu-id="78be8-122">String</span></span>|<span data-ttu-id="78be8-123">検疫が適用された理由を示すコードです。</span><span class="sxs-lookup"><span data-stu-id="78be8-123">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="78be8-124">可能な値は、`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`Unknown` です。</span><span class="sxs-lookup"><span data-stu-id="78be8-124">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="78be8-125">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="78be8-125">seriesBegan</span></span>|<span data-ttu-id="78be8-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78be8-126">DateTimeOffset</span></span>|<span data-ttu-id="78be8-127">日付と時刻の検査が最初にこのシリーズ (シリーズを開始すると、検疫が最初に適用されると、隔離が解除されると、すぐにリセットされます) に課されます。</span><span class="sxs-lookup"><span data-stu-id="78be8-127">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="78be8-128">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="78be8-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="78be8-129">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78be8-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="78be8-130">seriesCount</span><span class="sxs-lookup"><span data-stu-id="78be8-130">seriesCount</span></span>|<span data-ttu-id="78be8-131">Int64</span><span class="sxs-lookup"><span data-stu-id="78be8-131">Int64</span></span>|<span data-ttu-id="78be8-132">このシリーズは、検査の回数が再評価し、左 (シリーズ開始と検査は、最初に適用されると、隔離が解除されると、すぐにリセットされます) では有効にします。</span><span class="sxs-lookup"><span data-stu-id="78be8-132">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78be8-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78be8-133">JSON representation</span></span>

<span data-ttu-id="78be8-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78be8-134">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
