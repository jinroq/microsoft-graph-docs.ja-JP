---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: f70a1d71729be68fc4d5dcb3de2599ff131bb8a9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342094"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="749af-102">numberColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="749af-102">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="749af-103">[columnDefinition](columndefinition.md) リソースの **numberColumn** は、列の値が数値であることを示します。</span><span class="sxs-lookup"><span data-stu-id="749af-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="749af-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="749af-104">JSON representation</span></span>

<span data-ttu-id="749af-105">以下は、**numberColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="749af-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="749af-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="749af-106">Properties</span></span>

| <span data-ttu-id="749af-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="749af-107">Property name</span></span>      | <span data-ttu-id="749af-108">種類</span><span class="sxs-lookup"><span data-stu-id="749af-108">Type</span></span>   | <span data-ttu-id="749af-109">説明</span><span class="sxs-lookup"><span data-stu-id="749af-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="749af-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="749af-110">**decimalPlaces**</span></span>  | <span data-ttu-id="749af-111">string</span><span class="sxs-lookup"><span data-stu-id="749af-111">string</span></span> | <span data-ttu-id="749af-112">表示する小数点以下の桁数です。</span><span class="sxs-lookup"><span data-stu-id="749af-112">How many decimal places to display.</span></span> <span data-ttu-id="749af-113">使用可能な値については、下記を参照してください。</span><span class="sxs-lookup"><span data-stu-id="749af-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="749af-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="749af-114">**displayAs**</span></span>      | <span data-ttu-id="749af-115">string</span><span class="sxs-lookup"><span data-stu-id="749af-115">string</span></span> | <span data-ttu-id="749af-116">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="749af-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="749af-117">`number` または `percentage` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="749af-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="749af-118">指定しない場合、`number` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="749af-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="749af-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="749af-119">**maximum**</span></span>        | <span data-ttu-id="749af-120">double</span><span class="sxs-lookup"><span data-stu-id="749af-120">double</span></span> | <span data-ttu-id="749af-121">許容最大値です。</span><span class="sxs-lookup"><span data-stu-id="749af-121">The maximum permitted value.</span></span>
| <span data-ttu-id="749af-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="749af-122">**minimum**</span></span>        | <span data-ttu-id="749af-123">double</span><span class="sxs-lookup"><span data-stu-id="749af-123">double</span></span> | <span data-ttu-id="749af-124">許容最小値です。</span><span class="sxs-lookup"><span data-stu-id="749af-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="749af-125">DecimalPlaces values</span><span class="sxs-lookup"><span data-stu-id="749af-125">DecimalPlaces values</span></span>

| <span data-ttu-id="749af-126">値</span><span class="sxs-lookup"><span data-stu-id="749af-126">Value</span></span>          | <span data-ttu-id="749af-127">説明</span><span class="sxs-lookup"><span data-stu-id="749af-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="749af-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="749af-128">**automatic**</span></span>  | <span data-ttu-id="749af-129">既定。</span><span class="sxs-lookup"><span data-stu-id="749af-129">Default.</span></span> <span data-ttu-id="749af-130">必要に応じて自動的に小数点以下の桁を表示します。</span><span class="sxs-lookup"><span data-stu-id="749af-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="749af-131">**none**</span><span class="sxs-lookup"><span data-stu-id="749af-131">**none**</span></span>       | <span data-ttu-id="749af-132">小数点以下の桁は表示されません。</span><span class="sxs-lookup"><span data-stu-id="749af-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="749af-133">**one**</span><span class="sxs-lookup"><span data-stu-id="749af-133">**one**</span></span>        | <span data-ttu-id="749af-134">小数第 1 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="749af-134">Always display one decimal place.</span></span>
| <span data-ttu-id="749af-135">**two**</span><span class="sxs-lookup"><span data-stu-id="749af-135">**two**</span></span>        | <span data-ttu-id="749af-136">小数第 2 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="749af-136">Always display two decimal places.</span></span>
| <span data-ttu-id="749af-137">**three**</span><span class="sxs-lookup"><span data-stu-id="749af-137">**three**</span></span>      | <span data-ttu-id="749af-138">小数第 3 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="749af-138">Always display three decimal places.</span></span>
| <span data-ttu-id="749af-139">**four**</span><span class="sxs-lookup"><span data-stu-id="749af-139">**four**</span></span>       | <span data-ttu-id="749af-140">小数第 4 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="749af-140">Always display four decimal places.</span></span>
| <span data-ttu-id="749af-141">**five**</span><span class="sxs-lookup"><span data-stu-id="749af-141">**five**</span></span>       | <span data-ttu-id="749af-142">小数第 5 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="749af-142">Always display five decimal places.</span></span>

<span data-ttu-id="749af-143">注: **decimalPlaces** と **displayAs** は数値の格納方法ではなく、表示方法に適用されます。</span><span class="sxs-lookup"><span data-stu-id="749af-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="749af-144">これらのプロパティは更新される場合があります。</span><span class="sxs-lookup"><span data-stu-id="749af-144">These properties may be updated.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": []
}
-->
