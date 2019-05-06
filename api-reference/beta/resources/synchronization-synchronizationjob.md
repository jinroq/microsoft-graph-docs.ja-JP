---
title: 同期ジョブリソースの種類
description: バックグラウンドで定期的に実行して同期を実行し、1つのディレクトリに加えられた変更をポーリングして、別のディレクトリにプッシュします。 同期ジョブは、テナント内のアプリケーションの特定のインスタンスに対して常に固有です。 同期ジョブの設定の一部として、ターゲットディレクトリのオブジェクトの読み取りおよび書き込みの承認を付与し、ジョブの同期スキーマをカスタマイズする必要があります。
localization_priority: Normal
ms.openlocfilehash: 186df51b9a2a941d6c27cda03895423e311fb0b0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620830"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="aad3c-105">同期ジョブリソースの種類</span><span class="sxs-lookup"><span data-stu-id="aad3c-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aad3c-106">バックグラウンドで定期的に実行して同期を実行し、1つのディレクトリに加えられた変更をポーリングして、別のディレクトリにプッシュします。</span><span class="sxs-lookup"><span data-stu-id="aad3c-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="aad3c-107">同期ジョブは、テナント内のアプリケーションの特定のインスタンスに対して常に固有です。</span><span class="sxs-lookup"><span data-stu-id="aad3c-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="aad3c-108">同期ジョブの設定の一部として、ターゲットディレクトリのオブジェクトの読み取りおよび書き込みの承認を付与し、ジョブの同期スキーマをカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="aad3c-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="aad3c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="aad3c-109">Methods</span></span>

| <span data-ttu-id="aad3c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="aad3c-110">Method</span></span>        | <span data-ttu-id="aad3c-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aad3c-111">Return Type</span></span>               | <span data-ttu-id="aad3c-112">説明</span><span class="sxs-lookup"><span data-stu-id="aad3c-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="aad3c-113">List</span><span class="sxs-lookup"><span data-stu-id="aad3c-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="aad3c-114">[同期ジョブ](synchronization-synchronizationjob.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="aad3c-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="aad3c-115">特定のアプリケーションインスタンス (サービスプリンシパル) の既存のジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="aad3c-116">同期ジョブを取得する</span><span class="sxs-lookup"><span data-stu-id="aad3c-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="aad3c-117">同期ジョブ</span><span class="sxs-lookup"><span data-stu-id="aad3c-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="aad3c-118">同期ジョブオブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aad3c-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="aad3c-119">Create</span><span class="sxs-lookup"><span data-stu-id="aad3c-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="aad3c-120">同期ジョブ</span><span class="sxs-lookup"><span data-stu-id="aad3c-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="aad3c-121">指定したアプリケーションの新しいジョブを作成します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="aad3c-122">Start</span><span class="sxs-lookup"><span data-stu-id="aad3c-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="aad3c-123">なし</span><span class="sxs-lookup"><span data-stu-id="aad3c-123">None</span></span>   |<span data-ttu-id="aad3c-124">同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-124">Start synchronization.</span></span> <span data-ttu-id="aad3c-125">ジョブが一時停止状態である場合、ジョブが一時停止した時点から続行されます。</span><span class="sxs-lookup"><span data-stu-id="aad3c-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="aad3c-126">ジョブが検疫されている場合は、検疫の状態はクリアされます。</span><span class="sxs-lookup"><span data-stu-id="aad3c-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="aad3c-127">Restart</span><span class="sxs-lookup"><span data-stu-id="aad3c-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="aad3c-128">なし</span><span class="sxs-lookup"><span data-stu-id="aad3c-128">None</span></span>   |<span data-ttu-id="aad3c-129">ジョブを強制的に開始し、ディレクトリ内のすべてのオブジェクトを再処理します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="aad3c-130">Pause</span><span class="sxs-lookup"><span data-stu-id="aad3c-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="aad3c-131">なし</span><span class="sxs-lookup"><span data-stu-id="aad3c-131">None</span></span>   |<span data-ttu-id="aad3c-132">一時的に同期を停止します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="aad3c-133">ジョブの状態を含むすべての進行状況が持続され、[開始](../api/synchronization-synchronizationjob-start.md)呼び出しが行われたときにジョブは中断したところから続行されます。</span><span class="sxs-lookup"><span data-stu-id="aad3c-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="aad3c-134">削除</span><span class="sxs-lookup"><span data-stu-id="aad3c-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="aad3c-135">なし</span><span class="sxs-lookup"><span data-stu-id="aad3c-135">None</span></span>   |<span data-ttu-id="aad3c-136">同期を停止し、ジョブに関連付けられているすべての状態を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="aad3c-137">同期スキーマを取得する</span><span class="sxs-lookup"><span data-stu-id="aad3c-137">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="aad3c-138">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="aad3c-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="aad3c-139">ジョブの有効な同期スキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="aad3c-140">同期スキーマの更新</span><span class="sxs-lookup"><span data-stu-id="aad3c-140">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="aad3c-141">なし</span><span class="sxs-lookup"><span data-stu-id="aad3c-141">None</span></span>   |<span data-ttu-id="aad3c-142">ジョブの同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="aad3c-143">資格情報を検証する</span><span class="sxs-lookup"><span data-stu-id="aad3c-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="aad3c-144">なし</span><span class="sxs-lookup"><span data-stu-id="aad3c-144">None</span></span>|<span data-ttu-id="aad3c-145">ターゲットディレクトリに対して提供された資格情報をテストします。</span><span class="sxs-lookup"><span data-stu-id="aad3c-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="aad3c-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aad3c-146">Properties</span></span>

| <span data-ttu-id="aad3c-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aad3c-147">Property</span></span>      | <span data-ttu-id="aad3c-148">型</span><span class="sxs-lookup"><span data-stu-id="aad3c-148">Type</span></span>      | <span data-ttu-id="aad3c-149">説明</span><span class="sxs-lookup"><span data-stu-id="aad3c-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="aad3c-150">id</span><span class="sxs-lookup"><span data-stu-id="aad3c-150">id</span></span>             |<span data-ttu-id="aad3c-151">String</span><span class="sxs-lookup"><span data-stu-id="aad3c-151">String</span></span>                     |<span data-ttu-id="aad3c-152">一意の同期ジョブ識別子。</span><span class="sxs-lookup"><span data-stu-id="aad3c-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="aad3c-153">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aad3c-153">Read-only.</span></span>|
|<span data-ttu-id="aad3c-154">schedule</span><span class="sxs-lookup"><span data-stu-id="aad3c-154">schedule</span></span>       |[<span data-ttu-id="aad3c-155">同期スケジュール</span><span class="sxs-lookup"><span data-stu-id="aad3c-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="aad3c-156">ジョブを実行するために使用するスケジュール。</span><span class="sxs-lookup"><span data-stu-id="aad3c-156">Schedule used to run the job.</span></span> <span data-ttu-id="aad3c-157">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aad3c-157">Read-only.</span></span>|
|<span data-ttu-id="aad3c-158">status</span><span class="sxs-lookup"><span data-stu-id="aad3c-158">status</span></span>         |[<span data-ttu-id="aad3c-159">同期の状態</span><span class="sxs-lookup"><span data-stu-id="aad3c-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="aad3c-160">ジョブの状態。ジョブが最後に実行された日時、現在のジョブの状態、エラーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="aad3c-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="aad3c-161">templateId</span><span class="sxs-lookup"><span data-stu-id="aad3c-161">templateId</span></span>     |<span data-ttu-id="aad3c-162">String</span><span class="sxs-lookup"><span data-stu-id="aad3c-162">String</span></span>    |<span data-ttu-id="aad3c-163">このジョブの基になっている[同期テンプレート](synchronization-synchronizationtemplate.md)の識別子。</span><span class="sxs-lookup"><span data-stu-id="aad3c-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aad3c-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aad3c-164">Relationships</span></span>
| <span data-ttu-id="aad3c-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aad3c-165">Relationship</span></span> | <span data-ttu-id="aad3c-166">型</span><span class="sxs-lookup"><span data-stu-id="aad3c-166">Type</span></span>   |<span data-ttu-id="aad3c-167">説明</span><span class="sxs-lookup"><span data-stu-id="aad3c-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aad3c-168">スキーマ</span><span class="sxs-lookup"><span data-stu-id="aad3c-168">schema</span></span>|[<span data-ttu-id="aad3c-169">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="aad3c-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="aad3c-170">ジョブに対して構成されている同期スキーマ。</span><span class="sxs-lookup"><span data-stu-id="aad3c-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aad3c-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aad3c-171">JSON representation</span></span>

<span data-ttu-id="aad3c-172">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aad3c-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
