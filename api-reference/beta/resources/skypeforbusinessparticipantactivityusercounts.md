---
title: skypeForBusinessParticipantActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 6579552ef3ca5e9fefe8690a161bef4752ad2492
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853005"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="1810f-103">skypeForBusinessParticipantActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1810f-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1810f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1810f-104">Properties</span></span>

| <span data-ttu-id="1810f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1810f-105">Property</span></span>          | <span data-ttu-id="1810f-106">種類</span><span class="sxs-lookup"><span data-stu-id="1810f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1810f-107">im</span><span class="sxs-lookup"><span data-stu-id="1810f-107">im</span></span>                | <span data-ttu-id="1810f-108">Int64</span><span class="sxs-lookup"><span data-stu-id="1810f-108">Int64</span></span>  |
| <span data-ttu-id="1810f-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="1810f-109">audioVideo</span></span>        | <span data-ttu-id="1810f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1810f-110">Int64</span></span>  |
| <span data-ttu-id="1810f-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="1810f-111">appSharing</span></span>        | <span data-ttu-id="1810f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1810f-112">Int64</span></span>  |
| <span data-ttu-id="1810f-113">web</span><span class="sxs-lookup"><span data-stu-id="1810f-113">web</span></span>               | <span data-ttu-id="1810f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1810f-114">Int64</span></span>  |
| <span data-ttu-id="1810f-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="1810f-115">dialInOut3rdParty</span></span> | <span data-ttu-id="1810f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1810f-116">Int64</span></span>  |
| <span data-ttu-id="1810f-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1810f-117">reportRefreshDate</span></span> | <span data-ttu-id="1810f-118">日付</span><span class="sxs-lookup"><span data-stu-id="1810f-118">Date</span></span>   |
| <span data-ttu-id="1810f-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="1810f-119">reportDate</span></span>        | <span data-ttu-id="1810f-120">日付</span><span class="sxs-lookup"><span data-stu-id="1810f-120">Date</span></span>   |
| <span data-ttu-id="1810f-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1810f-121">reportPeriod</span></span>      | <span data-ttu-id="1810f-122">String</span><span class="sxs-lookup"><span data-stu-id="1810f-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1810f-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1810f-123">JSON representation</span></span>

<span data-ttu-id="1810f-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1810f-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 196, 
  "appSharing": 196, 
  "web": 196, 
  "dialInOut3rdParty": 196, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
