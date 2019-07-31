---
title: 同期状態リソースの種類
description: 同期ジョブの現在の状態を表します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e99db38b4f6c925f7ec7bfb2345582d6f8f9dae1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964621"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="ae720-103">同期状態リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae720-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae720-104">[同期ジョブ](synchronization-synchronizationjob.md)の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ae720-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ae720-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae720-105">Properties</span></span>

| <span data-ttu-id="ae720-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae720-106">Property</span></span>                              | <span data-ttu-id="ae720-107">型</span><span class="sxs-lookup"><span data-stu-id="ae720-107">Type</span></span>      | <span data-ttu-id="ae720-108">説明</span><span class="sxs-lookup"><span data-stu-id="ae720-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="ae720-109">code</span><span class="sxs-lookup"><span data-stu-id="ae720-109">code</span></span>|<span data-ttu-id="ae720-110">String</span><span class="sxs-lookup"><span data-stu-id="ae720-110">String</span></span>|<span data-ttu-id="ae720-111">同期ジョブの高レベルの状態コード。</span><span class="sxs-lookup"><span data-stu-id="ae720-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="ae720-112">可能な値は、`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="ae720-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="ae720-113">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="ae720-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="ae720-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ae720-114">Int64</span></span>|<span data-ttu-id="ae720-115">このジョブが失敗した連続した時間数。</span><span class="sxs-lookup"><span data-stu-id="ae720-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="ae720-116">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="ae720-116">escrowsPruned</span></span>|<span data-ttu-id="ae720-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae720-117">Boolean</span></span>|<span data-ttu-id="ae720-118">`true`最初の同期中にジョブの escrows (オブジェクトレベルのエラー) が排除された場合。</span><span class="sxs-lookup"><span data-stu-id="ae720-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="ae720-119">Escrows を排除できる初期の同期時には、通常、検疫内にジョブを配置するエラーのしきい値に達します。</span><span class="sxs-lookup"><span data-stu-id="ae720-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="ae720-120">検疫に入る代わりに、同期プロセスによってジョブのエラーがクリアされ、初期同期が完了するまで続行されます。</span><span class="sxs-lookup"><span data-stu-id="ae720-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="ae720-121">初期同期が完了すると、ジョブは一時停止し、ユーザーがエラーをクリーンアップするのを待ちます。</span><span class="sxs-lookup"><span data-stu-id="ae720-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="ae720-122">lastExecution</span><span class="sxs-lookup"><span data-stu-id="ae720-122">lastExecution</span></span>|[<span data-ttu-id="ae720-123">同期タスクの実行</span><span class="sxs-lookup"><span data-stu-id="ae720-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="ae720-124">ジョブの前回の実行の詳細。</span><span class="sxs-lookup"><span data-stu-id="ae720-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="ae720-125">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="ae720-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="ae720-126">同期タスクの実行</span><span class="sxs-lookup"><span data-stu-id="ae720-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="ae720-127">このジョブの前回の実行の詳細。エラーはありませんでした。</span><span class="sxs-lookup"><span data-stu-id="ae720-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="ae720-128">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="ae720-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="ae720-129">同期タスクの実行</span><span class="sxs-lookup"><span data-stu-id="ae720-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="ae720-130">ターゲットディレクトリにオブジェクトをエクスポートした、ジョブの最後の実行の詳細。</span><span class="sxs-lookup"><span data-stu-id="ae720-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="ae720-131">progress</span><span class="sxs-lookup"><span data-stu-id="ae720-131">progress</span></span>|<span data-ttu-id="ae720-132">[同期の進行状況](synchronization-synchronizationprogress.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="ae720-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="ae720-133">完了までのジョブの進行状況の詳細。</span><span class="sxs-lookup"><span data-stu-id="ae720-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="ae720-134">済み</span><span class="sxs-lookup"><span data-stu-id="ae720-134">quarantine</span></span>|[<span data-ttu-id="ae720-135">同期検疫</span><span class="sxs-lookup"><span data-stu-id="ae720-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="ae720-136">ジョブが検疫されている場合は、検疫の詳細。</span><span class="sxs-lookup"><span data-stu-id="ae720-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="ae720-137">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="ae720-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="ae720-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae720-138">DateTimeOffset</span></span>|<span data-ttu-id="ae720-139">安定した状態 (プロセスに加えられた変更はありません) が最初に達成された時刻。</span><span class="sxs-lookup"><span data-stu-id="ae720-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="ae720-140">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="ae720-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae720-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ae720-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ae720-142">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="ae720-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="ae720-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae720-143">DateTimeOffset</span></span>|<span data-ttu-id="ae720-144">安定した状態 (プロセスに加えられた変更がない状態) が最後に達成された時刻。</span><span class="sxs-lookup"><span data-stu-id="ae720-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="ae720-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="ae720-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae720-146">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ae720-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ae720-147">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="ae720-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="ae720-148">[Stringkeylongvaluepair](synchronization-stringkeylongvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ae720-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="ae720-149">オブジェクトの種類別にリストされた、同期されたオブジェクトの数。</span><span class="sxs-lookup"><span data-stu-id="ae720-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="ae720-150">トラブルシューティング Url</span><span class="sxs-lookup"><span data-stu-id="ae720-150">troubleshootingUrl</span></span>|<span data-ttu-id="ae720-151">String</span><span class="sxs-lookup"><span data-stu-id="ae720-151">String</span></span>|<span data-ttu-id="ae720-152">エラーが発生した場合は、問題のトラブルシューティング手順が記載されている URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="ae720-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="ae720-153">同期状態コードの詳細</span><span class="sxs-lookup"><span data-stu-id="ae720-153">Synchronization status code details</span></span>

| <span data-ttu-id="ae720-154">値</span><span class="sxs-lookup"><span data-stu-id="ae720-154">Value</span></span>                              | <span data-ttu-id="ae720-155">説明</span><span class="sxs-lookup"><span data-stu-id="ae720-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="ae720-156">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="ae720-156">NotConfigured</span></span>                       |<span data-ttu-id="ae720-157">ジョブは構成されておらず、実行されません。</span><span class="sxs-lookup"><span data-stu-id="ae720-157">Job was not configured and never run.</span></span> <span data-ttu-id="ae720-158">認証は提供されませんでした。</span><span class="sxs-lookup"><span data-stu-id="ae720-158">No authorization was provided.</span></span> |
|<span data-ttu-id="ae720-159">NotRun</span><span class="sxs-lookup"><span data-stu-id="ae720-159">NotRun</span></span>                              |<span data-ttu-id="ae720-160">ジョブが構成されている可能性がありますが、最初の実行が完了していない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ae720-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="ae720-161">Active</span><span class="sxs-lookup"><span data-stu-id="ae720-161">Active</span></span>                              |<span data-ttu-id="ae720-162">ジョブは定期的に実行されています。</span><span class="sxs-lookup"><span data-stu-id="ae720-162">Job is running periodically.</span></span>|
|<span data-ttu-id="ae720-163">一時停止</span><span class="sxs-lookup"><span data-stu-id="ae720-163">Paused</span></span>                              |<span data-ttu-id="ae720-164">ジョブが一時停止されました (通常は管理者によって)。現在実行されていませんが、ジョブの状態は保持されます。</span><span class="sxs-lookup"><span data-stu-id="ae720-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="ae720-165">検疫</span><span class="sxs-lookup"><span data-stu-id="ae720-165">Quarantine</span></span>                          |<span data-ttu-id="ae720-166">ジョブは検疫中です。</span><span class="sxs-lookup"><span data-stu-id="ae720-166">Job is in quarantine.</span></span> <span data-ttu-id="ae720-167">これは、大量のエラーが発生した場合や、失効済みまたは期限が切れた資格情報などの重大なエラーが発生した場合に発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ae720-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="ae720-168">検疫中は、同期プロセスによってジョブの実行が試行されます。</span><span class="sxs-lookup"><span data-stu-id="ae720-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae720-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae720-169">JSON representation</span></span>

<span data-ttu-id="ae720-170">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ae720-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
