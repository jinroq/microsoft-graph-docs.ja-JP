---
title: skypeForBusinessParticipantActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 6579552ef3ca5e9fefe8690a161bef4752ad2492
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568118"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="f8966-103">skypeForBusinessParticipantActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f8966-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f8966-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8966-104">Properties</span></span>

| <span data-ttu-id="f8966-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8966-105">Property</span></span>          | <span data-ttu-id="f8966-106">型</span><span class="sxs-lookup"><span data-stu-id="f8966-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f8966-107">im</span><span class="sxs-lookup"><span data-stu-id="f8966-107">im</span></span>                | <span data-ttu-id="f8966-108">Int64</span><span class="sxs-lookup"><span data-stu-id="f8966-108">Int64</span></span>  |
| <span data-ttu-id="f8966-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="f8966-109">audioVideo</span></span>        | <span data-ttu-id="f8966-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f8966-110">Int64</span></span>  |
| <span data-ttu-id="f8966-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="f8966-111">appSharing</span></span>        | <span data-ttu-id="f8966-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f8966-112">Int64</span></span>  |
| <span data-ttu-id="f8966-113">web</span><span class="sxs-lookup"><span data-stu-id="f8966-113">web</span></span>               | <span data-ttu-id="f8966-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f8966-114">Int64</span></span>  |
| <span data-ttu-id="f8966-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="f8966-115">dialInOut3rdParty</span></span> | <span data-ttu-id="f8966-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f8966-116">Int64</span></span>  |
| <span data-ttu-id="f8966-117">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="f8966-117">reportRefreshDate</span></span> | <span data-ttu-id="f8966-118">Date</span><span class="sxs-lookup"><span data-stu-id="f8966-118">Date</span></span>   |
| <span data-ttu-id="f8966-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="f8966-119">reportDate</span></span>        | <span data-ttu-id="f8966-120">Date</span><span class="sxs-lookup"><span data-stu-id="f8966-120">Date</span></span>   |
| <span data-ttu-id="f8966-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="f8966-121">reportPeriod</span></span>      | <span data-ttu-id="f8966-122">String</span><span class="sxs-lookup"><span data-stu-id="f8966-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f8966-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8966-123">JSON representation</span></span>

<span data-ttu-id="f8966-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f8966-124">The following is a JSON representation of the resource.</span></span>

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
