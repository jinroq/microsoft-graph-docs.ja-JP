---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: f38fc2a29a5fdee77456a5ceee7c7689cfe3f412
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543232"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="f2ed1-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2ed1-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="f2ed1-103">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="f2ed1-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2ed1-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2ed1-104">JSON representation</span></span>

<span data-ttu-id="f2ed1-105">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2ed1-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="f2ed1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2ed1-106">Properties</span></span>

| <span data-ttu-id="f2ed1-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f2ed1-107">Property name</span></span> | <span data-ttu-id="f2ed1-108">種類</span><span class="sxs-lookup"><span data-stu-id="f2ed1-108">Type</span></span>   | <span data-ttu-id="f2ed1-109">説明</span><span class="sxs-lookup"><span data-stu-id="f2ed1-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f2ed1-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="f2ed1-110">**locale**</span></span>    | <span data-ttu-id="f2ed1-111">string</span><span class="sxs-lookup"><span data-stu-id="f2ed1-111">string</span></span> | <span data-ttu-id="f2ed1-112">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="f2ed1-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
