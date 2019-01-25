---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: c89d709c93eeee0003d193d620166f8abffd9d41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524500"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="8cf7d-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cf7d-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cf7d-103">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="8cf7d-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cf7d-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cf7d-104">JSON representation</span></span>

<span data-ttu-id="8cf7d-105">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cf7d-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="8cf7d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cf7d-106">Properties</span></span>

| <span data-ttu-id="8cf7d-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8cf7d-107">Property name</span></span> | <span data-ttu-id="8cf7d-108">種類</span><span class="sxs-lookup"><span data-stu-id="8cf7d-108">Type</span></span>   | <span data-ttu-id="8cf7d-109">説明</span><span class="sxs-lookup"><span data-stu-id="8cf7d-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8cf7d-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="8cf7d-110">**locale**</span></span>    | <span data-ttu-id="8cf7d-111">string</span><span class="sxs-lookup"><span data-stu-id="8cf7d-111">string</span></span> | <span data-ttu-id="8cf7d-112">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="8cf7d-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/currencycolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
