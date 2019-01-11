---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: a0f5d13381c82a42159d0802d850d9996aaf8b54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855182"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="ff22a-102">numberColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff22a-102">NumberColumn resource type</span></span>

> <span data-ttu-id="ff22a-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff22a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff22a-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff22a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff22a-105">[columnDefinition](columndefinition.md) リソースの **numberColumn** は、列の値が数値であることを示します。</span><span class="sxs-lookup"><span data-stu-id="ff22a-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff22a-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff22a-106">JSON representation</span></span>

<span data-ttu-id="ff22a-107">以下は、**numberColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff22a-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="ff22a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff22a-108">Properties</span></span>

| <span data-ttu-id="ff22a-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ff22a-109">Property name</span></span>      | <span data-ttu-id="ff22a-110">Type</span><span class="sxs-lookup"><span data-stu-id="ff22a-110">Type</span></span>   | <span data-ttu-id="ff22a-111">説明</span><span class="sxs-lookup"><span data-stu-id="ff22a-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="ff22a-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="ff22a-112">**decimalPlaces**</span></span>  | <span data-ttu-id="ff22a-113">文字列</span><span class="sxs-lookup"><span data-stu-id="ff22a-113">string</span></span> | <span data-ttu-id="ff22a-114">表示する小数点以下の桁数です。</span><span class="sxs-lookup"><span data-stu-id="ff22a-114">How many decimal places to display.</span></span> <span data-ttu-id="ff22a-115">使用可能な値については、下記を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff22a-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="ff22a-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="ff22a-116">**displayAs**</span></span>      | <span data-ttu-id="ff22a-117">文字列</span><span class="sxs-lookup"><span data-stu-id="ff22a-117">string</span></span> | <span data-ttu-id="ff22a-118">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="ff22a-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="ff22a-119">`number` または `percentage` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="ff22a-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="ff22a-120">指定しない場合、`number` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="ff22a-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="ff22a-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="ff22a-121">**maximum**</span></span>        | <span data-ttu-id="ff22a-122">double</span><span class="sxs-lookup"><span data-stu-id="ff22a-122">double</span></span> | <span data-ttu-id="ff22a-123">許容最大値です。</span><span class="sxs-lookup"><span data-stu-id="ff22a-123">The maximum permitted value.</span></span>
| <span data-ttu-id="ff22a-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="ff22a-124">**minimum**</span></span>        | <span data-ttu-id="ff22a-125">double</span><span class="sxs-lookup"><span data-stu-id="ff22a-125">double</span></span> | <span data-ttu-id="ff22a-126">許容最小値です。</span><span class="sxs-lookup"><span data-stu-id="ff22a-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="ff22a-127">DecimalPlaces values</span><span class="sxs-lookup"><span data-stu-id="ff22a-127">DecimalPlaces values</span></span>

| <span data-ttu-id="ff22a-128">値</span><span class="sxs-lookup"><span data-stu-id="ff22a-128">Value</span></span>          | <span data-ttu-id="ff22a-129">説明</span><span class="sxs-lookup"><span data-stu-id="ff22a-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="ff22a-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="ff22a-130">**automatic**</span></span>  | <span data-ttu-id="ff22a-131">既定値。</span><span class="sxs-lookup"><span data-stu-id="ff22a-131">Default.</span></span> <span data-ttu-id="ff22a-132">必要に応じて自動的に小数点以下の桁を表示します。</span><span class="sxs-lookup"><span data-stu-id="ff22a-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="ff22a-133">**none**</span><span class="sxs-lookup"><span data-stu-id="ff22a-133">**none**</span></span>       | <span data-ttu-id="ff22a-134">小数点以下の桁は表示されません。</span><span class="sxs-lookup"><span data-stu-id="ff22a-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="ff22a-135">**one**</span><span class="sxs-lookup"><span data-stu-id="ff22a-135">**one**</span></span>        | <span data-ttu-id="ff22a-136">小数第 1 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="ff22a-136">Always display one decimal place.</span></span>
| <span data-ttu-id="ff22a-137">**two**</span><span class="sxs-lookup"><span data-stu-id="ff22a-137">**two**</span></span>        | <span data-ttu-id="ff22a-138">小数第 2 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="ff22a-138">Always display two decimal places.</span></span>
| <span data-ttu-id="ff22a-139">**three**</span><span class="sxs-lookup"><span data-stu-id="ff22a-139">**three**</span></span>      | <span data-ttu-id="ff22a-140">小数第 3 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="ff22a-140">Always display three decimal places.</span></span>
| <span data-ttu-id="ff22a-141">**four**</span><span class="sxs-lookup"><span data-stu-id="ff22a-141">**four**</span></span>       | <span data-ttu-id="ff22a-142">小数第 4 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="ff22a-142">Always display four decimal places.</span></span>
| <span data-ttu-id="ff22a-143">**five**</span><span class="sxs-lookup"><span data-stu-id="ff22a-143">**five**</span></span>       | <span data-ttu-id="ff22a-144">小数第 5 位までを常に表示します。</span><span class="sxs-lookup"><span data-stu-id="ff22a-144">Always display five decimal places.</span></span>

<span data-ttu-id="ff22a-145">注: **decimalPlaces** と **displayAs** は数値の格納方法ではなく、表示方法に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ff22a-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="ff22a-146">これらのプロパティは更新される場合があります。</span><span class="sxs-lookup"><span data-stu-id="ff22a-146">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
