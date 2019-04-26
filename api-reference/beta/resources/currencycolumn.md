---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 8b39f20830da6621b1b6379674d5ef191afe5d9f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341027"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="b0b62-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0b62-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0b62-103">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="b0b62-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0b62-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0b62-104">JSON representation</span></span>

<span data-ttu-id="b0b62-105">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0b62-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="b0b62-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0b62-106">Properties</span></span>

| <span data-ttu-id="b0b62-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b0b62-107">Property name</span></span> | <span data-ttu-id="b0b62-108">種類</span><span class="sxs-lookup"><span data-stu-id="b0b62-108">Type</span></span>   | <span data-ttu-id="b0b62-109">説明</span><span class="sxs-lookup"><span data-stu-id="b0b62-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b0b62-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="b0b62-110">**locale**</span></span>    | <span data-ttu-id="b0b62-111">string</span><span class="sxs-lookup"><span data-stu-id="b0b62-111">string</span></span> | <span data-ttu-id="b0b62-112">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="b0b62-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": []
}
-->
