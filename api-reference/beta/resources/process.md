---
title: プロセス リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 2e60c9e008ccfddaa0bcc3e78c27cc17c65a3844
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069710"
---
# <a name="process-resource-type"></a><span data-ttu-id="7ee85-104">プロセス リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7ee85-104">process resource type</span></span>

 > <span data-ttu-id="7ee85-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ee85-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ee85-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ee85-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ee85-107">ステートフルなアラートに関連するプロセスについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="7ee85-107">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="7ee85-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ee85-108">Properties</span></span>

| <span data-ttu-id="7ee85-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ee85-109">Property</span></span>   | <span data-ttu-id="7ee85-110">型</span><span class="sxs-lookup"><span data-stu-id="7ee85-110">Type</span></span>|<span data-ttu-id="7ee85-111">説明</span><span class="sxs-lookup"><span data-stu-id="7ee85-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ee85-112">accountName</span><span class="sxs-lookup"><span data-stu-id="7ee85-112">accountName</span></span>|<span data-ttu-id="7ee85-113">String</span><span class="sxs-lookup"><span data-stu-id="7ee85-113">String</span></span>|<span data-ttu-id="7ee85-114">ユーザーは、例、アカウント名、SID、およびように識別子 (ユーザー アカウントのコンテキストでプロセスが実行された) を考慮します。</span><span class="sxs-lookup"><span data-stu-id="7ee85-114">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="7ee85-115">commandLine</span><span class="sxs-lookup"><span data-stu-id="7ee85-115">commandLine</span></span>|<span data-ttu-id="7ee85-116">String</span><span class="sxs-lookup"><span data-stu-id="7ee85-116">String</span></span>|<span data-ttu-id="7ee85-117">完全な処理の呼び出しは、すべてのパラメーターを含むを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7ee85-117">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="7ee85-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ee85-118">createdDateTime</span></span>|<span data-ttu-id="7ee85-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ee85-119">DateTimeOffset</span></span>|<span data-ttu-id="7ee85-120">プロセスが開始された時刻です。</span><span class="sxs-lookup"><span data-stu-id="7ee85-120">Time at which the process was started.</span></span> <span data-ttu-id="7ee85-121">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7ee85-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7ee85-122">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7ee85-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7ee85-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="7ee85-123">fileHash</span></span>|[<span data-ttu-id="7ee85-124">fileHash</span><span class="sxs-lookup"><span data-stu-id="7ee85-124">fileHash</span></span>](filehash.md)|<span data-ttu-id="7ee85-125">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ee85-125">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="7ee85-126">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="7ee85-126">integrityLevel</span></span>|<span data-ttu-id="7ee85-127">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="7ee85-127">processIntegrityLevel</span></span>|<span data-ttu-id="7ee85-128">プロセスの整合性レベルです。</span><span class="sxs-lookup"><span data-stu-id="7ee85-128">The integrity level of the process.</span></span> <span data-ttu-id="7ee85-129">使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="7ee85-129">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="7ee85-130">isElevated</span><span class="sxs-lookup"><span data-stu-id="7ee85-130">isElevated</span></span>|<span data-ttu-id="7ee85-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="7ee85-131">Boolean</span></span>|<span data-ttu-id="7ee85-132">プロセスが昇格した場合は true。</span><span class="sxs-lookup"><span data-stu-id="7ee85-132">True if the process is elevated.</span></span>|
|<span data-ttu-id="7ee85-133">名前</span><span class="sxs-lookup"><span data-stu-id="7ee85-133">name</span></span>|<span data-ttu-id="7ee85-134">String</span><span class="sxs-lookup"><span data-stu-id="7ee85-134">String</span></span>|<span data-ttu-id="7ee85-135">プロセスのイメージ ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="7ee85-135">The name of the process' Image file.</span></span>|
|<span data-ttu-id="7ee85-136">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ee85-136">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="7ee85-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ee85-137">DateTimeOffset</span></span>|<span data-ttu-id="7ee85-138">親プロセスの開始日時。</span><span class="sxs-lookup"><span data-stu-id="7ee85-138">DateTime at which the parent process was started.</span></span> <span data-ttu-id="7ee85-139">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7ee85-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7ee85-140">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7ee85-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7ee85-141">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="7ee85-141">parentProcessId</span></span>|<span data-ttu-id="7ee85-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee85-142">Int32</span></span>|<span data-ttu-id="7ee85-143">プロセス ID (PID) の親プロセスです。</span><span class="sxs-lookup"><span data-stu-id="7ee85-143">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="7ee85-144">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="7ee85-144">parentProcessName</span></span>|<span data-ttu-id="7ee85-145">String</span><span class="sxs-lookup"><span data-stu-id="7ee85-145">String</span></span>|<span data-ttu-id="7ee85-146">親プロセスのイメージ ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="7ee85-146">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="7ee85-147">path</span><span class="sxs-lookup"><span data-stu-id="7ee85-147">path</span></span>|<span data-ttu-id="7ee85-148">String</span><span class="sxs-lookup"><span data-stu-id="7ee85-148">String</span></span>|<span data-ttu-id="7ee85-149">ファイル名を含む完全パスです。</span><span class="sxs-lookup"><span data-stu-id="7ee85-149">Full path, including filename.</span></span>|
|<span data-ttu-id="7ee85-150">プロセス Id</span><span class="sxs-lookup"><span data-stu-id="7ee85-150">processId</span></span>|<span data-ttu-id="7ee85-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee85-151">Int32</span></span>|<span data-ttu-id="7ee85-152">プロセス ID (PID) のプロセスです。</span><span class="sxs-lookup"><span data-stu-id="7ee85-152">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ee85-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ee85-153">JSON representation</span></span>

<span data-ttu-id="7ee85-154">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ee85-154">The following is a JSON representation of the resource.</span></span>

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