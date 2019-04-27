---
title: workbookFilterCriteria リソースの種類
description: 列に適用するフィルター条件を表します。
localization_priority: Normal
ms.openlocfilehash: 4906a44c88fdd7cb071b4ea994fee609cda1151c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348883"
---
# <a name="workbookfiltercriteria-resource-type"></a><span data-ttu-id="b3dd7-103">workbookFilterCriteria リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3dd7-103">workbookFilterCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3dd7-104">列に適用するフィルター条件を表します。</span><span class="sxs-lookup"><span data-stu-id="b3dd7-104">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3dd7-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3dd7-105">JSON representation</span></span>

<span data-ttu-id="b3dd7-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3dd7-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": {"@odata.type":"microsoft.graph.Json"},
  "icon":{"@odata.type": "microsoft.graph.workbookIcon"},
  "operator":"string"
}
```
