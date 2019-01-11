---
title: プロセス リソースの種類
description: ステートフルなアラートに関連するプロセスについてを説明します。
localization_priority: Normal
ms.openlocfilehash: 0b4207c1780dfd6327ceb67e837f793341e609ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864422"
---
# <a name="process-resource-type"></a><span data-ttu-id="96cae-103">プロセス リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96cae-103">process resource type</span></span>

<span data-ttu-id="96cae-104">ステートフルなアラートに関連するプロセスについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="96cae-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="96cae-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96cae-105">Properties</span></span>

| <span data-ttu-id="96cae-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96cae-106">Property</span></span>   | <span data-ttu-id="96cae-107">種類</span><span class="sxs-lookup"><span data-stu-id="96cae-107">Type</span></span>|<span data-ttu-id="96cae-108">説明</span><span class="sxs-lookup"><span data-stu-id="96cae-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96cae-109">accountName</span><span class="sxs-lookup"><span data-stu-id="96cae-109">accountName</span></span>|<span data-ttu-id="96cae-110">String</span><span class="sxs-lookup"><span data-stu-id="96cae-110">String</span></span>|<span data-ttu-id="96cae-111">ユーザーは、例、アカウント名、SID、およびように識別子 (ユーザー アカウントのコンテキストでプロセスが実行された) を考慮します。</span><span class="sxs-lookup"><span data-stu-id="96cae-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="96cae-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="96cae-112">commandLine</span></span>|<span data-ttu-id="96cae-113">String</span><span class="sxs-lookup"><span data-stu-id="96cae-113">String</span></span>|<span data-ttu-id="96cae-114">完全な処理の呼び出しは、すべてのパラメーターを含むを使用できます。</span><span class="sxs-lookup"><span data-stu-id="96cae-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="96cae-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96cae-115">createdDateTime</span></span>|<span data-ttu-id="96cae-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96cae-116">DateTimeOffset</span></span>|<span data-ttu-id="96cae-117">プロセスが開始された時刻です。</span><span class="sxs-lookup"><span data-stu-id="96cae-117">Time at which the process was started.</span></span> <span data-ttu-id="96cae-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="96cae-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96cae-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96cae-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="96cae-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="96cae-120">fileHash</span></span>|[<span data-ttu-id="96cae-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="96cae-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="96cae-122">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="96cae-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="96cae-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="96cae-123">integrityLevel</span></span>|<span data-ttu-id="96cae-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="96cae-124">processIntegrityLevel</span></span>|<span data-ttu-id="96cae-125">プロセスの整合性レベルです。</span><span class="sxs-lookup"><span data-stu-id="96cae-125">The integrity level of the process.</span></span> <span data-ttu-id="96cae-126">使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="96cae-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="96cae-127">isElevated</span><span class="sxs-lookup"><span data-stu-id="96cae-127">isElevated</span></span>|<span data-ttu-id="96cae-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="96cae-128">Boolean</span></span>|<span data-ttu-id="96cae-129">プロセスが昇格した場合は true。</span><span class="sxs-lookup"><span data-stu-id="96cae-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="96cae-130">名前</span><span class="sxs-lookup"><span data-stu-id="96cae-130">name</span></span>|<span data-ttu-id="96cae-131">String</span><span class="sxs-lookup"><span data-stu-id="96cae-131">String</span></span>|<span data-ttu-id="96cae-132">プロセスのイメージ ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="96cae-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="96cae-133">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="96cae-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="96cae-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96cae-134">DateTimeOffset</span></span>|<span data-ttu-id="96cae-135">親プロセスの開始日時。</span><span class="sxs-lookup"><span data-stu-id="96cae-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="96cae-136">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="96cae-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96cae-137">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96cae-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="96cae-138">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="96cae-138">parentProcessId</span></span>|<span data-ttu-id="96cae-139">Int32</span><span class="sxs-lookup"><span data-stu-id="96cae-139">Int32</span></span>|<span data-ttu-id="96cae-140">プロセス ID (PID) の親プロセスです。</span><span class="sxs-lookup"><span data-stu-id="96cae-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="96cae-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="96cae-141">parentProcessName</span></span>|<span data-ttu-id="96cae-142">String</span><span class="sxs-lookup"><span data-stu-id="96cae-142">String</span></span>|<span data-ttu-id="96cae-143">親プロセスのイメージ ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="96cae-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="96cae-144">path</span><span class="sxs-lookup"><span data-stu-id="96cae-144">path</span></span>|<span data-ttu-id="96cae-145">String</span><span class="sxs-lookup"><span data-stu-id="96cae-145">String</span></span>|<span data-ttu-id="96cae-146">ファイル名を含む完全パスです。</span><span class="sxs-lookup"><span data-stu-id="96cae-146">Full path, including filename.</span></span>|
|<span data-ttu-id="96cae-147">プロセス Id</span><span class="sxs-lookup"><span data-stu-id="96cae-147">processId</span></span>|<span data-ttu-id="96cae-148">Int32</span><span class="sxs-lookup"><span data-stu-id="96cae-148">Int32</span></span>|<span data-ttu-id="96cae-149">プロセス ID (PID) のプロセスです。</span><span class="sxs-lookup"><span data-stu-id="96cae-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96cae-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96cae-150">JSON representation</span></span>

<span data-ttu-id="96cae-151">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96cae-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
