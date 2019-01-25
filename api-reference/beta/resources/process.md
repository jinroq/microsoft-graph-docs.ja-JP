---
title: プロセス リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521209"
---
# <a name="process-resource-type"></a><span data-ttu-id="2bb4a-104">プロセス リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2bb4a-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bb4a-105">ステートフルなアラートに関連するプロセスについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="2bb4a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2bb4a-106">Properties</span></span>

| <span data-ttu-id="2bb4a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2bb4a-107">Property</span></span>   | <span data-ttu-id="2bb4a-108">型</span><span class="sxs-lookup"><span data-stu-id="2bb4a-108">Type</span></span>|<span data-ttu-id="2bb4a-109">説明</span><span class="sxs-lookup"><span data-stu-id="2bb4a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bb4a-110">accountName</span><span class="sxs-lookup"><span data-stu-id="2bb4a-110">accountName</span></span>|<span data-ttu-id="2bb4a-111">String</span><span class="sxs-lookup"><span data-stu-id="2bb4a-111">String</span></span>|<span data-ttu-id="2bb4a-112">ユーザーは、例、アカウント名、SID、およびように識別子 (ユーザー アカウントのコンテキストでプロセスが実行された) を考慮します。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="2bb4a-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="2bb4a-113">commandLine</span></span>|<span data-ttu-id="2bb4a-114">String</span><span class="sxs-lookup"><span data-stu-id="2bb4a-114">String</span></span>|<span data-ttu-id="2bb4a-115">完全な処理の呼び出しは、すべてのパラメーターを含むを使用できます。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="2bb4a-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bb4a-116">createdDateTime</span></span>|<span data-ttu-id="2bb4a-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bb4a-117">DateTimeOffset</span></span>|<span data-ttu-id="2bb4a-118">プロセスが開始された時刻です。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-118">Time at which the process was started.</span></span> <span data-ttu-id="2bb4a-119">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2bb4a-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2bb4a-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="2bb4a-121">fileHash</span></span>|[<span data-ttu-id="2bb4a-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="2bb4a-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="2bb4a-123">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="2bb4a-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="2bb4a-124">integrityLevel</span></span>|<span data-ttu-id="2bb4a-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="2bb4a-125">processIntegrityLevel</span></span>|<span data-ttu-id="2bb4a-126">プロセスの整合性レベルです。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-126">The integrity level of the process.</span></span> <span data-ttu-id="2bb4a-127">使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="2bb4a-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="2bb4a-128">isElevated</span></span>|<span data-ttu-id="2bb4a-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="2bb4a-129">Boolean</span></span>|<span data-ttu-id="2bb4a-130">プロセスが昇格した場合は true。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="2bb4a-131">name</span><span class="sxs-lookup"><span data-stu-id="2bb4a-131">name</span></span>|<span data-ttu-id="2bb4a-132">String</span><span class="sxs-lookup"><span data-stu-id="2bb4a-132">String</span></span>|<span data-ttu-id="2bb4a-133">プロセスのイメージ ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="2bb4a-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bb4a-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="2bb4a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bb4a-135">DateTimeOffset</span></span>|<span data-ttu-id="2bb4a-136">親プロセスの開始日時。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="2bb4a-137">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2bb4a-138">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2bb4a-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="2bb4a-139">parentProcessId</span></span>|<span data-ttu-id="2bb4a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb4a-140">Int32</span></span>|<span data-ttu-id="2bb4a-141">プロセス ID (PID) の親プロセスです。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="2bb4a-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="2bb4a-142">parentProcessName</span></span>|<span data-ttu-id="2bb4a-143">String</span><span class="sxs-lookup"><span data-stu-id="2bb4a-143">String</span></span>|<span data-ttu-id="2bb4a-144">親プロセスのイメージ ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="2bb4a-145">path</span><span class="sxs-lookup"><span data-stu-id="2bb4a-145">path</span></span>|<span data-ttu-id="2bb4a-146">String</span><span class="sxs-lookup"><span data-stu-id="2bb4a-146">String</span></span>|<span data-ttu-id="2bb4a-147">ファイル名を含む完全パスです。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-147">Full path, including filename.</span></span>|
|<span data-ttu-id="2bb4a-148">ProcessID</span><span class="sxs-lookup"><span data-stu-id="2bb4a-148">processId</span></span>|<span data-ttu-id="2bb4a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb4a-149">Int32</span></span>|<span data-ttu-id="2bb4a-150">プロセス ID (PID) のプロセスです。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bb4a-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2bb4a-151">JSON representation</span></span>

<span data-ttu-id="2bb4a-152">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2bb4a-152">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/process.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
