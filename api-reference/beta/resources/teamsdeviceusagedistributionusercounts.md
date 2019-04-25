---
title: teamsDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d398782cef79cdf92bc56502f7c6cbf1bcdee99d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553611"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="c343a-103">teamsDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c343a-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c343a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c343a-104">Properties</span></span>

| <span data-ttu-id="c343a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c343a-105">Property</span></span>          | <span data-ttu-id="c343a-106">型</span><span class="sxs-lookup"><span data-stu-id="c343a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c343a-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="c343a-107">reportRefreshDate</span></span> | <span data-ttu-id="c343a-108">Date</span><span class="sxs-lookup"><span data-stu-id="c343a-108">Date</span></span>   |
| <span data-ttu-id="c343a-109">web</span><span class="sxs-lookup"><span data-stu-id="c343a-109">web</span></span>               | <span data-ttu-id="c343a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c343a-110">Int64</span></span>  |
| <span data-ttu-id="c343a-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="c343a-111">windowsPhone</span></span>      | <span data-ttu-id="c343a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c343a-112">Int64</span></span>  |
| <span data-ttu-id="c343a-113">androidphone</span><span class="sxs-lookup"><span data-stu-id="c343a-113">androidPhone</span></span>      | <span data-ttu-id="c343a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c343a-114">Int64</span></span>  |
| <span data-ttu-id="c343a-115">ios</span><span class="sxs-lookup"><span data-stu-id="c343a-115">ios</span></span>               | <span data-ttu-id="c343a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c343a-116">Int64</span></span>  |
| <span data-ttu-id="c343a-117">Mac</span><span class="sxs-lookup"><span data-stu-id="c343a-117">mac</span></span>               | <span data-ttu-id="c343a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c343a-118">Int64</span></span>  |
| <span data-ttu-id="c343a-119">ws</span><span class="sxs-lookup"><span data-stu-id="c343a-119">windows</span></span>           | <span data-ttu-id="c343a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c343a-120">Int64</span></span>  |
| <span data-ttu-id="c343a-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="c343a-121">reportPeriod</span></span>      | <span data-ttu-id="c343a-122">String</span><span class="sxs-lookup"><span data-stu-id="c343a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c343a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c343a-123">JSON representation</span></span>

<span data-ttu-id="c343a-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c343a-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportPeriod": "String"
}
```
