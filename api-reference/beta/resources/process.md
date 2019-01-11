---
title: プロセス リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 36acd6ed0f6e2cee5095d445de3ba4ff024a024a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869469"
---
# <a name="process-resource-type"></a><span data-ttu-id="29de0-104">プロセス リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29de0-104">process resource type</span></span>

 > <span data-ttu-id="29de0-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29de0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29de0-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29de0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29de0-107">ステートフルなアラートに関連するプロセスについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="29de0-107">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="29de0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29de0-108">Properties</span></span>

| <span data-ttu-id="29de0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29de0-109">Property</span></span>   | <span data-ttu-id="29de0-110">種類</span><span class="sxs-lookup"><span data-stu-id="29de0-110">Type</span></span>|<span data-ttu-id="29de0-111">説明</span><span class="sxs-lookup"><span data-stu-id="29de0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29de0-112">accountName</span><span class="sxs-lookup"><span data-stu-id="29de0-112">accountName</span></span>|<span data-ttu-id="29de0-113">String</span><span class="sxs-lookup"><span data-stu-id="29de0-113">String</span></span>|<span data-ttu-id="29de0-114">ユーザーは、例、アカウント名、SID、およびように識別子 (ユーザー アカウントのコンテキストでプロセスが実行された) を考慮します。</span><span class="sxs-lookup"><span data-stu-id="29de0-114">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="29de0-115">commandLine</span><span class="sxs-lookup"><span data-stu-id="29de0-115">commandLine</span></span>|<span data-ttu-id="29de0-116">String</span><span class="sxs-lookup"><span data-stu-id="29de0-116">String</span></span>|<span data-ttu-id="29de0-117">完全な処理の呼び出しは、すべてのパラメーターを含むを使用できます。</span><span class="sxs-lookup"><span data-stu-id="29de0-117">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="29de0-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29de0-118">createdDateTime</span></span>|<span data-ttu-id="29de0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29de0-119">DateTimeOffset</span></span>|<span data-ttu-id="29de0-120">プロセスが開始された時刻です。</span><span class="sxs-lookup"><span data-stu-id="29de0-120">Time at which the process was started.</span></span> <span data-ttu-id="29de0-121">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="29de0-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29de0-122">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="29de0-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="29de0-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="29de0-123">fileHash</span></span>|[<span data-ttu-id="29de0-124">fileHash</span><span class="sxs-lookup"><span data-stu-id="29de0-124">fileHash</span></span>](filehash.md)|<span data-ttu-id="29de0-125">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="29de0-125">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="29de0-126">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="29de0-126">integrityLevel</span></span>|<span data-ttu-id="29de0-127">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="29de0-127">processIntegrityLevel</span></span>|<span data-ttu-id="29de0-128">プロセスの整合性レベルです。</span><span class="sxs-lookup"><span data-stu-id="29de0-128">The integrity level of the process.</span></span> <span data-ttu-id="29de0-129">使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="29de0-129">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="29de0-130">isElevated</span><span class="sxs-lookup"><span data-stu-id="29de0-130">isElevated</span></span>|<span data-ttu-id="29de0-131">ブール型</span><span class="sxs-lookup"><span data-stu-id="29de0-131">Boolean</span></span>|<span data-ttu-id="29de0-132">プロセスが昇格した場合は true。</span><span class="sxs-lookup"><span data-stu-id="29de0-132">True if the process is elevated.</span></span>|
|<span data-ttu-id="29de0-133">名前</span><span class="sxs-lookup"><span data-stu-id="29de0-133">name</span></span>|<span data-ttu-id="29de0-134">String</span><span class="sxs-lookup"><span data-stu-id="29de0-134">String</span></span>|<span data-ttu-id="29de0-135">プロセスのイメージ ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="29de0-135">The name of the process' Image file.</span></span>|
|<span data-ttu-id="29de0-136">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="29de0-136">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="29de0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29de0-137">DateTimeOffset</span></span>|<span data-ttu-id="29de0-138">親プロセスの開始日時。</span><span class="sxs-lookup"><span data-stu-id="29de0-138">DateTime at which the parent process was started.</span></span> <span data-ttu-id="29de0-139">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="29de0-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29de0-140">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="29de0-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="29de0-141">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="29de0-141">parentProcessId</span></span>|<span data-ttu-id="29de0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="29de0-142">Int32</span></span>|<span data-ttu-id="29de0-143">プロセス ID (PID) の親プロセスです。</span><span class="sxs-lookup"><span data-stu-id="29de0-143">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="29de0-144">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="29de0-144">parentProcessName</span></span>|<span data-ttu-id="29de0-145">String</span><span class="sxs-lookup"><span data-stu-id="29de0-145">String</span></span>|<span data-ttu-id="29de0-146">親プロセスのイメージ ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="29de0-146">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="29de0-147">path</span><span class="sxs-lookup"><span data-stu-id="29de0-147">path</span></span>|<span data-ttu-id="29de0-148">String</span><span class="sxs-lookup"><span data-stu-id="29de0-148">String</span></span>|<span data-ttu-id="29de0-149">ファイル名を含む完全パスです。</span><span class="sxs-lookup"><span data-stu-id="29de0-149">Full path, including filename.</span></span>|
|<span data-ttu-id="29de0-150">プロセス Id</span><span class="sxs-lookup"><span data-stu-id="29de0-150">processId</span></span>|<span data-ttu-id="29de0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="29de0-151">Int32</span></span>|<span data-ttu-id="29de0-152">プロセス ID (PID) のプロセスです。</span><span class="sxs-lookup"><span data-stu-id="29de0-152">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29de0-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29de0-153">JSON representation</span></span>

<span data-ttu-id="29de0-154">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29de0-154">The following is a JSON representation of the resource.</span></span>

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
