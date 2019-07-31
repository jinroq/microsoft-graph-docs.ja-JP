---
title: accessReviewRecurrenceSettings リソースの種類
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: ''
ms.openlocfilehash: 2bf71fe1c715eb96e98b0caf7720cc0d637ee33b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974537"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="6db9d-102">accessReviewRecurrenceSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6db9d-102">accessReviewRecurrenceSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="6db9d-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6db9d-103">Properties</span></span>
|<span data-ttu-id="6db9d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6db9d-104">Property</span></span>|<span data-ttu-id="6db9d-105">型</span><span class="sxs-lookup"><span data-stu-id="6db9d-105">Type</span></span>|<span data-ttu-id="6db9d-106">説明</span><span class="sxs-lookup"><span data-stu-id="6db9d-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="6db9d-107">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="6db9d-107">recurrenceType</span></span> | <span data-ttu-id="6db9d-108">string</span><span class="sxs-lookup"><span data-stu-id="6db9d-108">string</span></span> |  |
| <span data-ttu-id="6db9d-109">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="6db9d-109">recurrenceEndType</span></span> | <span data-ttu-id="6db9d-110">string</span><span class="sxs-lookup"><span data-stu-id="6db9d-110">string</span></span> |  |
| <span data-ttu-id="6db9d-111">durationInDays</span><span class="sxs-lookup"><span data-stu-id="6db9d-111">durationInDays</span></span> | <span data-ttu-id="6db9d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6db9d-112">Int32</span></span> |  |
| <span data-ttu-id="6db9d-113">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="6db9d-113">recurrenceCount</span></span> | <span data-ttu-id="6db9d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6db9d-114">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="6db9d-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6db9d-115">Relationships</span></span>
<span data-ttu-id="6db9d-116">なし</span><span class="sxs-lookup"><span data-stu-id="6db9d-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6db9d-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6db9d-117">JSON Representation</span></span>
<span data-ttu-id="6db9d-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6db9d-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
``` json
{
    "recurrenceType":"string",
    "recurrenceEndType":"string",
    "durationInDays":"Int32",
    "recurrenceCount":"Int32"
}
```



