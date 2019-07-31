---
author: JeremyKelley
description: columnDefinition リソースの calculatedColumn は、列のデータがサイト内の他の列に基づいて計算されることを示します。
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8492dcf39cbdee92a998a418599fc00b314078c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013060"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="bd585-103">CalculatedColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd585-103">CalculatedColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd585-104">[columnDefinition](columndefinition.md) リソースの **calculatedColumn** は、列のデータがサイト内の他の列に基づいて計算されることを示します。</span><span class="sxs-lookup"><span data-stu-id="bd585-104">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd585-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd585-105">JSON representation</span></span>

<span data-ttu-id="bd585-106">以下は、**calculatedColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bd585-106">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="bd585-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd585-107">Properties</span></span>

| <span data-ttu-id="bd585-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="bd585-108">Property name</span></span>  | <span data-ttu-id="bd585-109">種類</span><span class="sxs-lookup"><span data-stu-id="bd585-109">Type</span></span>    | <span data-ttu-id="bd585-110">説明</span><span class="sxs-lookup"><span data-stu-id="bd585-110">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="bd585-111">**format**</span><span class="sxs-lookup"><span data-stu-id="bd585-111">**format**</span></span>     | <span data-ttu-id="bd585-112">string</span><span class="sxs-lookup"><span data-stu-id="bd585-112">string</span></span>  | <span data-ttu-id="bd585-113">`dateTime` 出力の種類に対する値の形式。</span><span class="sxs-lookup"><span data-stu-id="bd585-113">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="bd585-114">`dateOnly` または `dateTime` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="bd585-114">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="bd585-115">**formula**</span><span class="sxs-lookup"><span data-stu-id="bd585-115">**formula**</span></span>    | <span data-ttu-id="bd585-116">string</span><span class="sxs-lookup"><span data-stu-id="bd585-116">string</span></span>  | <span data-ttu-id="bd585-117">この列の値を計算するために使用する数式。</span><span class="sxs-lookup"><span data-stu-id="bd585-117">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="bd585-118">**outputType**</span><span class="sxs-lookup"><span data-stu-id="bd585-118">**outputType**</span></span> | <span data-ttu-id="bd585-119">string</span><span class="sxs-lookup"><span data-stu-id="bd585-119">string</span></span>  | <span data-ttu-id="bd585-120">この列の値の形式を設定するために使用する出力の種類。</span><span class="sxs-lookup"><span data-stu-id="bd585-120">The output type used to format values in this column.</span></span> <span data-ttu-id="bd585-121">`boolean`、`currency`、`dateTime`、`number`、`text` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="bd585-121">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="bd585-122">SharePoint の数式は、Excel の数式のような構文を使用します。</span><span class="sxs-lookup"><span data-stu-id="bd585-122">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="bd585-123">詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd585-123">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": []
}
-->
