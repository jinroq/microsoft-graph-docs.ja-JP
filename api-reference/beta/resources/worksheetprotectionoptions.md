---
title: WorksheetProtectionOptions リソースの種類
description: シート保護のオプションを表します。
author: lumine2008
ms.openlocfilehash: 772c8b5eca7e9754a6bbc00e43cac102680974a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348574"
---
# <a name="worksheetprotectionoptions-resource-type"></a><span data-ttu-id="71a73-103">WorksheetProtectionOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71a73-103">WorksheetProtectionOptions resource type</span></span>

> <span data-ttu-id="71a73-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="71a73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71a73-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71a73-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71a73-106">シート保護のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-106">Represents the options in sheet protection.</span></span>

## <a name="properties"></a><span data-ttu-id="71a73-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71a73-107">Properties</span></span>
| <span data-ttu-id="71a73-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71a73-108">Property</span></span>     | <span data-ttu-id="71a73-109">種類</span><span class="sxs-lookup"><span data-stu-id="71a73-109">Type</span></span>   |<span data-ttu-id="71a73-110">説明</span><span class="sxs-lookup"><span data-stu-id="71a73-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71a73-111">allowAutoFilter</span><span class="sxs-lookup"><span data-stu-id="71a73-111">allowAutoFilter</span></span>|<span data-ttu-id="71a73-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-112">boolean</span></span>|<span data-ttu-id="71a73-113">自動フィルター機能の使用を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-113">Represents the worksheet protection option of allowing using auto filter feature.</span></span>|
|<span data-ttu-id="71a73-114">allowDeleteColumns</span><span class="sxs-lookup"><span data-stu-id="71a73-114">allowDeleteColumns</span></span>|<span data-ttu-id="71a73-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-115">boolean</span></span>|<span data-ttu-id="71a73-116">列の削除を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-116">Represents the worksheet protection option of allowing deleting columns.</span></span>|
|<span data-ttu-id="71a73-117">allowDeleteRows</span><span class="sxs-lookup"><span data-stu-id="71a73-117">allowDeleteRows</span></span>|<span data-ttu-id="71a73-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-118">boolean</span></span>|<span data-ttu-id="71a73-119">行の削除を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-119">Represents the worksheet protection option of allowing deleting rows.</span></span>|
|<span data-ttu-id="71a73-120">allowFormatCells</span><span class="sxs-lookup"><span data-stu-id="71a73-120">allowFormatCells</span></span>|<span data-ttu-id="71a73-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-121">boolean</span></span>|<span data-ttu-id="71a73-122">セルの書式設定を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-122">Represents the worksheet protection option of allowing formatting cells.</span></span>|
|<span data-ttu-id="71a73-123">allowFormatColumns</span><span class="sxs-lookup"><span data-stu-id="71a73-123">allowFormatColumns</span></span>|<span data-ttu-id="71a73-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-124">boolean</span></span>|<span data-ttu-id="71a73-125">列の書式設定を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-125">Represents the worksheet protection option of allowing formatting columns.</span></span>|
|<span data-ttu-id="71a73-126">allowFormatRows</span><span class="sxs-lookup"><span data-stu-id="71a73-126">allowFormatRows</span></span>|<span data-ttu-id="71a73-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-127">boolean</span></span>|<span data-ttu-id="71a73-128">行の書式設定を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-128">Represents the worksheet protection option of allowing formatting rows.</span></span>|
|<span data-ttu-id="71a73-129">allowInsertColumns</span><span class="sxs-lookup"><span data-stu-id="71a73-129">allowInsertColumns</span></span>|<span data-ttu-id="71a73-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-130">boolean</span></span>|<span data-ttu-id="71a73-131">列の挿入を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-131">Represents the worksheet protection option of allowing inserting columns.</span></span>|
|<span data-ttu-id="71a73-132">allowInsertHyperlinks</span><span class="sxs-lookup"><span data-stu-id="71a73-132">allowInsertHyperlinks</span></span>|<span data-ttu-id="71a73-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-133">boolean</span></span>|<span data-ttu-id="71a73-134">ハイパーリンクの挿入を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-134">Represents the worksheet protection option of allowing inserting hyperlinks.</span></span>|
|<span data-ttu-id="71a73-135">allowInsertRows</span><span class="sxs-lookup"><span data-stu-id="71a73-135">allowInsertRows</span></span>|<span data-ttu-id="71a73-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-136">boolean</span></span>|<span data-ttu-id="71a73-137">行の挿入を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-137">Represents the worksheet protection option of allowing inserting rows.</span></span>|
|<span data-ttu-id="71a73-138">allowPivotTables</span><span class="sxs-lookup"><span data-stu-id="71a73-138">allowPivotTables</span></span>|<span data-ttu-id="71a73-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-139">boolean</span></span>|<span data-ttu-id="71a73-140">ピボット テーブル機能の使用を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-140">Represents the worksheet protection option of allowing using pivot table feature.</span></span>|
|<span data-ttu-id="71a73-141">allowSort</span><span class="sxs-lookup"><span data-stu-id="71a73-141">allowSort</span></span>|<span data-ttu-id="71a73-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="71a73-142">boolean</span></span>|<span data-ttu-id="71a73-143">並ベ替え機能の使用を可能にするワークシート保護オプションを表します。</span><span class="sxs-lookup"><span data-stu-id="71a73-143">Represents the worksheet protection option of allowing using sort feature.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71a73-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71a73-144">JSON representation</span></span>

<span data-ttu-id="71a73-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71a73-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtectionOptions"
}-->

```json
{
  "allowAutoFilter": true,
  "allowDeleteColumns": true,
  "allowDeleteRows": true,
  "allowFormatCells": true,
  "allowFormatColumns": true,
  "allowFormatRows": true,
  "allowInsertColumns": true,
  "allowInsertHyperlinks": true,
  "allowInsertRows": true,
  "allowPivotTables": true,
  "allowSort": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->