---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
description: columnDefinition リソースの currencyColumn は、列の値が通貨を表していることを示します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d01ae79c8c271f1076d14e44f5f4cb5b147f4b79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029569"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="523cb-103">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="523cb-103">CurrencyColumn resource type</span></span>

<span data-ttu-id="523cb-104">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="523cb-104">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="523cb-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="523cb-105">JSON representation</span></span>

<span data-ttu-id="523cb-106">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="523cb-106">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="523cb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="523cb-107">Properties</span></span>

| <span data-ttu-id="523cb-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="523cb-108">Property name</span></span> | <span data-ttu-id="523cb-109">種類</span><span class="sxs-lookup"><span data-stu-id="523cb-109">Type</span></span>   | <span data-ttu-id="523cb-110">説明</span><span class="sxs-lookup"><span data-stu-id="523cb-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="523cb-111">**locale**</span><span class="sxs-lookup"><span data-stu-id="523cb-111">**locale**</span></span>    | <span data-ttu-id="523cb-112">string</span><span class="sxs-lookup"><span data-stu-id="523cb-112">string</span></span> | <span data-ttu-id="523cb-113">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="523cb-113">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
