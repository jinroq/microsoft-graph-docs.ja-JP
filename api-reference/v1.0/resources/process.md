---
title: プロセスリソースの種類
description: 通知に関連するプロセスに関するステートフルな情報を含みます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ccaf2e3048fc26573e9599a515aabf391dda6d58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035085"
---
# <a name="process-resource-type"></a><span data-ttu-id="bfc23-103">プロセスリソースの種類</span><span class="sxs-lookup"><span data-stu-id="bfc23-103">process resource type</span></span>

<span data-ttu-id="bfc23-104">通知に関連するプロセスに関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="bfc23-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="bfc23-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfc23-105">Properties</span></span>

| <span data-ttu-id="bfc23-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfc23-106">Property</span></span>   | <span data-ttu-id="bfc23-107">型</span><span class="sxs-lookup"><span data-stu-id="bfc23-107">Type</span></span>|<span data-ttu-id="bfc23-108">説明</span><span class="sxs-lookup"><span data-stu-id="bfc23-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfc23-109">accountName</span><span class="sxs-lookup"><span data-stu-id="bfc23-109">accountName</span></span>|<span data-ttu-id="bfc23-110">String</span><span class="sxs-lookup"><span data-stu-id="bfc23-110">String</span></span>|<span data-ttu-id="bfc23-111">ユーザーアカウント識別子 (アカウントの下で実行されたユーザーアカウントコンテキスト)。たとえば、AccountName、SID など。</span><span class="sxs-lookup"><span data-stu-id="bfc23-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="bfc23-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="bfc23-112">commandLine</span></span>|<span data-ttu-id="bfc23-113">String</span><span class="sxs-lookup"><span data-stu-id="bfc23-113">String</span></span>|<span data-ttu-id="bfc23-114">すべてのパラメーターを含む完全なプロセス呼び出しの commandline。</span><span class="sxs-lookup"><span data-stu-id="bfc23-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="bfc23-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfc23-115">createdDateTime</span></span>|<span data-ttu-id="bfc23-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfc23-116">DateTimeOffset</span></span>|<span data-ttu-id="bfc23-117">プロセスが開始された時刻。</span><span class="sxs-lookup"><span data-stu-id="bfc23-117">Time at which the process was started.</span></span> <span data-ttu-id="bfc23-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="bfc23-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfc23-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfc23-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bfc23-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="bfc23-120">fileHash</span></span>|[<span data-ttu-id="bfc23-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="bfc23-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="bfc23-122">ファイルハッシュを含む複合型 (暗号化と場所に依存)。</span><span class="sxs-lookup"><span data-stu-id="bfc23-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="bfc23-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="bfc23-123">integrityLevel</span></span>|<span data-ttu-id="bfc23-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="bfc23-124">processIntegrityLevel</span></span>|<span data-ttu-id="bfc23-125">プロセスの整合性レベル。</span><span class="sxs-lookup"><span data-stu-id="bfc23-125">The integrity level of the process.</span></span> <span data-ttu-id="bfc23-126">使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="bfc23-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="bfc23-127">isElevated</span><span class="sxs-lookup"><span data-stu-id="bfc23-127">isElevated</span></span>|<span data-ttu-id="bfc23-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfc23-128">Boolean</span></span>|<span data-ttu-id="bfc23-129">プロセスが昇格された場合は True。</span><span class="sxs-lookup"><span data-stu-id="bfc23-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="bfc23-130">name</span><span class="sxs-lookup"><span data-stu-id="bfc23-130">name</span></span>|<span data-ttu-id="bfc23-131">String</span><span class="sxs-lookup"><span data-stu-id="bfc23-131">String</span></span>|<span data-ttu-id="bfc23-132">プロセスのイメージファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="bfc23-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="bfc23-133">Parentprocess/Datetime</span><span class="sxs-lookup"><span data-stu-id="bfc23-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="bfc23-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfc23-134">DateTimeOffset</span></span>|<span data-ttu-id="bfc23-135">親プロセスが開始された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bfc23-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="bfc23-136">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="bfc23-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfc23-137">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfc23-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bfc23-138">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="bfc23-138">parentProcessId</span></span>|<span data-ttu-id="bfc23-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bfc23-139">Int32</span></span>|<span data-ttu-id="bfc23-140">親プロセスのプロセス ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="bfc23-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="bfc23-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="bfc23-141">parentProcessName</span></span>|<span data-ttu-id="bfc23-142">String</span><span class="sxs-lookup"><span data-stu-id="bfc23-142">String</span></span>|<span data-ttu-id="bfc23-143">親プロセスのイメージファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="bfc23-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="bfc23-144">path</span><span class="sxs-lookup"><span data-stu-id="bfc23-144">path</span></span>|<span data-ttu-id="bfc23-145">String</span><span class="sxs-lookup"><span data-stu-id="bfc23-145">String</span></span>|<span data-ttu-id="bfc23-146">ファイル名を含む完全なパス。</span><span class="sxs-lookup"><span data-stu-id="bfc23-146">Full path, including filename.</span></span>|
|<span data-ttu-id="bfc23-147">processId</span><span class="sxs-lookup"><span data-stu-id="bfc23-147">processId</span></span>|<span data-ttu-id="bfc23-148">Int32</span><span class="sxs-lookup"><span data-stu-id="bfc23-148">Int32</span></span>|<span data-ttu-id="bfc23-149">プロセスのプロセス ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="bfc23-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfc23-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bfc23-150">JSON representation</span></span>

<span data-ttu-id="bfc23-151">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bfc23-151">The following is a JSON representation of the resource.</span></span>

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
