---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 065ac52a4d5216a4b3e62df892c8fe0a07a82ed0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481532"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="693d2-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="693d2-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="693d2-103">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="693d2-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="693d2-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="693d2-104">JSON representation</span></span>

<span data-ttu-id="693d2-105">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="693d2-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="693d2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="693d2-106">Properties</span></span>

| <span data-ttu-id="693d2-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="693d2-107">Property name</span></span> | <span data-ttu-id="693d2-108">種類</span><span class="sxs-lookup"><span data-stu-id="693d2-108">Type</span></span>   | <span data-ttu-id="693d2-109">説明</span><span class="sxs-lookup"><span data-stu-id="693d2-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="693d2-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="693d2-110">**locale**</span></span>    | <span data-ttu-id="693d2-111">string</span><span class="sxs-lookup"><span data-stu-id="693d2-111">string</span></span> | <span data-ttu-id="693d2-112">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="693d2-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
