---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: columnDefinition リソースの defaultColumnValue は、この列の既定値を指定します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4a2ddff8de7efb2bb697ffae63d69376588e6ac9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029513"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="a501e-103">DefaultColumnValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a501e-103">DefaultColumnValue resource type</span></span>

<span data-ttu-id="a501e-104">[columnDefinition](columndefinition.md) リソースの **defaultColumnValue** は、この列の既定値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a501e-104">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="a501e-105">既定値は直接または数式として指定できます。</span><span class="sxs-lookup"><span data-stu-id="a501e-105">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a501e-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a501e-106">JSON representation</span></span>

<span data-ttu-id="a501e-107">以下は、**defaultColumnValue** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a501e-107">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="a501e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a501e-108">Properties</span></span>

| <span data-ttu-id="a501e-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a501e-109">Property name</span></span> | <span data-ttu-id="a501e-110">種類</span><span class="sxs-lookup"><span data-stu-id="a501e-110">Type</span></span>   | <span data-ttu-id="a501e-111">説明</span><span class="sxs-lookup"><span data-stu-id="a501e-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a501e-112">**formula**</span><span class="sxs-lookup"><span data-stu-id="a501e-112">**formula**</span></span>   | <span data-ttu-id="a501e-113">string</span><span class="sxs-lookup"><span data-stu-id="a501e-113">string</span></span> | <span data-ttu-id="a501e-114">この列の既定値を計算するために使用する数式。</span><span class="sxs-lookup"><span data-stu-id="a501e-114">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="a501e-115">**value**</span><span class="sxs-lookup"><span data-stu-id="a501e-115">**value**</span></span>     | <span data-ttu-id="a501e-116">string</span><span class="sxs-lookup"><span data-stu-id="a501e-116">string</span></span> | <span data-ttu-id="a501e-117">この列の既定値として使用する直接値。</span><span class="sxs-lookup"><span data-stu-id="a501e-117">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="a501e-118">一度に**数式**または**値**のうちの 1 つだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="a501e-118">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="a501e-119">SharePoint の数式は、Excel の数式のような構文を使用します。</span><span class="sxs-lookup"><span data-stu-id="a501e-119">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="a501e-120">詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a501e-120">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
