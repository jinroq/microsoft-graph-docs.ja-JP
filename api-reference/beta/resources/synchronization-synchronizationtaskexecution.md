---
title: 同期タスク実行リソースの種類
description: 同期ジョブの実行結果の概要を示します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e5a863111861d78b8a4131b68b8637b005aba49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007754"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="e49a2-103">同期タスク実行リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e49a2-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e49a2-104">同期ジョブの実行結果の概要を示します。</span><span class="sxs-lookup"><span data-stu-id="e49a2-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="e49a2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e49a2-105">Properties</span></span>
| <span data-ttu-id="e49a2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e49a2-106">Property</span></span>     | <span data-ttu-id="e49a2-107">型</span><span class="sxs-lookup"><span data-stu-id="e49a2-107">Type</span></span>   |<span data-ttu-id="e49a2-108">説明</span><span class="sxs-lookup"><span data-stu-id="e49a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e49a2-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="e49a2-109">activityIdentifier</span></span>           |<span data-ttu-id="e49a2-110">String</span><span class="sxs-lookup"><span data-stu-id="e49a2-110">String</span></span> |<span data-ttu-id="e49a2-111">ジョブの実行の識別子。</span><span class="sxs-lookup"><span data-stu-id="e49a2-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="e49a2-112">対象の count</span><span class="sxs-lookup"><span data-stu-id="e49a2-112">countEntitled</span></span>                |<span data-ttu-id="e49a2-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-113">Int64</span></span>  |<span data-ttu-id="e49a2-114">このアプリケーションに対して割り当てられた処理済みエントリの数。</span><span class="sxs-lookup"><span data-stu-id="e49a2-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="e49a2-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="e49a2-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="e49a2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-116">Int64</span></span>  |<span data-ttu-id="e49a2-117">プロビジョニング用に割り当てられた処理済みエントリの数。</span><span class="sxs-lookup"><span data-stu-id="e49a2-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="e49a2-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="e49a2-118">countEscrowed</span></span>                |<span data-ttu-id="e49a2-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-119">Int64</span></span>  |<span data-ttu-id="e49a2-120">Escrowed されたエントリの数 (エラー)。</span><span class="sxs-lookup"><span data-stu-id="e49a2-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="e49a2-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="e49a2-121">countEscrowedRaw</span></span>             |<span data-ttu-id="e49a2-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-122">Int64</span></span>  |<span data-ttu-id="e49a2-123">システム生成 escrows を含む、escrowed されたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="e49a2-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="e49a2-124">countExported 済み</span><span class="sxs-lookup"><span data-stu-id="e49a2-124">countExported</span></span>                |<span data-ttu-id="e49a2-125">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-125">Int64</span></span>  |<span data-ttu-id="e49a2-126">エクスポートされたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="e49a2-126">Count of exported entries.</span></span>|
|<span data-ttu-id="e49a2-127">countExports</span><span class="sxs-lookup"><span data-stu-id="e49a2-127">countExports</span></span>                 |<span data-ttu-id="e49a2-128">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-128">Int64</span></span>  |<span data-ttu-id="e49a2-129">エクスポートが予期されたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="e49a2-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="e49a2-130">countImported</span><span class="sxs-lookup"><span data-stu-id="e49a2-130">countImported</span></span>                |<span data-ttu-id="e49a2-131">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-131">Int64</span></span>  |<span data-ttu-id="e49a2-132">インポートされたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="e49a2-132">Count of imported entries.</span></span>|
|<span data-ttu-id="e49a2-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="e49a2-133">countImportedDeltas</span></span>          |<span data-ttu-id="e49a2-134">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-134">Int64</span></span>  |<span data-ttu-id="e49a2-135">インポートされたデルタ変更の数。</span><span class="sxs-lookup"><span data-stu-id="e49a2-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="e49a2-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="e49a2-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="e49a2-137">Int64</span><span class="sxs-lookup"><span data-stu-id="e49a2-137">Int64</span></span>  |<span data-ttu-id="e49a2-138">参照変更に関連するインポートされたデルタ変更の数。</span><span class="sxs-lookup"><span data-stu-id="e49a2-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="e49a2-139">error</span><span class="sxs-lookup"><span data-stu-id="e49a2-139">error</span></span>                        |[<span data-ttu-id="e49a2-140">同期エラー</span><span class="sxs-lookup"><span data-stu-id="e49a2-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="e49a2-141">エラーが発生した場合は、詳細情報を含む**同期エラー**オブジェクトが格納されています。</span><span class="sxs-lookup"><span data-stu-id="e49a2-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="e49a2-142">state</span><span class="sxs-lookup"><span data-stu-id="e49a2-142">state</span></span>                        |<span data-ttu-id="e49a2-143">String</span><span class="sxs-lookup"><span data-stu-id="e49a2-143">String</span></span> |<span data-ttu-id="e49a2-144">この実行の結果を要約したコード。</span><span class="sxs-lookup"><span data-stu-id="e49a2-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="e49a2-145">可能な値は、`Succeeded`、`Failed`、`EntryLevelErrors` です。</span><span class="sxs-lookup"><span data-stu-id="e49a2-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="e49a2-146">開始時刻</span><span class="sxs-lookup"><span data-stu-id="e49a2-146">timeBegan</span></span>                    |<span data-ttu-id="e49a2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49a2-147">DateTimeOffset</span></span>|<span data-ttu-id="e49a2-148">このジョブの実行が開始された時刻。</span><span class="sxs-lookup"><span data-stu-id="e49a2-148">Time when this job run began.</span></span> <span data-ttu-id="e49a2-149">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="e49a2-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e49a2-150">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e49a2-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e49a2-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="e49a2-151">timeEnded</span></span>                    |<span data-ttu-id="e49a2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49a2-152">DateTimeOffset</span></span>|<span data-ttu-id="e49a2-153">このジョブの実行が終了した時刻。</span><span class="sxs-lookup"><span data-stu-id="e49a2-153">Time when this job run ended.</span></span> <span data-ttu-id="e49a2-154">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="e49a2-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e49a2-155">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e49a2-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e49a2-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e49a2-156">JSON representation</span></span>

<span data-ttu-id="e49a2-157">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e49a2-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
