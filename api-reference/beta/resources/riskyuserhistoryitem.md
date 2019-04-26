---
title: riskyUserHistoryItem リソースの種類
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7143fffecee52747109674e81e5bfbd9860df7f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343557"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="d1fb8-102">riskyUserHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1fb8-102">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="d1fb8-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1fb8-103">Properties</span></span>

| <span data-ttu-id="d1fb8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1fb8-104">Property</span></span>       | <span data-ttu-id="d1fb8-105">型</span><span class="sxs-lookup"><span data-stu-id="d1fb8-105">Type</span></span>    | <span data-ttu-id="d1fb8-106">説明</span><span class="sxs-lookup"><span data-stu-id="d1fb8-106">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="d1fb8-107">userId</span><span class="sxs-lookup"><span data-stu-id="d1fb8-107">userId</span></span>         | <span data-ttu-id="d1fb8-108">string</span><span class="sxs-lookup"><span data-stu-id="d1fb8-108">string</span></span>  |             |
| <span data-ttu-id="d1fb8-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d1fb8-109">initiatedBy</span></span>    | <span data-ttu-id="d1fb8-110">bool</span><span class="sxs-lookup"><span data-stu-id="d1fb8-110">bool</span></span>    |             |
| <span data-ttu-id="d1fb8-111">activity</span><span class="sxs-lookup"><span data-stu-id="d1fb8-111">activity</span></span>       | [<span data-ttu-id="d1fb8-112">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="d1fb8-112">riskUserActivity</span></span>](riskuseractivity.md)| |

## <a name="json-representation"></a><span data-ttu-id="d1fb8-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1fb8-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "bool",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
