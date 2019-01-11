---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f0bbf3652223a532cd3d815aca832d4cfcd37171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860714"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="b35d1-103">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b35d1-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="b35d1-104">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="b35d1-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="b35d1-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b35d1-105">Methods</span></span>

| <span data-ttu-id="b35d1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b35d1-106">Method</span></span>           | <span data-ttu-id="b35d1-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b35d1-107">Return Type</span></span>    |<span data-ttu-id="b35d1-108">説明</span><span class="sxs-lookup"><span data-stu-id="b35d1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b35d1-109">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="b35d1-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="b35d1-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="b35d1-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="b35d1-111">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b35d1-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="b35d1-112">Protect</span><span class="sxs-lookup"><span data-stu-id="b35d1-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="b35d1-113">なし</span><span class="sxs-lookup"><span data-stu-id="b35d1-113">None</span></span>|<span data-ttu-id="b35d1-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="b35d1-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="b35d1-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="b35d1-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="b35d1-117">なし</span><span class="sxs-lookup"><span data-stu-id="b35d1-117">None</span></span>|<span data-ttu-id="b35d1-118">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="b35d1-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="b35d1-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b35d1-119">Properties</span></span>
| <span data-ttu-id="b35d1-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b35d1-120">Property</span></span>     | <span data-ttu-id="b35d1-121">種類</span><span class="sxs-lookup"><span data-stu-id="b35d1-121">Type</span></span>   |<span data-ttu-id="b35d1-122">説明</span><span class="sxs-lookup"><span data-stu-id="b35d1-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b35d1-123">options</span><span class="sxs-lookup"><span data-stu-id="b35d1-123">options</span></span>|[<span data-ttu-id="b35d1-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="b35d1-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="b35d1-p102">シートの保護のオプション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b35d1-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="b35d1-127">protected</span><span class="sxs-lookup"><span data-stu-id="b35d1-127">protected</span></span>|<span data-ttu-id="b35d1-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="b35d1-128">boolean</span></span>|<span data-ttu-id="b35d1-p103">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b35d1-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b35d1-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b35d1-131">JSON representation</span></span>

<span data-ttu-id="b35d1-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b35d1-132">Here is a JSON representation of the resource.</span></span>

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
