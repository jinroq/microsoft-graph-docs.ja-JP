---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
ms.openlocfilehash: 73761e224a59b3a9a4206d5e1cfb058294b7f53b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="f3e8f-102">DefaultColumnValue リソース型</span><span class="sxs-lookup"><span data-stu-id="f3e8f-102">DefaultColumnValue resource type</span></span>

<span data-ttu-id="f3e8f-103">[columnDefinition](columnDefinition.md) リソースの **defaultColumnValue** は、この列の既定値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e8f-103">The **defaultColumnValue** on a [columnDefinition](columnDefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="f3e8f-104">既定値は直接または数式として指定できます。</span><span class="sxs-lookup"><span data-stu-id="f3e8f-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3e8f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3e8f-105">JSON representation</span></span>

<span data-ttu-id="f3e8f-106">以下は、**defaultColumnValue** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3e8f-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="f3e8f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3e8f-107">Properties</span></span>

| <span data-ttu-id="f3e8f-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f3e8f-108">Property name</span></span> | <span data-ttu-id="f3e8f-109">種類</span><span class="sxs-lookup"><span data-stu-id="f3e8f-109">Type</span></span>   | <span data-ttu-id="f3e8f-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3e8f-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f3e8f-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="f3e8f-111">**formula**</span></span>   | <span data-ttu-id="f3e8f-112">string</span><span class="sxs-lookup"><span data-stu-id="f3e8f-112">string</span></span> | <span data-ttu-id="f3e8f-113">この列の既定値を計算するために使用する数式。</span><span class="sxs-lookup"><span data-stu-id="f3e8f-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="f3e8f-114">**value**</span><span class="sxs-lookup"><span data-stu-id="f3e8f-114">**value**</span></span>     | <span data-ttu-id="f3e8f-115">string</span><span class="sxs-lookup"><span data-stu-id="f3e8f-115">string</span></span> | <span data-ttu-id="f3e8f-116">この列の既定値として使用する直接値。</span><span class="sxs-lookup"><span data-stu-id="f3e8f-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="f3e8f-117">一度に **formula** または **value** のうちの 1 つだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="f3e8f-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="f3e8f-118">SharePoint の数式は、Excel の数式のような構文を使用します。</span><span class="sxs-lookup"><span data-stu-id="f3e8f-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="f3e8f-119">詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3e8f-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
