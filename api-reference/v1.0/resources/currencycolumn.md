---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: e4ee085882cadafc0102ee31e17841978cef7822
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836457"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="41c0b-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41c0b-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="41c0b-103">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="41c0b-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41c0b-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41c0b-104">JSON representation</span></span>

<span data-ttu-id="41c0b-105">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41c0b-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="41c0b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41c0b-106">Properties</span></span>

| <span data-ttu-id="41c0b-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="41c0b-107">Property name</span></span> | <span data-ttu-id="41c0b-108">種類</span><span class="sxs-lookup"><span data-stu-id="41c0b-108">Type</span></span>   | <span data-ttu-id="41c0b-109">説明</span><span class="sxs-lookup"><span data-stu-id="41c0b-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="41c0b-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="41c0b-110">**locale**</span></span>    | <span data-ttu-id="41c0b-111">string</span><span class="sxs-lookup"><span data-stu-id="41c0b-111">string</span></span> | <span data-ttu-id="41c0b-112">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="41c0b-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
