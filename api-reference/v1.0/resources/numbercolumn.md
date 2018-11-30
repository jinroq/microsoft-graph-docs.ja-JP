---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 8aa366e3c4f59fc5d22f945c863bab4f91373b67
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="eff42-102">NumberColumn リソース型</span><span class="sxs-lookup"><span data-stu-id="eff42-102">NumberColumn resource type</span></span>

<span data-ttu-id="eff42-103">[columnDefinition](columnDefinition.md) リソースの **numberColumn** は、列の値が数値であることを示します。</span><span class="sxs-lookup"><span data-stu-id="eff42-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eff42-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eff42-104">JSON representation</span></span>

<span data-ttu-id="eff42-105">以下は、**numberColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eff42-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="eff42-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eff42-106">Properties</span></span>

| <span data-ttu-id="eff42-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="eff42-107">Property name</span></span>      | <span data-ttu-id="eff42-108">種類</span><span class="sxs-lookup"><span data-stu-id="eff42-108">Type</span></span>   | <span data-ttu-id="eff42-109">説明</span><span class="sxs-lookup"><span data-stu-id="eff42-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="eff42-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="eff42-110">**DecimalPlaces**</span></span>  | <span data-ttu-id="eff42-111">string</span><span class="sxs-lookup"><span data-stu-id="eff42-111">string</span></span> | <span data-ttu-id="eff42-112">表示する小数点以下の桁数です。</span><span class="sxs-lookup"><span data-stu-id="eff42-112">How many decimal places to display.</span></span> <span data-ttu-id="eff42-113">使用可能な値については、下記を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eff42-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="eff42-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="eff42-114">**displayAs**</span></span>      | <span data-ttu-id="eff42-115">string</span><span class="sxs-lookup"><span data-stu-id="eff42-115">string</span></span> | <span data-ttu-id="eff42-116">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="eff42-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="eff42-117">`number` または `percentage` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="eff42-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="eff42-118">指定しない場合、`number` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="eff42-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="eff42-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="eff42-119">**maximum**</span></span>        | <span data-ttu-id="eff42-120">double</span><span class="sxs-lookup"><span data-stu-id="eff42-120">double</span></span> | <span data-ttu-id="eff42-121">許容最大値です。</span><span class="sxs-lookup"><span data-stu-id="eff42-121">The maximum permitted value.</span></span>
| <span data-ttu-id="eff42-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="eff42-122">**minimum**</span></span>        | <span data-ttu-id="eff42-123">double</span><span class="sxs-lookup"><span data-stu-id="eff42-123">double</span></span> | <span data-ttu-id="eff42-124">許容最小値です。</span><span class="sxs-lookup"><span data-stu-id="eff42-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="eff42-125">DecimalPlaces 値</span><span class="sxs-lookup"><span data-stu-id="eff42-125">DecimalPlaces values</span></span>

| <span data-ttu-id="eff42-126">値</span><span class="sxs-lookup"><span data-stu-id="eff42-126">Value</span></span>          | <span data-ttu-id="eff42-127">説明</span><span class="sxs-lookup"><span data-stu-id="eff42-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="eff42-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="eff42-128">**Automatic**</span></span>  | <span data-ttu-id="eff42-129">既定値。</span><span class="sxs-lookup"><span data-stu-id="eff42-129">Default.</span></span> <span data-ttu-id="eff42-130">必要に応じて自動的に小数点以下の桁を表示します。</span><span class="sxs-lookup"><span data-stu-id="eff42-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="eff42-131">**none**</span><span class="sxs-lookup"><span data-stu-id="eff42-131">**None**</span></span>       | <span data-ttu-id="eff42-132">小数点以下の桁は表示されません。</span><span class="sxs-lookup"><span data-stu-id="eff42-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="eff42-133">**one**</span><span class="sxs-lookup"><span data-stu-id="eff42-133">**One**</span></span>        | <span data-ttu-id="eff42-134">小数第 1 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="eff42-134">Always display one decimal place.</span></span>
| <span data-ttu-id="eff42-135">**two**</span><span class="sxs-lookup"><span data-stu-id="eff42-135">**Two**</span></span>        | <span data-ttu-id="eff42-136">小数第 2 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="eff42-136">Always display two decimal places.</span></span>
| <span data-ttu-id="eff42-137">**three**</span><span class="sxs-lookup"><span data-stu-id="eff42-137">**Three**</span></span>      | <span data-ttu-id="eff42-138">小数第 3 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="eff42-138">Always display three decimal places.</span></span>
| <span data-ttu-id="eff42-139">**four**</span><span class="sxs-lookup"><span data-stu-id="eff42-139">**Four**</span></span>       | <span data-ttu-id="eff42-140">小数第 4 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="eff42-140">Always display four decimal places.</span></span>
| <span data-ttu-id="eff42-141">**five**</span><span class="sxs-lookup"><span data-stu-id="eff42-141">**five**</span></span>       | <span data-ttu-id="eff42-142">小数第 5 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="eff42-142">Always display five decimal places.</span></span>

<span data-ttu-id="eff42-143">注: **decimalPlaces** と **displayAs** は数値の格納方法ではなく、表示方法に適用されます。</span><span class="sxs-lookup"><span data-stu-id="eff42-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="eff42-144">これらのプロパティは更新される場合があります。</span><span class="sxs-lookup"><span data-stu-id="eff42-144">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
