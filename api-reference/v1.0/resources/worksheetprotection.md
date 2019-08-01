---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9d3cbf4c03ff1e9938c7464d1501f261634ef347
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033307"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="843d4-103">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="843d4-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="843d4-104">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="843d4-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="843d4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="843d4-105">Methods</span></span>

| <span data-ttu-id="843d4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="843d4-106">Method</span></span>           | <span data-ttu-id="843d4-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="843d4-107">Return Type</span></span>    |<span data-ttu-id="843d4-108">説明</span><span class="sxs-lookup"><span data-stu-id="843d4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="843d4-109">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="843d4-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="843d4-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="843d4-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="843d4-111">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="843d4-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="843d4-112">Protect</span><span class="sxs-lookup"><span data-stu-id="843d4-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="843d4-113">None</span><span class="sxs-lookup"><span data-stu-id="843d4-113">None</span></span>|<span data-ttu-id="843d4-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="843d4-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="843d4-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="843d4-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="843d4-117">なし</span><span class="sxs-lookup"><span data-stu-id="843d4-117">None</span></span>|<span data-ttu-id="843d4-118">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="843d4-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="843d4-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="843d4-119">Properties</span></span>
| <span data-ttu-id="843d4-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="843d4-120">Property</span></span>     | <span data-ttu-id="843d4-121">型</span><span class="sxs-lookup"><span data-stu-id="843d4-121">Type</span></span>   |<span data-ttu-id="843d4-122">説明</span><span class="sxs-lookup"><span data-stu-id="843d4-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="843d4-123">オプション</span><span class="sxs-lookup"><span data-stu-id="843d4-123">options</span></span>|[<span data-ttu-id="843d4-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="843d4-124">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="843d4-125">シートの保護のオプション。</span><span class="sxs-lookup"><span data-stu-id="843d4-125">Sheet protection options.</span></span> <span data-ttu-id="843d4-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="843d4-126">Read-only.</span></span>|
|<span data-ttu-id="843d4-127">protected</span><span class="sxs-lookup"><span data-stu-id="843d4-127">protected</span></span>|<span data-ttu-id="843d4-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="843d4-128">boolean</span></span>|<span data-ttu-id="843d4-p103">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="843d4-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="843d4-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="843d4-131">JSON representation</span></span>

<span data-ttu-id="843d4-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="843d4-132">Here is a JSON representation of the resource.</span></span>

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
