---
title: workbookFilterCriteria リソースの種類
description: 列に適用するフィルター条件を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 6e0b2b09ab464c0a04bf97ed666f3fd3a687e912
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964039"
---
# <a name="workbookfiltercriteria-resource-type"></a><span data-ttu-id="4158a-103">workbookFilterCriteria リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4158a-103">workbookFilterCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4158a-104">列に適用するフィルター条件を表します。</span><span class="sxs-lookup"><span data-stu-id="4158a-104">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4158a-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4158a-105">JSON representation</span></span>

<span data-ttu-id="4158a-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4158a-106">Here is a JSON representation of the resource.</span></span>

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
