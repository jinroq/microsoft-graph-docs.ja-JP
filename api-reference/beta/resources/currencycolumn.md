---
author: JeremyKelley
description: columnDefinition リソースの currencyColumn は、列の値が通貨を表していることを示します。
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61a3c968ff48cd3bf59ec3611bc2e50a1a92a797
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973175"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="2a857-103">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a857-103">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a857-104">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="2a857-104">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a857-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a857-105">JSON representation</span></span>

<span data-ttu-id="2a857-106">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a857-106">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="2a857-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a857-107">Properties</span></span>

| <span data-ttu-id="2a857-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2a857-108">Property name</span></span> | <span data-ttu-id="2a857-109">種類</span><span class="sxs-lookup"><span data-stu-id="2a857-109">Type</span></span>   | <span data-ttu-id="2a857-110">説明</span><span class="sxs-lookup"><span data-stu-id="2a857-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2a857-111">**locale**</span><span class="sxs-lookup"><span data-stu-id="2a857-111">**locale**</span></span>    | <span data-ttu-id="2a857-112">string</span><span class="sxs-lookup"><span data-stu-id="2a857-112">string</span></span> | <span data-ttu-id="2a857-113">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a857-113">Specifies the locale from which to infer the currency symbol.</span></span>

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
