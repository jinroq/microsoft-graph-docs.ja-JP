---
title: 同期ジョブリソースの種類
description: バックグラウンドで定期的に実行して同期を実行し、1つのディレクトリに加えられた変更をポーリングして、別のディレクトリにプッシュします。 同期ジョブは、テナント内のアプリケーションの特定のインスタンスに対して常に固有です。 同期ジョブの設定の一部として、ターゲットディレクトリのオブジェクトの読み取りおよび書き込みの承認を付与し、ジョブの同期スキーマをカスタマイズする必要があります。
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580660"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="027c8-105">同期ジョブリソースの種類</span><span class="sxs-lookup"><span data-stu-id="027c8-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="027c8-106">バックグラウンドで定期的に実行して同期を実行し、1つのディレクトリに加えられた変更をポーリングして、別のディレクトリにプッシュします。</span><span class="sxs-lookup"><span data-stu-id="027c8-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="027c8-107">同期ジョブは、テナント内のアプリケーションの特定のインスタンスに対して常に固有です。</span><span class="sxs-lookup"><span data-stu-id="027c8-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="027c8-108">同期ジョブの設定の一部として、ターゲットディレクトリのオブジェクトの読み取りおよび書き込みの承認を付与し、ジョブの同期スキーマをカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="027c8-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="027c8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="027c8-109">Methods</span></span>

| <span data-ttu-id="027c8-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="027c8-110">Method</span></span>        | <span data-ttu-id="027c8-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="027c8-111">Return Type</span></span>               | <span data-ttu-id="027c8-112">説明</span><span class="sxs-lookup"><span data-stu-id="027c8-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="027c8-113">List</span><span class="sxs-lookup"><span data-stu-id="027c8-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="027c8-114">[同期ジョブ](synchronization-synchronizationjob.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="027c8-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="027c8-115">特定のアプリケーションインスタンス (サービスプリンシパル) の既存のジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="027c8-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="027c8-116">同期ジョブを取得する</span><span class="sxs-lookup"><span data-stu-id="027c8-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="027c8-117">同期ジョブ</span><span class="sxs-lookup"><span data-stu-id="027c8-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="027c8-118">同期ジョブオブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="027c8-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="027c8-119">作成</span><span class="sxs-lookup"><span data-stu-id="027c8-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="027c8-120">同期ジョブ</span><span class="sxs-lookup"><span data-stu-id="027c8-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="027c8-121">指定したアプリケーションの新しいジョブを作成します。</span><span class="sxs-lookup"><span data-stu-id="027c8-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="027c8-122">Start</span><span class="sxs-lookup"><span data-stu-id="027c8-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="027c8-123">なし</span><span class="sxs-lookup"><span data-stu-id="027c8-123">None</span></span>   |<span data-ttu-id="027c8-124">同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="027c8-124">Start synchronization.</span></span> <span data-ttu-id="027c8-125">ジョブが一時停止状態である場合、ジョブが一時停止した時点から続行されます。</span><span class="sxs-lookup"><span data-stu-id="027c8-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="027c8-126">ジョブが検疫されている場合は、検疫の状態はクリアされます。</span><span class="sxs-lookup"><span data-stu-id="027c8-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="027c8-127">Restart</span><span class="sxs-lookup"><span data-stu-id="027c8-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="027c8-128">なし</span><span class="sxs-lookup"><span data-stu-id="027c8-128">None</span></span>   |<span data-ttu-id="027c8-129">ジョブを強制的に開始し、ディレクトリ内のすべてのオブジェクトを再処理します。</span><span class="sxs-lookup"><span data-stu-id="027c8-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="027c8-130">Pause</span><span class="sxs-lookup"><span data-stu-id="027c8-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="027c8-131">なし</span><span class="sxs-lookup"><span data-stu-id="027c8-131">None</span></span>   |<span data-ttu-id="027c8-132">一時的に同期を停止します。</span><span class="sxs-lookup"><span data-stu-id="027c8-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="027c8-133">ジョブの状態を含むすべての進行状況が持続され、[開始](../api/synchronization-synchronizationjob-start.md)呼び出しが行われたときにジョブは中断したところから続行されます。</span><span class="sxs-lookup"><span data-stu-id="027c8-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="027c8-134">削除</span><span class="sxs-lookup"><span data-stu-id="027c8-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="027c8-135">なし</span><span class="sxs-lookup"><span data-stu-id="027c8-135">None</span></span>   |<span data-ttu-id="027c8-136">同期を停止し、ジョブに関連付けられているすべての状態を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="027c8-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="027c8-137">synchrnoizationSchema を取得する</span><span class="sxs-lookup"><span data-stu-id="027c8-137">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="027c8-138">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="027c8-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="027c8-139">ジョブの有効な同期スキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="027c8-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="027c8-140">synchroizationSchema の更新</span><span class="sxs-lookup"><span data-stu-id="027c8-140">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="027c8-141">なし</span><span class="sxs-lookup"><span data-stu-id="027c8-141">None</span></span>   |<span data-ttu-id="027c8-142">ジョブの同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="027c8-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="027c8-143">資格情報を検証する</span><span class="sxs-lookup"><span data-stu-id="027c8-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="027c8-144">なし</span><span class="sxs-lookup"><span data-stu-id="027c8-144">None</span></span>|<span data-ttu-id="027c8-145">ターゲットディレクトリに対して提供された資格情報をテストします。</span><span class="sxs-lookup"><span data-stu-id="027c8-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="027c8-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="027c8-146">Properties</span></span>

| <span data-ttu-id="027c8-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="027c8-147">Property</span></span>      | <span data-ttu-id="027c8-148">型</span><span class="sxs-lookup"><span data-stu-id="027c8-148">Type</span></span>      | <span data-ttu-id="027c8-149">説明</span><span class="sxs-lookup"><span data-stu-id="027c8-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="027c8-150">id</span><span class="sxs-lookup"><span data-stu-id="027c8-150">id</span></span>             |<span data-ttu-id="027c8-151">String</span><span class="sxs-lookup"><span data-stu-id="027c8-151">String</span></span>                     |<span data-ttu-id="027c8-152">一意の同期ジョブ識別子。</span><span class="sxs-lookup"><span data-stu-id="027c8-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="027c8-153">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="027c8-153">Read-only.</span></span>|
|<span data-ttu-id="027c8-154">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="027c8-154">schedule</span></span>       |[<span data-ttu-id="027c8-155">同期スケジュール</span><span class="sxs-lookup"><span data-stu-id="027c8-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="027c8-156">ジョブを実行するために使用するスケジュール。</span><span class="sxs-lookup"><span data-stu-id="027c8-156">Schedule used to run the job.</span></span> <span data-ttu-id="027c8-157">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="027c8-157">Read-only.</span></span>|
|<span data-ttu-id="027c8-158">status</span><span class="sxs-lookup"><span data-stu-id="027c8-158">status</span></span>         |[<span data-ttu-id="027c8-159">同期の状態</span><span class="sxs-lookup"><span data-stu-id="027c8-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="027c8-160">ジョブの状態。ジョブが最後に実行された日時、現在のジョブの状態、エラーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="027c8-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="027c8-161">templateId</span><span class="sxs-lookup"><span data-stu-id="027c8-161">templateId</span></span>     |<span data-ttu-id="027c8-162">String</span><span class="sxs-lookup"><span data-stu-id="027c8-162">String</span></span>    |<span data-ttu-id="027c8-163">このジョブの基になっている[同期テンプレート](synchronization-synchronizationtemplate.md)の識別子。</span><span class="sxs-lookup"><span data-stu-id="027c8-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="027c8-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="027c8-164">Relationships</span></span>
| <span data-ttu-id="027c8-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="027c8-165">Relationship</span></span> | <span data-ttu-id="027c8-166">型</span><span class="sxs-lookup"><span data-stu-id="027c8-166">Type</span></span>   |<span data-ttu-id="027c8-167">説明</span><span class="sxs-lookup"><span data-stu-id="027c8-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="027c8-168">スキーマ</span><span class="sxs-lookup"><span data-stu-id="027c8-168">schema</span></span>|[<span data-ttu-id="027c8-169">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="027c8-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="027c8-170">ジョブに対して構成されている同期スキーマ。</span><span class="sxs-lookup"><span data-stu-id="027c8-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="027c8-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="027c8-171">JSON representation</span></span>

<span data-ttu-id="027c8-172">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="027c8-172">The following is a JSON representation of the resource.</span></span>

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
