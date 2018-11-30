---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 796bd9fc7bf379ea38dc2d2f602411740caf4b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023985"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="e557a-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e557a-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="e557a-103">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="e557a-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e557a-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e557a-104">JSON representation</span></span>

<span data-ttu-id="e557a-105">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e557a-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="e557a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e557a-106">Properties</span></span>

| <span data-ttu-id="e557a-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e557a-107">Property name</span></span> | <span data-ttu-id="e557a-108">種類</span><span class="sxs-lookup"><span data-stu-id="e557a-108">Type</span></span>   | <span data-ttu-id="e557a-109">説明</span><span class="sxs-lookup"><span data-stu-id="e557a-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e557a-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="e557a-110">**locale**</span></span>    | <span data-ttu-id="e557a-111">string</span><span class="sxs-lookup"><span data-stu-id="e557a-111">string</span></span> | <span data-ttu-id="e557a-112">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="e557a-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
