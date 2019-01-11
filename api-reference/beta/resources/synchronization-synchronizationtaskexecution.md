---
title: synchronizationTaskExecution リソースの種類
description: 同期ジョブの実行の結果をまとめたものです。
localization_priority: Normal
ms.openlocfilehash: 99b6c66b15577ee4c6cbbf5ffe44e17cf0672696
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851507"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="eee59-103">synchronizationTaskExecution リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eee59-103">synchronizationTaskExecution resource type</span></span>

> <span data-ttu-id="eee59-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eee59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eee59-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eee59-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eee59-106">同期ジョブの実行の結果をまとめたものです。</span><span class="sxs-lookup"><span data-stu-id="eee59-106">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="eee59-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eee59-107">Properties</span></span>
| <span data-ttu-id="eee59-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eee59-108">Property</span></span>     | <span data-ttu-id="eee59-109">種類</span><span class="sxs-lookup"><span data-stu-id="eee59-109">Type</span></span>   |<span data-ttu-id="eee59-110">説明</span><span class="sxs-lookup"><span data-stu-id="eee59-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eee59-111">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="eee59-111">activityIdentifier</span></span>           |<span data-ttu-id="eee59-112">String</span><span class="sxs-lookup"><span data-stu-id="eee59-112">String</span></span> |<span data-ttu-id="eee59-113">実行ジョブの識別子です。</span><span class="sxs-lookup"><span data-stu-id="eee59-113">Identifier of the job run.</span></span>|
|<span data-ttu-id="eee59-114">countEntitled</span><span class="sxs-lookup"><span data-stu-id="eee59-114">countEntitled</span></span>                |<span data-ttu-id="eee59-115">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-115">Int64</span></span>  |<span data-ttu-id="eee59-116">このアプリケーションに割り当てられた処理されたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="eee59-116">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="eee59-117">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="eee59-117">countEntitledForProvisioning</span></span> |<span data-ttu-id="eee59-118">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-118">Int64</span></span>  |<span data-ttu-id="eee59-119">プロビジョニング用に割り当てられた処理されたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="eee59-119">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="eee59-120">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="eee59-120">countEscrowed</span></span>                |<span data-ttu-id="eee59-121">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-121">Int64</span></span>  |<span data-ttu-id="eee59-122">Escrowed (エラー) のエントリの数。</span><span class="sxs-lookup"><span data-stu-id="eee59-122">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="eee59-123">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="eee59-123">countEscrowedRaw</span></span>             |<span data-ttu-id="eee59-124">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-124">Int64</span></span>  |<span data-ttu-id="eee59-125">Escrows のシステムで生成されたを含む、escrowed されたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="eee59-125">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="eee59-126">countExported</span><span class="sxs-lookup"><span data-stu-id="eee59-126">countExported</span></span>                |<span data-ttu-id="eee59-127">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-127">Int64</span></span>  |<span data-ttu-id="eee59-128">エクスポートされたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="eee59-128">Count of exported entries.</span></span>|
|<span data-ttu-id="eee59-129">countExports</span><span class="sxs-lookup"><span data-stu-id="eee59-129">countExports</span></span>                 |<span data-ttu-id="eee59-130">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-130">Int64</span></span>  |<span data-ttu-id="eee59-131">エクスポートする必要があるエントリの数です。</span><span class="sxs-lookup"><span data-stu-id="eee59-131">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="eee59-132">countImported</span><span class="sxs-lookup"><span data-stu-id="eee59-132">countImported</span></span>                |<span data-ttu-id="eee59-133">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-133">Int64</span></span>  |<span data-ttu-id="eee59-134">インポートされたエントリの数。</span><span class="sxs-lookup"><span data-stu-id="eee59-134">Count of imported entries.</span></span>|
|<span data-ttu-id="eee59-135">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="eee59-135">countImportedDeltas</span></span>          |<span data-ttu-id="eee59-136">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-136">Int64</span></span>  |<span data-ttu-id="eee59-137">インポートの差分変更の数です。</span><span class="sxs-lookup"><span data-stu-id="eee59-137">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="eee59-138">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="eee59-138">countImportedReferenceDeltas</span></span> |<span data-ttu-id="eee59-139">Int64</span><span class="sxs-lookup"><span data-stu-id="eee59-139">Int64</span></span>  |<span data-ttu-id="eee59-140">参照の変更に関連するインポートされたデルタの変更の数です。</span><span class="sxs-lookup"><span data-stu-id="eee59-140">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="eee59-141">エラー</span><span class="sxs-lookup"><span data-stu-id="eee59-141">error</span></span>                        |[<span data-ttu-id="eee59-142">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="eee59-142">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="eee59-143">エラーが発生した場合に、詳細を含む、 **synchronizationError**オブジェクトが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eee59-143">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="eee59-144">state</span><span class="sxs-lookup"><span data-stu-id="eee59-144">state</span></span>                        |<span data-ttu-id="eee59-145">String</span><span class="sxs-lookup"><span data-stu-id="eee59-145">String</span></span> |<span data-ttu-id="eee59-146">コードがこの実行の結果を要約します。</span><span class="sxs-lookup"><span data-stu-id="eee59-146">Code summarizing the result of this run.</span></span> <span data-ttu-id="eee59-147">可能な値は、`Succeeded`、`Failed`、`EntryLevelErrors` です。</span><span class="sxs-lookup"><span data-stu-id="eee59-147">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="eee59-148">timeBegan</span><span class="sxs-lookup"><span data-stu-id="eee59-148">timeBegan</span></span>                    |<span data-ttu-id="eee59-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eee59-149">DateTimeOffset</span></span>|<span data-ttu-id="eee59-150">このジョブの実行を開始したときの時間です。</span><span class="sxs-lookup"><span data-stu-id="eee59-150">Time when this job run began.</span></span> <span data-ttu-id="eee59-151">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="eee59-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eee59-152">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eee59-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="eee59-153">timeEnded</span><span class="sxs-lookup"><span data-stu-id="eee59-153">timeEnded</span></span>                    |<span data-ttu-id="eee59-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eee59-154">DateTimeOffset</span></span>|<span data-ttu-id="eee59-155">このジョブを実行すると時間が終了しました。</span><span class="sxs-lookup"><span data-stu-id="eee59-155">Time when this job run ended.</span></span> <span data-ttu-id="eee59-156">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="eee59-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eee59-157">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eee59-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eee59-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eee59-158">JSON representation</span></span>

<span data-ttu-id="eee59-159">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eee59-159">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
