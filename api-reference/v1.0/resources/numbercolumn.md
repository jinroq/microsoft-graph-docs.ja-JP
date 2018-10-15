---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 4aaff6539fc9c7ce77029463562c0f8fca57cac6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266507"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="551cd-102">NumberColumn リソース型</span><span class="sxs-lookup"><span data-stu-id="551cd-102">NumberColumn resource type</span></span>

<span data-ttu-id="551cd-103">[columnDefinition](columnDefinition.md) リソースの **numberColumn** は、列の値が数値であることを示します。</span><span class="sxs-lookup"><span data-stu-id="551cd-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="551cd-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="551cd-104">JSON representation</span></span>

<span data-ttu-id="551cd-105">以下は、**numberColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="551cd-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="551cd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="551cd-106">Properties</span></span>

| <span data-ttu-id="551cd-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="551cd-107">Property name</span></span>      | <span data-ttu-id="551cd-108">型</span><span class="sxs-lookup"><span data-stu-id="551cd-108">Type</span></span>   | <span data-ttu-id="551cd-109">説明</span><span class="sxs-lookup"><span data-stu-id="551cd-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="551cd-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="551cd-110">**decimalPlaces**</span></span>  | <span data-ttu-id="551cd-111">string</span><span class="sxs-lookup"><span data-stu-id="551cd-111">string</span></span> | <span data-ttu-id="551cd-112">表示する小数点以下の桁数です。</span><span class="sxs-lookup"><span data-stu-id="551cd-112">How many decimal places to display.</span></span> <span data-ttu-id="551cd-113">使用可能な値については、下記を参照してください。</span><span class="sxs-lookup"><span data-stu-id="551cd-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="551cd-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="551cd-114">**displayAs**</span></span>      | <span data-ttu-id="551cd-115">string</span><span class="sxs-lookup"><span data-stu-id="551cd-115">string</span></span> | <span data-ttu-id="551cd-116">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="551cd-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="551cd-117">または `percentage` のいずれかでなければなりません。`number`</span><span class="sxs-lookup"><span data-stu-id="551cd-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="551cd-118">指定しない場合、`number` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="551cd-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="551cd-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="551cd-119">**maximum**</span></span>        | <span data-ttu-id="551cd-120">double</span><span class="sxs-lookup"><span data-stu-id="551cd-120">double</span></span> | <span data-ttu-id="551cd-121">許容最大値です。</span><span class="sxs-lookup"><span data-stu-id="551cd-121">The maximum permitted value.</span></span>
| <span data-ttu-id="551cd-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="551cd-122">**minimum**</span></span>        | <span data-ttu-id="551cd-123">double</span><span class="sxs-lookup"><span data-stu-id="551cd-123">double</span></span> | <span data-ttu-id="551cd-124">許容最小値です。</span><span class="sxs-lookup"><span data-stu-id="551cd-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="551cd-125">decimalPlaces</span><span class="sxs-lookup"><span data-stu-id="551cd-125">decimalPlaces</span></span>

| <span data-ttu-id="551cd-126">値</span><span class="sxs-lookup"><span data-stu-id="551cd-126">Value</span></span>          | <span data-ttu-id="551cd-127">説明</span><span class="sxs-lookup"><span data-stu-id="551cd-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="551cd-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="551cd-128">**automatic**</span></span>  | <span data-ttu-id="551cd-129">既定。</span><span class="sxs-lookup"><span data-stu-id="551cd-129">Default.</span></span> <span data-ttu-id="551cd-130">必要に応じて自動的に小数点以下の桁を表示します。</span><span class="sxs-lookup"><span data-stu-id="551cd-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="551cd-131">**なし**</span><span class="sxs-lookup"><span data-stu-id="551cd-131">**none**</span></span>       | <span data-ttu-id="551cd-132">小数点以下の桁は表示されません。</span><span class="sxs-lookup"><span data-stu-id="551cd-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="551cd-133">**one**</span><span class="sxs-lookup"><span data-stu-id="551cd-133">**one**</span></span>        | <span data-ttu-id="551cd-134">小数第 1 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="551cd-134">Always display one decimal place.</span></span>
| <span data-ttu-id="551cd-135">**two**</span><span class="sxs-lookup"><span data-stu-id="551cd-135">**two**</span></span>        | <span data-ttu-id="551cd-136">小数第 2 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="551cd-136">Always display two decimal places.</span></span>
| <span data-ttu-id="551cd-137">**three**</span><span class="sxs-lookup"><span data-stu-id="551cd-137">**three**</span></span>      | <span data-ttu-id="551cd-138">小数第 3 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="551cd-138">Always display three decimal places.</span></span>
| <span data-ttu-id="551cd-139">**four**</span><span class="sxs-lookup"><span data-stu-id="551cd-139">**four**</span></span>       | <span data-ttu-id="551cd-140">小数第 4 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="551cd-140">Always display four decimal places.</span></span>
| <span data-ttu-id="551cd-141">**five**</span><span class="sxs-lookup"><span data-stu-id="551cd-141">**five**</span></span>       | <span data-ttu-id="551cd-142">小数第 5 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="551cd-142">Always display five decimal places.</span></span>

<span data-ttu-id="551cd-143">注: **decimalPlaces** と **displayAs** は数値の格納方法ではなく、表示方法に適用されます。</span><span class="sxs-lookup"><span data-stu-id="551cd-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="551cd-144">これらのプロパティは更新される場合があります。</span><span class="sxs-lookup"><span data-stu-id="551cd-144">These properties may be updated.</span></span>

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
