---
title: accessReviewRecurrenceSettings リソースの種類
description: ''
localization_priority: Normal
ms.openlocfilehash: 1a5235639209830d36cf69c027cfd309fab09c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348403"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="f5cda-102">accessReviewRecurrenceSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5cda-102">accessReviewRecurrenceSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="f5cda-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5cda-103">Properties</span></span>
|<span data-ttu-id="f5cda-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5cda-104">Property</span></span>|<span data-ttu-id="f5cda-105">型</span><span class="sxs-lookup"><span data-stu-id="f5cda-105">Type</span></span>|<span data-ttu-id="f5cda-106">説明</span><span class="sxs-lookup"><span data-stu-id="f5cda-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="f5cda-107">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="f5cda-107">recurrenceType</span></span> | <span data-ttu-id="f5cda-108">string</span><span class="sxs-lookup"><span data-stu-id="f5cda-108">string</span></span> |  |
| <span data-ttu-id="f5cda-109">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="f5cda-109">recurrenceEndType</span></span> | <span data-ttu-id="f5cda-110">string</span><span class="sxs-lookup"><span data-stu-id="f5cda-110">string</span></span> |  |
| <span data-ttu-id="f5cda-111">durationInDays</span><span class="sxs-lookup"><span data-stu-id="f5cda-111">durationInDays</span></span> | <span data-ttu-id="f5cda-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f5cda-112">Int32</span></span> |  |
| <span data-ttu-id="f5cda-113">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="f5cda-113">recurrenceCount</span></span> | <span data-ttu-id="f5cda-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f5cda-114">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="f5cda-115">関係</span><span class="sxs-lookup"><span data-stu-id="f5cda-115">Relationships</span></span>
<span data-ttu-id="f5cda-116">なし</span><span class="sxs-lookup"><span data-stu-id="f5cda-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5cda-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5cda-117">JSON Representation</span></span>
<span data-ttu-id="f5cda-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5cda-118">Here is a JSON representation of the resource.</span></span>
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



