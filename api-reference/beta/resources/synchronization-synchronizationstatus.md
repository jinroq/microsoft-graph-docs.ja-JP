---
title: synchronizationStatus リソースの種類
description: SynchronizationJob の現在の状態を表します。
ms.openlocfilehash: cf1b1e79e5ad784f1f43a2e5bf082c68b41e96ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074417"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="18e78-103">synchronizationStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18e78-103">synchronizationStatus resource type</span></span>

> <span data-ttu-id="18e78-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18e78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18e78-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18e78-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18e78-106">[SynchronizationJob](synchronization-synchronizationjob.md)の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="18e78-106">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="18e78-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18e78-107">Properties</span></span>

| <span data-ttu-id="18e78-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18e78-108">Property</span></span>                              | <span data-ttu-id="18e78-109">型</span><span class="sxs-lookup"><span data-stu-id="18e78-109">Type</span></span>      | <span data-ttu-id="18e78-110">説明</span><span class="sxs-lookup"><span data-stu-id="18e78-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="18e78-111">code</span><span class="sxs-lookup"><span data-stu-id="18e78-111">code</span></span>|<span data-ttu-id="18e78-112">String</span><span class="sxs-lookup"><span data-stu-id="18e78-112">String</span></span>|<span data-ttu-id="18e78-113">同期ジョブの高度なステータス コードです。</span><span class="sxs-lookup"><span data-stu-id="18e78-113">High-level status code of the synchronization job.</span></span> <span data-ttu-id="18e78-114">可能な値は、`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="18e78-114">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="18e78-115">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="18e78-115">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="18e78-116">Int64</span><span class="sxs-lookup"><span data-stu-id="18e78-116">Int64</span></span>|<span data-ttu-id="18e78-117">連続回数このジョブが失敗しました。</span><span class="sxs-lookup"><span data-stu-id="18e78-117">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="18e78-118">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="18e78-118">escrowsPruned</span></span>|<span data-ttu-id="18e78-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="18e78-119">Boolean</span></span>|<span data-ttu-id="18e78-120">`true`場合はジョブの escrows (オブジェクト レベルのエラー) は、初期同期中に排除されました。</span><span class="sxs-lookup"><span data-stu-id="18e78-120">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="18e78-121">初期同期中にエラーを通常どおりになりそうなジョブ検疫のしきい値に達した場合、escrows を排除することができます。</span><span class="sxs-lookup"><span data-stu-id="18e78-121">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="18e78-122">検疫場所にではなく、同期プロセスはジョブのエラーをクリアし、初期同期が完了するまで続きます。</span><span class="sxs-lookup"><span data-stu-id="18e78-122">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="18e78-123">初期同期が完了すると、ジョブが一時停止し、エラーをクリーンアップするまで待機します。</span><span class="sxs-lookup"><span data-stu-id="18e78-123">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="18e78-124">lastExecution</span><span class="sxs-lookup"><span data-stu-id="18e78-124">lastExecution</span></span>|[<span data-ttu-id="18e78-125">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="18e78-125">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="18e78-126">ジョブの前回の実行の詳細です。</span><span class="sxs-lookup"><span data-stu-id="18e78-126">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="18e78-127">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="18e78-127">lastSuccessfulExecution</span></span>|[<span data-ttu-id="18e78-128">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="18e78-128">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="18e78-129">このジョブは、エラーがなかったは、前回の実行の詳細です。</span><span class="sxs-lookup"><span data-stu-id="18e78-129">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="18e78-130">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="18e78-130">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="18e78-131">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="18e78-131">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="18e78-132">ターゲット ディレクトリにオブジェクトをエクスポートすると、ジョブの前回の実行の詳細です。</span><span class="sxs-lookup"><span data-stu-id="18e78-132">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="18e78-133">進行状況</span><span class="sxs-lookup"><span data-stu-id="18e78-133">progress</span></span>|<span data-ttu-id="18e78-134">[synchronizationProgress](synchronization-synchronizationprogress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18e78-134">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="18e78-135">完了するまで、ジョブの進行状況の詳細です。</span><span class="sxs-lookup"><span data-stu-id="18e78-135">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="18e78-136">検査</span><span class="sxs-lookup"><span data-stu-id="18e78-136">quarantine</span></span>|[<span data-ttu-id="18e78-137">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="18e78-137">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="18e78-138">検査中のジョブの場合は、詳細を検査します。</span><span class="sxs-lookup"><span data-stu-id="18e78-138">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="18e78-139">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="18e78-139">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="18e78-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18e78-140">DateTimeOffset</span></span>|<span data-ttu-id="18e78-141">最初に安定した状態 (プロセスに変更) が達成された時間です。</span><span class="sxs-lookup"><span data-stu-id="18e78-141">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="18e78-142">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="18e78-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18e78-143">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="18e78-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="18e78-144">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="18e78-144">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="18e78-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18e78-145">DateTimeOffset</span></span>|<span data-ttu-id="18e78-146">最後に安定した状態 (プロセスに変更) が達成された時間です。</span><span class="sxs-lookup"><span data-stu-id="18e78-146">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="18e78-147">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="18e78-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18e78-148">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="18e78-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="18e78-149">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="18e78-149">synchronizedEntryCountByType</span></span>|<span data-ttu-id="18e78-150">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18e78-150">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="18e78-151">オブジェクトの種類ごとに一覧表示、同期オブジェクトの数。</span><span class="sxs-lookup"><span data-stu-id="18e78-151">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="18e78-152">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="18e78-152">troubleshootingUrl</span></span>|<span data-ttu-id="18e78-153">String</span><span class="sxs-lookup"><span data-stu-id="18e78-153">String</span></span>|<span data-ttu-id="18e78-154">エラーの場合、問題のトラブルシューティングの手順で URL です。</span><span class="sxs-lookup"><span data-stu-id="18e78-154">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="18e78-155">同期ステータス コードの詳細</span><span class="sxs-lookup"><span data-stu-id="18e78-155">Synchronization status code details</span></span>

| <span data-ttu-id="18e78-156">値</span><span class="sxs-lookup"><span data-stu-id="18e78-156">Value</span></span>                              | <span data-ttu-id="18e78-157">説明</span><span class="sxs-lookup"><span data-stu-id="18e78-157">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="18e78-158">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="18e78-158">NotConfigured</span></span>                       |<span data-ttu-id="18e78-159">ジョブが構成されていないと、実行しません。</span><span class="sxs-lookup"><span data-stu-id="18e78-159">Job was not configured and never run.</span></span> <span data-ttu-id="18e78-160">認証が指定されていません。</span><span class="sxs-lookup"><span data-stu-id="18e78-160">No authorization was provided.</span></span> |
|<span data-ttu-id="18e78-161">NotRun</span><span class="sxs-lookup"><span data-stu-id="18e78-161">NotRun</span></span>                              |<span data-ttu-id="18e78-162">ジョブは、設定されていれば、および可能性があります開始は、その最初の実行を終了していません。</span><span class="sxs-lookup"><span data-stu-id="18e78-162">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="18e78-163">アクティブ</span><span class="sxs-lookup"><span data-stu-id="18e78-163">Active</span></span>                              |<span data-ttu-id="18e78-164">ジョブの有効期限が定期的に行われています。</span><span class="sxs-lookup"><span data-stu-id="18e78-164">Job is running periodically.</span></span>|
|<span data-ttu-id="18e78-165">一時停止</span><span class="sxs-lookup"><span data-stu-id="18e78-165">Paused</span></span>                              |<span data-ttu-id="18e78-166">ジョブ (管理者) は通常、一時停止し、現在実行されていないが、ジョブの状態が保持されます。</span><span class="sxs-lookup"><span data-stu-id="18e78-166">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="18e78-167">検査</span><span class="sxs-lookup"><span data-stu-id="18e78-167">Quarantine</span></span>                          |<span data-ttu-id="18e78-168">ジョブでは、検査中です。</span><span class="sxs-lookup"><span data-stu-id="18e78-168">Job is in quarantine.</span></span> <span data-ttu-id="18e78-169">大量のエラー、または資格情報の失効期限切れなどの重大なエラーがある場合、このエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="18e78-169">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="18e78-170">検査中に、同期処理を減少の頻度でジョブの実行を試みます。</span><span class="sxs-lookup"><span data-stu-id="18e78-170">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18e78-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18e78-171">JSON representation</span></span>

<span data-ttu-id="18e78-172">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="18e78-172">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
