---
title: synchronizationTaskExecution リソースの種類
description: 同期ジョブの実行の結果をまとめたものです。
localization_priority: Normal
ms.openlocfilehash: 37a0fd57269cef6d3cb03c5cc5c38d3024fe198d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510555"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="2da1b-103">synchronizationTaskExecution リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2da1b-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2da1b-104">同期ジョブの実行の結果をまとめたものです。</span><span class="sxs-lookup"><span data-stu-id="2da1b-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="2da1b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2da1b-105">Properties</span></span>
| <span data-ttu-id="2da1b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2da1b-106">Property</span></span>     | <span data-ttu-id="2da1b-107">型</span><span class="sxs-lookup"><span data-stu-id="2da1b-107">Type</span></span>   |<span data-ttu-id="2da1b-108">説明</span><span class="sxs-lookup"><span data-stu-id="2da1b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2da1b-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="2da1b-109">activityIdentifier</span></span>           |<span data-ttu-id="2da1b-110">String</span><span class="sxs-lookup"><span data-stu-id="2da1b-110">String</span></span> |<span data-ttu-id="2da1b-111">実行ジョブの識別子です。</span><span class="sxs-lookup"><span data-stu-id="2da1b-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="2da1b-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="2da1b-112">countEntitled</span></span>                |<span data-ttu-id="2da1b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-113">Int64</span></span>  |<span data-ttu-id="2da1b-114">このアプリケーションに割り当てられた処理されたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="2da1b-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="2da1b-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="2da1b-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="2da1b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-116">Int64</span></span>  |<span data-ttu-id="2da1b-117">プロビジョニング用に割り当てられた処理されたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="2da1b-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="2da1b-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="2da1b-118">countEscrowed</span></span>                |<span data-ttu-id="2da1b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-119">Int64</span></span>  |<span data-ttu-id="2da1b-120">Escrowed (エラー) のエントリの数。</span><span class="sxs-lookup"><span data-stu-id="2da1b-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="2da1b-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="2da1b-121">countEscrowedRaw</span></span>             |<span data-ttu-id="2da1b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-122">Int64</span></span>  |<span data-ttu-id="2da1b-123">Escrows のシステムで生成されたを含む、escrowed されたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="2da1b-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="2da1b-124">countExported</span><span class="sxs-lookup"><span data-stu-id="2da1b-124">countExported</span></span>                |<span data-ttu-id="2da1b-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-125">Int64</span></span>  |<span data-ttu-id="2da1b-126">エクスポートされたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="2da1b-126">Count of exported entries.</span></span>|
|<span data-ttu-id="2da1b-127">countExports</span><span class="sxs-lookup"><span data-stu-id="2da1b-127">countExports</span></span>                 |<span data-ttu-id="2da1b-128">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-128">Int64</span></span>  |<span data-ttu-id="2da1b-129">エクスポートする必要があるエントリの数です。</span><span class="sxs-lookup"><span data-stu-id="2da1b-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="2da1b-130">countImported</span><span class="sxs-lookup"><span data-stu-id="2da1b-130">countImported</span></span>                |<span data-ttu-id="2da1b-131">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-131">Int64</span></span>  |<span data-ttu-id="2da1b-132">インポートされたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="2da1b-132">Count of imported entries.</span></span>|
|<span data-ttu-id="2da1b-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="2da1b-133">countImportedDeltas</span></span>          |<span data-ttu-id="2da1b-134">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-134">Int64</span></span>  |<span data-ttu-id="2da1b-135">インポートの差分変更の数です。</span><span class="sxs-lookup"><span data-stu-id="2da1b-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="2da1b-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="2da1b-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="2da1b-137">Int64</span><span class="sxs-lookup"><span data-stu-id="2da1b-137">Int64</span></span>  |<span data-ttu-id="2da1b-138">参照の変更に関連するインポートされたデルタの変更の数です。</span><span class="sxs-lookup"><span data-stu-id="2da1b-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="2da1b-139">エラー</span><span class="sxs-lookup"><span data-stu-id="2da1b-139">error</span></span>                        |[<span data-ttu-id="2da1b-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="2da1b-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="2da1b-141">エラーが発生した場合に、詳細を含む、 **synchronizationError**オブジェクトが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2da1b-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="2da1b-142">state</span><span class="sxs-lookup"><span data-stu-id="2da1b-142">state</span></span>                        |<span data-ttu-id="2da1b-143">String</span><span class="sxs-lookup"><span data-stu-id="2da1b-143">String</span></span> |<span data-ttu-id="2da1b-144">コードがこの実行の結果を要約します。</span><span class="sxs-lookup"><span data-stu-id="2da1b-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="2da1b-145">可能な値は、`Succeeded`、`Failed`、`EntryLevelErrors` です。</span><span class="sxs-lookup"><span data-stu-id="2da1b-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="2da1b-146">timeBegan</span><span class="sxs-lookup"><span data-stu-id="2da1b-146">timeBegan</span></span>                    |<span data-ttu-id="2da1b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2da1b-147">DateTimeOffset</span></span>|<span data-ttu-id="2da1b-148">このジョブの実行を開始したときの時間です。</span><span class="sxs-lookup"><span data-stu-id="2da1b-148">Time when this job run began.</span></span> <span data-ttu-id="2da1b-149">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2da1b-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2da1b-150">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="2da1b-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2da1b-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="2da1b-151">timeEnded</span></span>                    |<span data-ttu-id="2da1b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2da1b-152">DateTimeOffset</span></span>|<span data-ttu-id="2da1b-153">このジョブを実行すると時間が終了しました。</span><span class="sxs-lookup"><span data-stu-id="2da1b-153">Time when this job run ended.</span></span> <span data-ttu-id="2da1b-154">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2da1b-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2da1b-155">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="2da1b-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2da1b-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2da1b-156">JSON representation</span></span>

<span data-ttu-id="2da1b-157">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2da1b-157">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtaskexecution.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
