---
title: synchronizationJob リソースの種類
description: バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。 同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。 同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。
ms.openlocfilehash: 0e6428f2a088e5326f4412e743489c4d94b10296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073911"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="3213e-105">synchronizationJob リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3213e-105">synchronizationJob resource type</span></span>

> <span data-ttu-id="3213e-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3213e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3213e-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3213e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3213e-108">バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。</span><span class="sxs-lookup"><span data-stu-id="3213e-108">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="3213e-109">同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。</span><span class="sxs-lookup"><span data-stu-id="3213e-109">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="3213e-110">同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3213e-110">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="3213e-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="3213e-111">Methods</span></span>

| <span data-ttu-id="3213e-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="3213e-112">Method</span></span>        | <span data-ttu-id="3213e-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3213e-113">Return Type</span></span>               | <span data-ttu-id="3213e-114">説明</span><span class="sxs-lookup"><span data-stu-id="3213e-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="3213e-115">List</span><span class="sxs-lookup"><span data-stu-id="3213e-115">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="3213e-116">[synchronizationJob](synchronization-synchronizationjob.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3213e-116">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="3213e-117">特定のアプリケーションのインスタンス (サービス主体) の既存のジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3213e-117">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="3213e-118">SynchronizationJob を取得します。</span><span class="sxs-lookup"><span data-stu-id="3213e-118">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="3213e-119">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3213e-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="3213e-120">SynchronizationJob オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3213e-120">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="3213e-121">作成</span><span class="sxs-lookup"><span data-stu-id="3213e-121">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="3213e-122">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3213e-122">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="3213e-123">特定のアプリケーション用の新しいジョブを作成します。</span><span class="sxs-lookup"><span data-stu-id="3213e-123">Create new job for a given application.</span></span>|
|[<span data-ttu-id="3213e-124">Start</span><span class="sxs-lookup"><span data-stu-id="3213e-124">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="3213e-125">なし</span><span class="sxs-lookup"><span data-stu-id="3213e-125">None</span></span>   |<span data-ttu-id="3213e-126">同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="3213e-126">Start synchronization.</span></span> <span data-ttu-id="3213e-127">ジョブが一時停止状態にある場合は、ジョブが一時停止された時点から続行します。</span><span class="sxs-lookup"><span data-stu-id="3213e-127">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="3213e-128">ジョブは、検疫では、検疫の状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="3213e-128">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="3213e-129">Restart</span><span class="sxs-lookup"><span data-stu-id="3213e-129">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="3213e-130">なし</span><span class="sxs-lookup"><span data-stu-id="3213e-130">None</span></span>   |<span data-ttu-id="3213e-131">上で起動し、ディレクトリ内のすべてのオブジェクトを再処理するジョブを強制します。</span><span class="sxs-lookup"><span data-stu-id="3213e-131">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="3213e-132">Pause</span><span class="sxs-lookup"><span data-stu-id="3213e-132">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="3213e-133">なし</span><span class="sxs-lookup"><span data-stu-id="3213e-133">None</span></span>   |<span data-ttu-id="3213e-134">同期を一時的に停止します。</span><span class="sxs-lookup"><span data-stu-id="3213e-134">Temporarily stop synchronization.</span></span> <span data-ttu-id="3213e-135">ジョブの状態を含むすべての進捗が保持され、ジョブが[起動](../api/synchronization-synchronizationjob-start.md)の呼び出しが行われる場合停止した位置から続行されます。</span><span class="sxs-lookup"><span data-stu-id="3213e-135">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="3213e-136">削除</span><span class="sxs-lookup"><span data-stu-id="3213e-136">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="3213e-137">なし</span><span class="sxs-lookup"><span data-stu-id="3213e-137">None</span></span>   |<span data-ttu-id="3213e-138">同期を停止し、ジョブに関連付けられているすべての状態を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="3213e-138">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="3213e-139">SynchrnoizationSchema を取得します。</span><span class="sxs-lookup"><span data-stu-id="3213e-139">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="3213e-140">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="3213e-140">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="3213e-141">ジョブの効果的な同期スキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="3213e-141">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="3213e-142">SynchroizationSchema を更新します。</span><span class="sxs-lookup"><span data-stu-id="3213e-142">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="3213e-143">なし</span><span class="sxs-lookup"><span data-stu-id="3213e-143">None</span></span>   |<span data-ttu-id="3213e-144">ジョブの同期のスキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="3213e-144">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="3213e-145">資格情報を検証します。</span><span class="sxs-lookup"><span data-stu-id="3213e-145">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="3213e-146">なし</span><span class="sxs-lookup"><span data-stu-id="3213e-146">None</span></span>|<span data-ttu-id="3213e-147">ターゲット ディレクトリに対して指定された資格情報をテストします。</span><span class="sxs-lookup"><span data-stu-id="3213e-147">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="3213e-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3213e-148">Properties</span></span>

| <span data-ttu-id="3213e-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3213e-149">Property</span></span>      | <span data-ttu-id="3213e-150">型</span><span class="sxs-lookup"><span data-stu-id="3213e-150">Type</span></span>      | <span data-ttu-id="3213e-151">説明</span><span class="sxs-lookup"><span data-stu-id="3213e-151">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="3213e-152">id</span><span class="sxs-lookup"><span data-stu-id="3213e-152">id</span></span>             |<span data-ttu-id="3213e-153">String</span><span class="sxs-lookup"><span data-stu-id="3213e-153">String</span></span>                     |<span data-ttu-id="3213e-154">固有の同期ジョブの識別子です。</span><span class="sxs-lookup"><span data-stu-id="3213e-154">Unique synchronization job identifier.</span></span> <span data-ttu-id="3213e-155">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3213e-155">Read-only.</span></span>|
|<span data-ttu-id="3213e-156">スケジュール</span><span class="sxs-lookup"><span data-stu-id="3213e-156">schedule</span></span>       |[<span data-ttu-id="3213e-157">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="3213e-157">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="3213e-158">スケジュールがジョブを実行するために使用します。</span><span class="sxs-lookup"><span data-stu-id="3213e-158">Schedule used to run the job.</span></span> <span data-ttu-id="3213e-159">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3213e-159">Read-only.</span></span>|
|<span data-ttu-id="3213e-160">status</span><span class="sxs-lookup"><span data-stu-id="3213e-160">status</span></span>         |[<span data-ttu-id="3213e-161">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="3213e-161">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="3213e-162">ジョブが前回実行されたときに、ジョブ、ジョブの現在の状態およびエラーの状態です。</span><span class="sxs-lookup"><span data-stu-id="3213e-162">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="3213e-163">templateId</span><span class="sxs-lookup"><span data-stu-id="3213e-163">templateId</span></span>     |<span data-ttu-id="3213e-164">文字列</span><span class="sxs-lookup"><span data-stu-id="3213e-164">String</span></span>    |<span data-ttu-id="3213e-165">このジョブで使用する[同期テンプレート](synchronization-synchronizationtemplate.md)の識別子です。</span><span class="sxs-lookup"><span data-stu-id="3213e-165">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3213e-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3213e-166">Relationships</span></span>
| <span data-ttu-id="3213e-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3213e-167">Relationship</span></span> | <span data-ttu-id="3213e-168">型</span><span class="sxs-lookup"><span data-stu-id="3213e-168">Type</span></span>   |<span data-ttu-id="3213e-169">説明</span><span class="sxs-lookup"><span data-stu-id="3213e-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3213e-170">スキーマ</span><span class="sxs-lookup"><span data-stu-id="3213e-170">schema</span></span>|[<span data-ttu-id="3213e-171">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="3213e-171">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="3213e-172">ジョブ用に構成された同期スキーマです。</span><span class="sxs-lookup"><span data-stu-id="3213e-172">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3213e-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3213e-173">JSON representation</span></span>

<span data-ttu-id="3213e-174">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3213e-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->