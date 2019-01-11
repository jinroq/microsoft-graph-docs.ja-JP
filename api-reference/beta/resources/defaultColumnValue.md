---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
ms.openlocfilehash: 6ceca45d09654771f161db63707682a4558b0d29
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815548"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="07aae-102">DefaultColumnValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="07aae-102">DefaultColumnValue resource type</span></span>

> <span data-ttu-id="07aae-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07aae-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07aae-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07aae-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07aae-105">[columnDefinition](columndefinition.md) リソースの **defaultColumnValue** は、この列の既定値を指定します。</span><span class="sxs-lookup"><span data-stu-id="07aae-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="07aae-106">既定値は直接または数式として指定できます。</span><span class="sxs-lookup"><span data-stu-id="07aae-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07aae-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07aae-107">JSON representation</span></span>

<span data-ttu-id="07aae-108">以下は、**defaultColumnValue** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="07aae-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="07aae-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07aae-109">Properties</span></span>

| <span data-ttu-id="07aae-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="07aae-110">Property name</span></span> | <span data-ttu-id="07aae-111">Type</span><span class="sxs-lookup"><span data-stu-id="07aae-111">Type</span></span>   | <span data-ttu-id="07aae-112">説明</span><span class="sxs-lookup"><span data-stu-id="07aae-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="07aae-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="07aae-113">**formula**</span></span>   | <span data-ttu-id="07aae-114">文字列</span><span class="sxs-lookup"><span data-stu-id="07aae-114">string</span></span> | <span data-ttu-id="07aae-115">この列の既定値を計算するために使用する数式。</span><span class="sxs-lookup"><span data-stu-id="07aae-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="07aae-116">**value**</span><span class="sxs-lookup"><span data-stu-id="07aae-116">**value**</span></span>     | <span data-ttu-id="07aae-117">文字列</span><span class="sxs-lookup"><span data-stu-id="07aae-117">string</span></span> | <span data-ttu-id="07aae-118">この列の既定値として使用する直接値。</span><span class="sxs-lookup"><span data-stu-id="07aae-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="07aae-119">一度に**数式**または**値**のうちの 1 つだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="07aae-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="07aae-120">SharePoint の数式は、Excel の数式のような構文を使用します。</span><span class="sxs-lookup"><span data-stu-id="07aae-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="07aae-121">詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07aae-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
