---
title: プロセスリソースの種類
description: 通知に関連するプロセスに関するステートフルな情報を含みます。
localization_priority: Normal
ms.openlocfilehash: 0b4207c1780dfd6327ceb67e837f793341e609ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579875"
---
# <a name="process-resource-type"></a><span data-ttu-id="f3893-103">プロセスリソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3893-103">process resource type</span></span>

<span data-ttu-id="f3893-104">通知に関連するプロセスに関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="f3893-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="f3893-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3893-105">Properties</span></span>

| <span data-ttu-id="f3893-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3893-106">Property</span></span>   | <span data-ttu-id="f3893-107">型</span><span class="sxs-lookup"><span data-stu-id="f3893-107">Type</span></span>|<span data-ttu-id="f3893-108">説明</span><span class="sxs-lookup"><span data-stu-id="f3893-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3893-109">accountName</span><span class="sxs-lookup"><span data-stu-id="f3893-109">accountName</span></span>|<span data-ttu-id="f3893-110">String</span><span class="sxs-lookup"><span data-stu-id="f3893-110">String</span></span>|<span data-ttu-id="f3893-111">ユーザーアカウント識別子 (アカウントの下で実行されたユーザーアカウントコンテキスト)。たとえば、AccountName、SID など。</span><span class="sxs-lookup"><span data-stu-id="f3893-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="f3893-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="f3893-112">commandLine</span></span>|<span data-ttu-id="f3893-113">String</span><span class="sxs-lookup"><span data-stu-id="f3893-113">String</span></span>|<span data-ttu-id="f3893-114">すべてのパラメーターを含む完全なプロセス呼び出しの commandline。</span><span class="sxs-lookup"><span data-stu-id="f3893-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="f3893-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3893-115">createdDateTime</span></span>|<span data-ttu-id="f3893-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3893-116">DateTimeOffset</span></span>|<span data-ttu-id="f3893-117">プロセスが開始された時刻。</span><span class="sxs-lookup"><span data-stu-id="f3893-117">Time at which the process was started.</span></span> <span data-ttu-id="f3893-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f3893-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f3893-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f3893-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f3893-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="f3893-120">fileHash</span></span>|[<span data-ttu-id="f3893-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="f3893-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="f3893-122">ファイルハッシュを含む複合型 (暗号化と場所に依存)。</span><span class="sxs-lookup"><span data-stu-id="f3893-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="f3893-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="f3893-123">integrityLevel</span></span>|<span data-ttu-id="f3893-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="f3893-124">processIntegrityLevel</span></span>|<span data-ttu-id="f3893-125">プロセスの整合性レベル。</span><span class="sxs-lookup"><span data-stu-id="f3893-125">The integrity level of the process.</span></span> <span data-ttu-id="f3893-126">使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="f3893-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="f3893-127">isElevated</span><span class="sxs-lookup"><span data-stu-id="f3893-127">isElevated</span></span>|<span data-ttu-id="f3893-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3893-128">Boolean</span></span>|<span data-ttu-id="f3893-129">プロセスが昇格された場合は True。</span><span class="sxs-lookup"><span data-stu-id="f3893-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="f3893-130">name</span><span class="sxs-lookup"><span data-stu-id="f3893-130">name</span></span>|<span data-ttu-id="f3893-131">String</span><span class="sxs-lookup"><span data-stu-id="f3893-131">String</span></span>|<span data-ttu-id="f3893-132">プロセスのイメージファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="f3893-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="f3893-133">parentprocess/datetime</span><span class="sxs-lookup"><span data-stu-id="f3893-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="f3893-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3893-134">DateTimeOffset</span></span>|<span data-ttu-id="f3893-135">親プロセスが開始された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f3893-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="f3893-136">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f3893-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f3893-137">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f3893-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f3893-138">parentprocessid</span><span class="sxs-lookup"><span data-stu-id="f3893-138">parentProcessId</span></span>|<span data-ttu-id="f3893-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f3893-139">Int32</span></span>|<span data-ttu-id="f3893-140">親プロセスのプロセス ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="f3893-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="f3893-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="f3893-141">parentProcessName</span></span>|<span data-ttu-id="f3893-142">String</span><span class="sxs-lookup"><span data-stu-id="f3893-142">String</span></span>|<span data-ttu-id="f3893-143">親プロセスのイメージファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="f3893-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="f3893-144">path</span><span class="sxs-lookup"><span data-stu-id="f3893-144">path</span></span>|<span data-ttu-id="f3893-145">String</span><span class="sxs-lookup"><span data-stu-id="f3893-145">String</span></span>|<span data-ttu-id="f3893-146">ファイル名を含む完全なパス。</span><span class="sxs-lookup"><span data-stu-id="f3893-146">Full path, including filename.</span></span>|
|<span data-ttu-id="f3893-147">processId</span><span class="sxs-lookup"><span data-stu-id="f3893-147">processId</span></span>|<span data-ttu-id="f3893-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f3893-148">Int32</span></span>|<span data-ttu-id="f3893-149">プロセスのプロセス ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="f3893-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3893-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3893-150">JSON representation</span></span>

<span data-ttu-id="f3893-151">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f3893-151">The following is a JSON representation of the resource.</span></span>

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
