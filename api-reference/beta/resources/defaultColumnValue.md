---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
ms.openlocfilehash: ad94cadaa26d0fab72236d4037ceffd09a52c561
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514279"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="17c7d-102">DefaultColumnValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17c7d-102">DefaultColumnValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17c7d-103">[columnDefinition](columndefinition.md) リソースの **defaultColumnValue** は、この列の既定値を指定します。</span><span class="sxs-lookup"><span data-stu-id="17c7d-103">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="17c7d-104">既定値は直接または数式として指定できます。</span><span class="sxs-lookup"><span data-stu-id="17c7d-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17c7d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17c7d-105">JSON representation</span></span>

<span data-ttu-id="17c7d-106">以下は、**defaultColumnValue** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17c7d-106">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="17c7d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17c7d-107">Properties</span></span>

| <span data-ttu-id="17c7d-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="17c7d-108">Property name</span></span> | <span data-ttu-id="17c7d-109">種類</span><span class="sxs-lookup"><span data-stu-id="17c7d-109">Type</span></span>   | <span data-ttu-id="17c7d-110">説明</span><span class="sxs-lookup"><span data-stu-id="17c7d-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="17c7d-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="17c7d-111">**formula**</span></span>   | <span data-ttu-id="17c7d-112">string</span><span class="sxs-lookup"><span data-stu-id="17c7d-112">string</span></span> | <span data-ttu-id="17c7d-113">この列の既定値を計算するために使用する数式。</span><span class="sxs-lookup"><span data-stu-id="17c7d-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="17c7d-114">**value**</span><span class="sxs-lookup"><span data-stu-id="17c7d-114">**value**</span></span>     | <span data-ttu-id="17c7d-115">string</span><span class="sxs-lookup"><span data-stu-id="17c7d-115">string</span></span> | <span data-ttu-id="17c7d-116">この列の既定値として使用する直接値。</span><span class="sxs-lookup"><span data-stu-id="17c7d-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="17c7d-117">一度に**数式**または**値**のうちの 1 つだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="17c7d-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="17c7d-118">SharePoint の数式は、Excel の数式のような構文を使用します。</span><span class="sxs-lookup"><span data-stu-id="17c7d-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="17c7d-119">詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17c7d-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": [
    "Error: /api-reference/beta/resources/defaultColumnValue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
