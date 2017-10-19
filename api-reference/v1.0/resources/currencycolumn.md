---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 4f3ae97e5abfb84ad523caf74fa70b1f1ec0322a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="71323-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71323-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="71323-103">[columnDefinition](columnDefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="71323-103">The **currencyColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71323-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71323-104">JSON representation</span></span>

<span data-ttu-id="71323-105">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71323-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="71323-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71323-106">Properties</span></span>

| <span data-ttu-id="71323-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="71323-107">Property name</span></span> | <span data-ttu-id="71323-108">種類</span><span class="sxs-lookup"><span data-stu-id="71323-108">Type</span></span>   | <span data-ttu-id="71323-109">説明</span><span class="sxs-lookup"><span data-stu-id="71323-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="71323-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="71323-110">**Locale**</span></span>    | <span data-ttu-id="71323-111">string</span><span class="sxs-lookup"><span data-stu-id="71323-111">string</span></span> | <span data-ttu-id="71323-112">通貨記号を推測する基となるロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="71323-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
