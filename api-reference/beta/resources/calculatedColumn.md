---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: a5850961e680459af27f3e76965f0d3e1c97e923
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072918"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="8b01e-102">CalculatedColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b01e-102">CalculatedColumn resource type</span></span>

> <span data-ttu-id="8b01e-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8b01e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b01e-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b01e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b01e-105">[columnDefinition](columndefinition.md) リソースの **calculatedColumn** は、列のデータがサイト内の他の列に基づいて計算されることを示します。</span><span class="sxs-lookup"><span data-stu-id="8b01e-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b01e-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b01e-106">JSON representation</span></span>

<span data-ttu-id="8b01e-107">以下は、**calculatedColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b01e-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="8b01e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b01e-108">Properties</span></span>

| <span data-ttu-id="8b01e-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8b01e-109">Property name</span></span>  | <span data-ttu-id="8b01e-110">型</span><span class="sxs-lookup"><span data-stu-id="8b01e-110">Type</span></span>    | <span data-ttu-id="8b01e-111">説明</span><span class="sxs-lookup"><span data-stu-id="8b01e-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="8b01e-112">**format**</span><span class="sxs-lookup"><span data-stu-id="8b01e-112">**format**</span></span>     | <span data-ttu-id="8b01e-113">文字列</span><span class="sxs-lookup"><span data-stu-id="8b01e-113">string</span></span>  | <span data-ttu-id="8b01e-114">`dateTime` 出力の種類に対する値の形式。</span><span class="sxs-lookup"><span data-stu-id="8b01e-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="8b01e-115">`dateOnly` または `dateTime` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8b01e-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="8b01e-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="8b01e-116">**formula**</span></span>    | <span data-ttu-id="8b01e-117">文字列</span><span class="sxs-lookup"><span data-stu-id="8b01e-117">string</span></span>  | <span data-ttu-id="8b01e-118">この列の値を計算するために使用する数式。</span><span class="sxs-lookup"><span data-stu-id="8b01e-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="8b01e-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="8b01e-119">**outputType**</span></span> | <span data-ttu-id="8b01e-120">文字列</span><span class="sxs-lookup"><span data-stu-id="8b01e-120">string</span></span>  | <span data-ttu-id="8b01e-121">この列の値の形式を設定するために使用する出力の種類。</span><span class="sxs-lookup"><span data-stu-id="8b01e-121">The output type used to format values in this column.</span></span> <span data-ttu-id="8b01e-122">`boolean`、`currency`、`dateTime`、`number`、`text` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8b01e-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="8b01e-123">SharePoint の数式は、Excel の数式のような構文を使用します。</span><span class="sxs-lookup"><span data-stu-id="8b01e-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="8b01e-124">詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b01e-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->
