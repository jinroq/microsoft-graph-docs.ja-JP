---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: 7e26b3683c2c84d1c413f3214da39e0a3d016f40
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267844"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="c8382-102">CalculatedColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8382-102">CalculatedColumn resource type</span></span>

<span data-ttu-id="c8382-103">[columnDefinition](columnDefinition.md) リソースの **calculatedColumn** は、列のデータがサイト内の他の列に基づいて計算されることを示します。</span><span class="sxs-lookup"><span data-stu-id="c8382-103">The **calculatedColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8382-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8382-104">JSON representation</span></span>

<span data-ttu-id="c8382-105">以下は、**calculatedColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8382-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="c8382-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8382-106">Properties</span></span>

| <span data-ttu-id="c8382-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="c8382-107">Property name</span></span>  | <span data-ttu-id="c8382-108">型</span><span class="sxs-lookup"><span data-stu-id="c8382-108">Type</span></span>    | <span data-ttu-id="c8382-109">説明</span><span class="sxs-lookup"><span data-stu-id="c8382-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="c8382-110">**書式設定**</span><span class="sxs-lookup"><span data-stu-id="c8382-110">**format**</span></span>     | <span data-ttu-id="c8382-111">文字列</span><span class="sxs-lookup"><span data-stu-id="c8382-111">string</span></span>  | <span data-ttu-id="c8382-112">出力の種類に対する値の形式。`dateTime`</span><span class="sxs-lookup"><span data-stu-id="c8382-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="c8382-113">または `dateTime` のいずれかでなければなりません。`dateOnly`</span><span class="sxs-lookup"><span data-stu-id="c8382-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="c8382-114">**数式**</span><span class="sxs-lookup"><span data-stu-id="c8382-114">**formula**</span></span>    | <span data-ttu-id="c8382-115">文字列</span><span class="sxs-lookup"><span data-stu-id="c8382-115">string</span></span>  | <span data-ttu-id="c8382-116">この列の値を計算するために使用する数式。</span><span class="sxs-lookup"><span data-stu-id="c8382-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="c8382-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="c8382-117">**outputType**</span></span> | <span data-ttu-id="c8382-118">文字列</span><span class="sxs-lookup"><span data-stu-id="c8382-118">string</span></span>  | <span data-ttu-id="c8382-119">この列の値の形式を設定するために使用する出力の種類。</span><span class="sxs-lookup"><span data-stu-id="c8382-119">The output type used to format values in this column.</span></span> <span data-ttu-id="c8382-120">、`currency`、`dateTime`、`number`、`text` のいずれかでなければなりません。`boolean`</span><span class="sxs-lookup"><span data-stu-id="c8382-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="c8382-121">SharePoint の数式は、Excel の数式のような構文を使用します。</span><span class="sxs-lookup"><span data-stu-id="c8382-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="c8382-122">詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8382-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->
