---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c92c02b9c5e2409ad3036bbc34c41588161ae79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345401"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="5151a-103">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5151a-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="5151a-104">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="5151a-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="5151a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5151a-105">Methods</span></span>

| <span data-ttu-id="5151a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5151a-106">Method</span></span>           | <span data-ttu-id="5151a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5151a-107">Return Type</span></span>    |<span data-ttu-id="5151a-108">説明</span><span class="sxs-lookup"><span data-stu-id="5151a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5151a-109">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="5151a-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="5151a-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5151a-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="5151a-111">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5151a-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="5151a-112">Protect</span><span class="sxs-lookup"><span data-stu-id="5151a-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="5151a-113">なし</span><span class="sxs-lookup"><span data-stu-id="5151a-113">None</span></span>|<span data-ttu-id="5151a-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="5151a-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="5151a-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="5151a-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="5151a-117">なし</span><span class="sxs-lookup"><span data-stu-id="5151a-117">None</span></span>|<span data-ttu-id="5151a-118">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="5151a-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="5151a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5151a-119">Properties</span></span>
| <span data-ttu-id="5151a-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5151a-120">Property</span></span>     | <span data-ttu-id="5151a-121">型</span><span class="sxs-lookup"><span data-stu-id="5151a-121">Type</span></span>   |<span data-ttu-id="5151a-122">説明</span><span class="sxs-lookup"><span data-stu-id="5151a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5151a-123">オプション</span><span class="sxs-lookup"><span data-stu-id="5151a-123">options</span></span>|[<span data-ttu-id="5151a-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="5151a-124">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="5151a-125">シートの保護のオプション。</span><span class="sxs-lookup"><span data-stu-id="5151a-125">Sheet protection options.</span></span> <span data-ttu-id="5151a-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5151a-126">Read-only.</span></span>|
|<span data-ttu-id="5151a-127">protected</span><span class="sxs-lookup"><span data-stu-id="5151a-127">protected</span></span>|<span data-ttu-id="5151a-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="5151a-128">boolean</span></span>|<span data-ttu-id="5151a-p103">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5151a-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5151a-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5151a-131">JSON representation</span></span>

<span data-ttu-id="5151a-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5151a-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
