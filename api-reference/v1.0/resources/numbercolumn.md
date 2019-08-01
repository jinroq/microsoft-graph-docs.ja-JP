---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: columnDefinition リソースの numberColumn は、列の値が数値であることを示します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9196e2508ed3109ee56c24ad72943ca50aed11bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035973"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="57b28-103">numberColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57b28-103">NumberColumn resource type</span></span>

<span data-ttu-id="57b28-104">[columnDefinition](columndefinition.md) リソースの **numberColumn** は、列の値が数値であることを示します。</span><span class="sxs-lookup"><span data-stu-id="57b28-104">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57b28-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57b28-105">JSON representation</span></span>

<span data-ttu-id="57b28-106">以下は、**numberColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="57b28-106">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="57b28-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57b28-107">Properties</span></span>

| <span data-ttu-id="57b28-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="57b28-108">Property name</span></span>      | <span data-ttu-id="57b28-109">種類</span><span class="sxs-lookup"><span data-stu-id="57b28-109">Type</span></span>   | <span data-ttu-id="57b28-110">説明</span><span class="sxs-lookup"><span data-stu-id="57b28-110">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="57b28-111">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="57b28-111">**decimalPlaces**</span></span>  | <span data-ttu-id="57b28-112">string</span><span class="sxs-lookup"><span data-stu-id="57b28-112">string</span></span> | <span data-ttu-id="57b28-113">表示する小数点以下の桁数です。</span><span class="sxs-lookup"><span data-stu-id="57b28-113">How many decimal places to display.</span></span> <span data-ttu-id="57b28-114">使用可能な値については、下記を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57b28-114">See below for information about the possible values.</span></span>
| <span data-ttu-id="57b28-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="57b28-115">**displayAs**</span></span>      | <span data-ttu-id="57b28-116">string</span><span class="sxs-lookup"><span data-stu-id="57b28-116">string</span></span> | <span data-ttu-id="57b28-117">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="57b28-117">How the value should be presented in the UX.</span></span> <span data-ttu-id="57b28-118">`number` または `percentage` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="57b28-118">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="57b28-119">指定しない場合、`number` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="57b28-119">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="57b28-120">**maximum**</span><span class="sxs-lookup"><span data-stu-id="57b28-120">**maximum**</span></span>        | <span data-ttu-id="57b28-121">double</span><span class="sxs-lookup"><span data-stu-id="57b28-121">double</span></span> | <span data-ttu-id="57b28-122">許容最大値です。</span><span class="sxs-lookup"><span data-stu-id="57b28-122">The maximum permitted value.</span></span>
| <span data-ttu-id="57b28-123">**minimum**</span><span class="sxs-lookup"><span data-stu-id="57b28-123">**minimum**</span></span>        | <span data-ttu-id="57b28-124">double</span><span class="sxs-lookup"><span data-stu-id="57b28-124">double</span></span> | <span data-ttu-id="57b28-125">許容最小値です。</span><span class="sxs-lookup"><span data-stu-id="57b28-125">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="57b28-126">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="57b28-126">DecimalPlaces</span></span>

| <span data-ttu-id="57b28-127">値</span><span class="sxs-lookup"><span data-stu-id="57b28-127">Value</span></span>          | <span data-ttu-id="57b28-128">説明</span><span class="sxs-lookup"><span data-stu-id="57b28-128">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="57b28-129">**automatic**</span><span class="sxs-lookup"><span data-stu-id="57b28-129">**automatic**</span></span>  | <span data-ttu-id="57b28-130">既定。</span><span class="sxs-lookup"><span data-stu-id="57b28-130">Default.</span></span> <span data-ttu-id="57b28-131">必要に応じて自動的に小数点以下の桁を表示します。</span><span class="sxs-lookup"><span data-stu-id="57b28-131">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="57b28-132">**none**</span><span class="sxs-lookup"><span data-stu-id="57b28-132">**none**</span></span>       | <span data-ttu-id="57b28-133">小数点以下の桁は表示されません。</span><span class="sxs-lookup"><span data-stu-id="57b28-133">Do not display any decimal places.</span></span>
| <span data-ttu-id="57b28-134">**one**</span><span class="sxs-lookup"><span data-stu-id="57b28-134">**one**</span></span>        | <span data-ttu-id="57b28-135">小数第 1 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="57b28-135">Always display one decimal place.</span></span>
| <span data-ttu-id="57b28-136">**two**</span><span class="sxs-lookup"><span data-stu-id="57b28-136">**two**</span></span>        | <span data-ttu-id="57b28-137">小数第 2 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="57b28-137">Always display two decimal places.</span></span>
| <span data-ttu-id="57b28-138">**three**</span><span class="sxs-lookup"><span data-stu-id="57b28-138">**three**</span></span>      | <span data-ttu-id="57b28-139">小数第 3 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="57b28-139">Always display three decimal places.</span></span>
| <span data-ttu-id="57b28-140">**four**</span><span class="sxs-lookup"><span data-stu-id="57b28-140">**four**</span></span>       | <span data-ttu-id="57b28-141">小数第 4 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="57b28-141">Always display four decimal places.</span></span>
| <span data-ttu-id="57b28-142">**five**</span><span class="sxs-lookup"><span data-stu-id="57b28-142">**five**</span></span>       | <span data-ttu-id="57b28-143">小数第 5 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="57b28-143">Always display five decimal places.</span></span>

<span data-ttu-id="57b28-144">注: **decimalPlaces** と **displayAs** は数値の格納方法ではなく、表示方法に適用されます。</span><span class="sxs-lookup"><span data-stu-id="57b28-144">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="57b28-145">これらのプロパティは更新される場合があります。</span><span class="sxs-lookup"><span data-stu-id="57b28-145">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
