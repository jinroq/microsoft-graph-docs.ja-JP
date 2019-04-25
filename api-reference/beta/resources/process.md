---
title: プロセスリソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563341"
---
# <a name="process-resource-type"></a><span data-ttu-id="64a90-104">プロセスリソースの種類</span><span class="sxs-lookup"><span data-stu-id="64a90-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64a90-105">通知に関連するプロセスに関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="64a90-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="64a90-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64a90-106">Properties</span></span>

| <span data-ttu-id="64a90-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64a90-107">Property</span></span>   | <span data-ttu-id="64a90-108">型</span><span class="sxs-lookup"><span data-stu-id="64a90-108">Type</span></span>|<span data-ttu-id="64a90-109">説明</span><span class="sxs-lookup"><span data-stu-id="64a90-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64a90-110">accountName</span><span class="sxs-lookup"><span data-stu-id="64a90-110">accountName</span></span>|<span data-ttu-id="64a90-111">String</span><span class="sxs-lookup"><span data-stu-id="64a90-111">String</span></span>|<span data-ttu-id="64a90-112">ユーザーアカウント識別子 (アカウントの下で実行されたユーザーアカウントコンテキスト)。たとえば、AccountName、SID など。</span><span class="sxs-lookup"><span data-stu-id="64a90-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="64a90-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="64a90-113">commandLine</span></span>|<span data-ttu-id="64a90-114">String</span><span class="sxs-lookup"><span data-stu-id="64a90-114">String</span></span>|<span data-ttu-id="64a90-115">すべてのパラメーターを含む完全なプロセス呼び出しの commandline。</span><span class="sxs-lookup"><span data-stu-id="64a90-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="64a90-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64a90-116">createdDateTime</span></span>|<span data-ttu-id="64a90-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64a90-117">DateTimeOffset</span></span>|<span data-ttu-id="64a90-118">プロセスが開始された時刻。</span><span class="sxs-lookup"><span data-stu-id="64a90-118">Time at which the process was started.</span></span> <span data-ttu-id="64a90-119">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="64a90-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64a90-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="64a90-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="64a90-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="64a90-121">fileHash</span></span>|[<span data-ttu-id="64a90-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="64a90-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="64a90-123">ファイルハッシュを含む複合型 (暗号化と場所に依存)。</span><span class="sxs-lookup"><span data-stu-id="64a90-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="64a90-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="64a90-124">integrityLevel</span></span>|<span data-ttu-id="64a90-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="64a90-125">processIntegrityLevel</span></span>|<span data-ttu-id="64a90-126">プロセスの整合性レベル。</span><span class="sxs-lookup"><span data-stu-id="64a90-126">The integrity level of the process.</span></span> <span data-ttu-id="64a90-127">使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。</span><span class="sxs-lookup"><span data-stu-id="64a90-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="64a90-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="64a90-128">isElevated</span></span>|<span data-ttu-id="64a90-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="64a90-129">Boolean</span></span>|<span data-ttu-id="64a90-130">プロセスが昇格された場合は True。</span><span class="sxs-lookup"><span data-stu-id="64a90-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="64a90-131">name</span><span class="sxs-lookup"><span data-stu-id="64a90-131">name</span></span>|<span data-ttu-id="64a90-132">String</span><span class="sxs-lookup"><span data-stu-id="64a90-132">String</span></span>|<span data-ttu-id="64a90-133">プロセスのイメージファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="64a90-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="64a90-134">parentprocess/datetime</span><span class="sxs-lookup"><span data-stu-id="64a90-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="64a90-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64a90-135">DateTimeOffset</span></span>|<span data-ttu-id="64a90-136">親プロセスが開始された DateTime。</span><span class="sxs-lookup"><span data-stu-id="64a90-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="64a90-137">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="64a90-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64a90-138">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="64a90-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="64a90-139">parentprocessid</span><span class="sxs-lookup"><span data-stu-id="64a90-139">parentProcessId</span></span>|<span data-ttu-id="64a90-140">Int32</span><span class="sxs-lookup"><span data-stu-id="64a90-140">Int32</span></span>|<span data-ttu-id="64a90-141">親プロセスのプロセス ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="64a90-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="64a90-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="64a90-142">parentProcessName</span></span>|<span data-ttu-id="64a90-143">String</span><span class="sxs-lookup"><span data-stu-id="64a90-143">String</span></span>|<span data-ttu-id="64a90-144">親プロセスのイメージファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="64a90-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="64a90-145">path</span><span class="sxs-lookup"><span data-stu-id="64a90-145">path</span></span>|<span data-ttu-id="64a90-146">String</span><span class="sxs-lookup"><span data-stu-id="64a90-146">String</span></span>|<span data-ttu-id="64a90-147">ファイル名を含む完全なパス。</span><span class="sxs-lookup"><span data-stu-id="64a90-147">Full path, including filename.</span></span>|
|<span data-ttu-id="64a90-148">processId</span><span class="sxs-lookup"><span data-stu-id="64a90-148">processId</span></span>|<span data-ttu-id="64a90-149">Int32</span><span class="sxs-lookup"><span data-stu-id="64a90-149">Int32</span></span>|<span data-ttu-id="64a90-150">プロセスのプロセス ID (PID)。</span><span class="sxs-lookup"><span data-stu-id="64a90-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64a90-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64a90-151">JSON representation</span></span>

<span data-ttu-id="64a90-152">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64a90-152">The following is a JSON representation of the resource.</span></span>

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
