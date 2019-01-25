---
title: synchronizationJob リソースの種類
description: バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。 同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。 同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510569"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="ca479-105">synchronizationJob リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ca479-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca479-106">バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。</span><span class="sxs-lookup"><span data-stu-id="ca479-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="ca479-107">同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。</span><span class="sxs-lookup"><span data-stu-id="ca479-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="ca479-108">同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca479-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="ca479-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca479-109">Methods</span></span>

| <span data-ttu-id="ca479-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca479-110">Method</span></span>        | <span data-ttu-id="ca479-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ca479-111">Return Type</span></span>               | <span data-ttu-id="ca479-112">説明</span><span class="sxs-lookup"><span data-stu-id="ca479-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="ca479-113">List</span><span class="sxs-lookup"><span data-stu-id="ca479-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="ca479-114">[synchronizationJob](synchronization-synchronizationjob.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ca479-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="ca479-115">特定のアプリケーションのインスタンス (サービス主体) の既存のジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ca479-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="ca479-116">SynchronizationJob を取得します。</span><span class="sxs-lookup"><span data-stu-id="ca479-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="ca479-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="ca479-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="ca479-118">SynchronizationJob オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca479-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="ca479-119">Create</span><span class="sxs-lookup"><span data-stu-id="ca479-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="ca479-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="ca479-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="ca479-121">特定のアプリケーション用の新しいジョブを作成します。</span><span class="sxs-lookup"><span data-stu-id="ca479-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="ca479-122">Start</span><span class="sxs-lookup"><span data-stu-id="ca479-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="ca479-123">なし</span><span class="sxs-lookup"><span data-stu-id="ca479-123">None</span></span>   |<span data-ttu-id="ca479-124">同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="ca479-124">Start synchronization.</span></span> <span data-ttu-id="ca479-125">ジョブが一時停止状態にある場合は、ジョブが一時停止された時点から続行します。</span><span class="sxs-lookup"><span data-stu-id="ca479-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="ca479-126">ジョブは、検疫では、検疫の状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="ca479-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="ca479-127">Restart</span><span class="sxs-lookup"><span data-stu-id="ca479-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="ca479-128">なし</span><span class="sxs-lookup"><span data-stu-id="ca479-128">None</span></span>   |<span data-ttu-id="ca479-129">上で起動し、ディレクトリ内のすべてのオブジェクトを再処理するジョブを強制します。</span><span class="sxs-lookup"><span data-stu-id="ca479-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="ca479-130">Pause</span><span class="sxs-lookup"><span data-stu-id="ca479-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="ca479-131">なし</span><span class="sxs-lookup"><span data-stu-id="ca479-131">None</span></span>   |<span data-ttu-id="ca479-132">同期を一時的に停止します。</span><span class="sxs-lookup"><span data-stu-id="ca479-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="ca479-133">ジョブの状態を含むすべての進捗が保持され、ジョブが[起動](../api/synchronization-synchronizationjob-start.md)の呼び出しが行われる場合停止した位置から続行されます。</span><span class="sxs-lookup"><span data-stu-id="ca479-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="ca479-134">Delete</span><span class="sxs-lookup"><span data-stu-id="ca479-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="ca479-135">なし</span><span class="sxs-lookup"><span data-stu-id="ca479-135">None</span></span>   |<span data-ttu-id="ca479-136">同期を停止し、ジョブに関連付けられているすべての状態を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="ca479-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="ca479-137">SynchrnoizationSchema を取得します。</span><span class="sxs-lookup"><span data-stu-id="ca479-137">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="ca479-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="ca479-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="ca479-139">ジョブの効果的な同期スキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="ca479-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="ca479-140">SynchroizationSchema を更新します。</span><span class="sxs-lookup"><span data-stu-id="ca479-140">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="ca479-141">なし</span><span class="sxs-lookup"><span data-stu-id="ca479-141">None</span></span>   |<span data-ttu-id="ca479-142">ジョブの同期のスキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="ca479-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="ca479-143">資格情報を検証します。</span><span class="sxs-lookup"><span data-stu-id="ca479-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="ca479-144">なし</span><span class="sxs-lookup"><span data-stu-id="ca479-144">None</span></span>|<span data-ttu-id="ca479-145">ターゲット ディレクトリに対して指定された資格情報をテストします。</span><span class="sxs-lookup"><span data-stu-id="ca479-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca479-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca479-146">Properties</span></span>

| <span data-ttu-id="ca479-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca479-147">Property</span></span>      | <span data-ttu-id="ca479-148">型</span><span class="sxs-lookup"><span data-stu-id="ca479-148">Type</span></span>      | <span data-ttu-id="ca479-149">説明</span><span class="sxs-lookup"><span data-stu-id="ca479-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="ca479-150">id</span><span class="sxs-lookup"><span data-stu-id="ca479-150">id</span></span>             |<span data-ttu-id="ca479-151">String</span><span class="sxs-lookup"><span data-stu-id="ca479-151">String</span></span>                     |<span data-ttu-id="ca479-152">固有の同期ジョブの識別子です。</span><span class="sxs-lookup"><span data-stu-id="ca479-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="ca479-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ca479-153">Read-only.</span></span>|
|<span data-ttu-id="ca479-154">Schedule</span><span class="sxs-lookup"><span data-stu-id="ca479-154">schedule</span></span>       |[<span data-ttu-id="ca479-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="ca479-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="ca479-156">スケジュールがジョブを実行するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ca479-156">Schedule used to run the job.</span></span> <span data-ttu-id="ca479-157">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ca479-157">Read-only.</span></span>|
|<span data-ttu-id="ca479-158">status</span><span class="sxs-lookup"><span data-stu-id="ca479-158">status</span></span>         |[<span data-ttu-id="ca479-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="ca479-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="ca479-160">ジョブが前回実行されたときに、ジョブ、ジョブの現在の状態およびエラーの状態です。</span><span class="sxs-lookup"><span data-stu-id="ca479-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="ca479-161">templateId</span><span class="sxs-lookup"><span data-stu-id="ca479-161">templateId</span></span>     |<span data-ttu-id="ca479-162">文字列</span><span class="sxs-lookup"><span data-stu-id="ca479-162">String</span></span>    |<span data-ttu-id="ca479-163">このジョブで使用する[同期テンプレート](synchronization-synchronizationtemplate.md)の識別子です。</span><span class="sxs-lookup"><span data-stu-id="ca479-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca479-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca479-164">Relationships</span></span>
| <span data-ttu-id="ca479-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca479-165">Relationship</span></span> | <span data-ttu-id="ca479-166">型</span><span class="sxs-lookup"><span data-stu-id="ca479-166">Type</span></span>   |<span data-ttu-id="ca479-167">説明</span><span class="sxs-lookup"><span data-stu-id="ca479-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca479-168">スキーマ</span><span class="sxs-lookup"><span data-stu-id="ca479-168">schema</span></span>|[<span data-ttu-id="ca479-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="ca479-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="ca479-170">ジョブ用に構成された同期スキーマです。</span><span class="sxs-lookup"><span data-stu-id="ca479-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca479-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca479-171">JSON representation</span></span>

<span data-ttu-id="ca479-172">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ca479-172">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjob.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
