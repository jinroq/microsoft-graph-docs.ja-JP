---
title: locationDataModel リソースの種類
description: イベントの locationDataModel 情報を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2b1fd0c25cdd41e6a8d9c87f8a1c0c80d70b78e5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057397"
---
# <a name="locationdatamodel-resource-type"></a><span data-ttu-id="b7361-103">locationDataModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7361-103">locationDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7361-104">会議の場所情報を表します。</span><span class="sxs-lookup"><span data-stu-id="b7361-104">Represents location information for a meeting.</span></span>


## <a name="properties"></a><span data-ttu-id="b7361-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7361-105">Properties</span></span>
| <span data-ttu-id="b7361-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7361-106">Property</span></span>  | <span data-ttu-id="b7361-107">型</span><span class="sxs-lookup"><span data-stu-id="b7361-107">Type</span></span>   | <span data-ttu-id="b7361-108">説明</span><span class="sxs-lookup"><span data-stu-id="b7361-108">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="b7361-109">address</span><span class="sxs-lookup"><span data-stu-id="b7361-109">address</span></span> | [<span data-ttu-id="b7361-110">"postaladdress</span><span class="sxs-lookup"><span data-stu-id="b7361-110">postalAddress</span></span>](postaladdress.md) |<span data-ttu-id="b7361-111">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="b7361-111">The street address of the location.</span></span> |
| <span data-ttu-id="b7361-112">coordinates</span><span class="sxs-lookup"><span data-stu-id="b7361-112">coordinates</span></span> | [<span data-ttu-id="b7361-113">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b7361-113">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="b7361-114">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="b7361-114">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="b7361-115">displayName</span><span class="sxs-lookup"><span data-stu-id="b7361-115">displayName</span></span>  | <span data-ttu-id="b7361-116">文字列</span><span class="sxs-lookup"><span data-stu-id="b7361-116">String</span></span> | <span data-ttu-id="b7361-117">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="b7361-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="b7361-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b7361-118">locationEmailAddress</span></span> | <span data-ttu-id="b7361-119">String</span><span class="sxs-lookup"><span data-stu-id="b7361-119">String</span></span> | <span data-ttu-id="b7361-120">場所のメール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="b7361-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="b7361-121">locationUri</span><span class="sxs-lookup"><span data-stu-id="b7361-121">locationUri</span></span> | <span data-ttu-id="b7361-122">String</span><span class="sxs-lookup"><span data-stu-id="b7361-122">String</span></span> | <span data-ttu-id="b7361-123">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="b7361-123">Optional URI representing the location.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b7361-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7361-124">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationDataModel"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
