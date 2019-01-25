---
title: synchronizationStatus リソースの種類
description: SynchronizationJob の現在の状態を表します。
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523765"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="18858-103">synchronizationStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18858-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18858-104">[SynchronizationJob](synchronization-synchronizationjob.md)の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="18858-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="18858-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18858-105">Properties</span></span>

| <span data-ttu-id="18858-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18858-106">Property</span></span>                              | <span data-ttu-id="18858-107">型</span><span class="sxs-lookup"><span data-stu-id="18858-107">Type</span></span>      | <span data-ttu-id="18858-108">説明</span><span class="sxs-lookup"><span data-stu-id="18858-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="18858-109">code</span><span class="sxs-lookup"><span data-stu-id="18858-109">code</span></span>|<span data-ttu-id="18858-110">String</span><span class="sxs-lookup"><span data-stu-id="18858-110">String</span></span>|<span data-ttu-id="18858-111">同期ジョブの高度なステータス コードです。</span><span class="sxs-lookup"><span data-stu-id="18858-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="18858-112">可能な値は、`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="18858-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="18858-113">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="18858-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="18858-114">Int64</span><span class="sxs-lookup"><span data-stu-id="18858-114">Int64</span></span>|<span data-ttu-id="18858-115">連続回数このジョブが失敗しました。</span><span class="sxs-lookup"><span data-stu-id="18858-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="18858-116">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="18858-116">escrowsPruned</span></span>|<span data-ttu-id="18858-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="18858-117">Boolean</span></span>|<span data-ttu-id="18858-118">`true`場合はジョブの escrows (オブジェクト レベルのエラー) は、初期同期中に排除されました。</span><span class="sxs-lookup"><span data-stu-id="18858-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="18858-119">初期同期中にエラーを通常どおりになりそうなジョブ検疫のしきい値に達した場合、escrows を排除することができます。</span><span class="sxs-lookup"><span data-stu-id="18858-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="18858-120">検疫場所にではなく、同期プロセスはジョブのエラーをクリアし、初期同期が完了するまで続きます。</span><span class="sxs-lookup"><span data-stu-id="18858-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="18858-121">初期同期が完了すると、ジョブが一時停止し、エラーをクリーンアップするまで待機します。</span><span class="sxs-lookup"><span data-stu-id="18858-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="18858-122">lastExecution</span><span class="sxs-lookup"><span data-stu-id="18858-122">lastExecution</span></span>|[<span data-ttu-id="18858-123">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="18858-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="18858-124">ジョブの前回の実行の詳細です。</span><span class="sxs-lookup"><span data-stu-id="18858-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="18858-125">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="18858-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="18858-126">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="18858-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="18858-127">このジョブは、エラーがなかったは、前回の実行の詳細です。</span><span class="sxs-lookup"><span data-stu-id="18858-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="18858-128">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="18858-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="18858-129">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="18858-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="18858-130">ターゲット ディレクトリにオブジェクトをエクスポートすると、ジョブの前回の実行の詳細です。</span><span class="sxs-lookup"><span data-stu-id="18858-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="18858-131">進行状況</span><span class="sxs-lookup"><span data-stu-id="18858-131">progress</span></span>|<span data-ttu-id="18858-132">[synchronizationProgress](synchronization-synchronizationprogress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18858-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="18858-133">完了するまで、ジョブの進行状況の詳細です。</span><span class="sxs-lookup"><span data-stu-id="18858-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="18858-134">検査</span><span class="sxs-lookup"><span data-stu-id="18858-134">quarantine</span></span>|[<span data-ttu-id="18858-135">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="18858-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="18858-136">検査中のジョブの場合は、詳細を検査します。</span><span class="sxs-lookup"><span data-stu-id="18858-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="18858-137">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="18858-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="18858-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18858-138">DateTimeOffset</span></span>|<span data-ttu-id="18858-139">最初に安定した状態 (プロセスに変更) が達成された時間です。</span><span class="sxs-lookup"><span data-stu-id="18858-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="18858-140">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="18858-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18858-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="18858-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="18858-142">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="18858-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="18858-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18858-143">DateTimeOffset</span></span>|<span data-ttu-id="18858-144">最後に安定した状態 (プロセスに変更) が達成された時間です。</span><span class="sxs-lookup"><span data-stu-id="18858-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="18858-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="18858-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18858-146">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="18858-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="18858-147">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="18858-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="18858-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18858-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="18858-149">オブジェクトの種類ごとに一覧表示、同期オブジェクトの数。</span><span class="sxs-lookup"><span data-stu-id="18858-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="18858-150">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="18858-150">troubleshootingUrl</span></span>|<span data-ttu-id="18858-151">String</span><span class="sxs-lookup"><span data-stu-id="18858-151">String</span></span>|<span data-ttu-id="18858-152">エラーの場合、問題のトラブルシューティングの手順で URL です。</span><span class="sxs-lookup"><span data-stu-id="18858-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="18858-153">同期ステータス コードの詳細</span><span class="sxs-lookup"><span data-stu-id="18858-153">Synchronization status code details</span></span>

| <span data-ttu-id="18858-154">値</span><span class="sxs-lookup"><span data-stu-id="18858-154">Value</span></span>                              | <span data-ttu-id="18858-155">説明</span><span class="sxs-lookup"><span data-stu-id="18858-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="18858-156">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="18858-156">NotConfigured</span></span>                       |<span data-ttu-id="18858-157">ジョブが構成されていないと、実行しません。</span><span class="sxs-lookup"><span data-stu-id="18858-157">Job was not configured and never run.</span></span> <span data-ttu-id="18858-158">認証が指定されていません。</span><span class="sxs-lookup"><span data-stu-id="18858-158">No authorization was provided.</span></span> |
|<span data-ttu-id="18858-159">NotRun</span><span class="sxs-lookup"><span data-stu-id="18858-159">NotRun</span></span>                              |<span data-ttu-id="18858-160">ジョブは、設定されていれば、および可能性があります開始は、その最初の実行を終了していません。</span><span class="sxs-lookup"><span data-stu-id="18858-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="18858-161">Active</span><span class="sxs-lookup"><span data-stu-id="18858-161">Active</span></span>                              |<span data-ttu-id="18858-162">ジョブの有効期限が定期的に行われています。</span><span class="sxs-lookup"><span data-stu-id="18858-162">Job is running periodically.</span></span>|
|<span data-ttu-id="18858-163">一時停止</span><span class="sxs-lookup"><span data-stu-id="18858-163">Paused</span></span>                              |<span data-ttu-id="18858-164">ジョブ (管理者) は通常、一時停止し、現在実行されていないが、ジョブの状態が保持されます。</span><span class="sxs-lookup"><span data-stu-id="18858-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="18858-165">検査</span><span class="sxs-lookup"><span data-stu-id="18858-165">Quarantine</span></span>                          |<span data-ttu-id="18858-166">ジョブでは、検査中です。</span><span class="sxs-lookup"><span data-stu-id="18858-166">Job is in quarantine.</span></span> <span data-ttu-id="18858-167">大量のエラー、または資格情報の失効期限切れなどの重大なエラーがある場合、このエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="18858-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="18858-168">検査中に、同期処理を減少の頻度でジョブの実行を試みます。</span><span class="sxs-lookup"><span data-stu-id="18858-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18858-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18858-169">JSON representation</span></span>

<span data-ttu-id="18858-170">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="18858-170">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
