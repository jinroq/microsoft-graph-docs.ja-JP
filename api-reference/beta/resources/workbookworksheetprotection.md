---
title: workbookWorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e4a2f3130c71df35b1106d1a342004cfc6fdf25
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348862"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="2c8c1-103">workbookWorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c8c1-103">workbookWorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c8c1-104">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="2c8c1-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c8c1-105">Methods</span></span>

| <span data-ttu-id="2c8c1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c8c1-106">Method</span></span>           | <span data-ttu-id="2c8c1-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2c8c1-107">Return Type</span></span>    |<span data-ttu-id="2c8c1-108">説明</span><span class="sxs-lookup"><span data-stu-id="2c8c1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c8c1-109">workbookWorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="2c8c1-109">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="2c8c1-110">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="2c8c1-110">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="2c8c1-111">workbookWorksheetProtection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-111">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="2c8c1-112">Protect</span><span class="sxs-lookup"><span data-stu-id="2c8c1-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="2c8c1-113">なし</span><span class="sxs-lookup"><span data-stu-id="2c8c1-113">None</span></span>|<span data-ttu-id="2c8c1-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="2c8c1-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="2c8c1-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="2c8c1-117">なし</span><span class="sxs-lookup"><span data-stu-id="2c8c1-117">None</span></span>|<span data-ttu-id="2c8c1-118">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="2c8c1-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c8c1-119">Properties</span></span>
| <span data-ttu-id="2c8c1-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c8c1-120">Property</span></span>     | <span data-ttu-id="2c8c1-121">型</span><span class="sxs-lookup"><span data-stu-id="2c8c1-121">Type</span></span>   |<span data-ttu-id="2c8c1-122">説明</span><span class="sxs-lookup"><span data-stu-id="2c8c1-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c8c1-123">オプション</span><span class="sxs-lookup"><span data-stu-id="2c8c1-123">options</span></span>|[<span data-ttu-id="2c8c1-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="2c8c1-124">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="2c8c1-125">シートの保護のオプション。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-125">Sheet protection options.</span></span> <span data-ttu-id="2c8c1-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-126">Read-only.</span></span>|
|<span data-ttu-id="2c8c1-127">protected</span><span class="sxs-lookup"><span data-stu-id="2c8c1-127">protected</span></span>|<span data-ttu-id="2c8c1-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="2c8c1-128">boolean</span></span>|<span data-ttu-id="2c8c1-p103">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c8c1-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c8c1-131">Relationships</span></span>
<span data-ttu-id="2c8c1-132">なし。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c8c1-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c8c1-133">JSON representation</span></span>

<span data-ttu-id="2c8c1-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c8c1-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "options"
  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": "boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
