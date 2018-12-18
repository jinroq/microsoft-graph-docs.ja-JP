---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
ms.openlocfilehash: 3df3ea522b7d4f476bf09173ed7998e62e9562d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344290"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="c9d60-103">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9d60-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="c9d60-104">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="c9d60-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="c9d60-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9d60-105">Methods</span></span>

| <span data-ttu-id="c9d60-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9d60-106">Method</span></span>           | <span data-ttu-id="c9d60-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c9d60-107">Return Type</span></span>    |<span data-ttu-id="c9d60-108">説明</span><span class="sxs-lookup"><span data-stu-id="c9d60-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9d60-109">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="c9d60-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="c9d60-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="c9d60-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="c9d60-111">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c9d60-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="c9d60-112">Protect</span><span class="sxs-lookup"><span data-stu-id="c9d60-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="c9d60-113">なし</span><span class="sxs-lookup"><span data-stu-id="c9d60-113">None</span></span>|<span data-ttu-id="c9d60-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="c9d60-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="c9d60-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="c9d60-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="c9d60-117">なし</span><span class="sxs-lookup"><span data-stu-id="c9d60-117">None</span></span>|<span data-ttu-id="c9d60-118">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="c9d60-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="c9d60-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9d60-119">Properties</span></span>
| <span data-ttu-id="c9d60-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9d60-120">Property</span></span>     | <span data-ttu-id="c9d60-121">種類</span><span class="sxs-lookup"><span data-stu-id="c9d60-121">Type</span></span>   |<span data-ttu-id="c9d60-122">説明</span><span class="sxs-lookup"><span data-stu-id="c9d60-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9d60-123">options</span><span class="sxs-lookup"><span data-stu-id="c9d60-123">options</span></span>|[<span data-ttu-id="c9d60-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="c9d60-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="c9d60-p102">シートの保護のオプション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c9d60-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="c9d60-127">protected</span><span class="sxs-lookup"><span data-stu-id="c9d60-127">protected</span></span>|<span data-ttu-id="c9d60-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="c9d60-128">boolean</span></span>|<span data-ttu-id="c9d60-p103">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c9d60-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9d60-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9d60-131">JSON representation</span></span>

<span data-ttu-id="c9d60-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9d60-132">Here is a JSON representation of the resource.</span></span>

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