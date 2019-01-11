---
title: teamsDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: a02dfa5a5036d67a624656d715c0fb0d3c8194ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868699"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="815e0-103">teamsDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="815e0-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="815e0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="815e0-104">Properties</span></span>

| <span data-ttu-id="815e0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="815e0-105">Property</span></span>          | <span data-ttu-id="815e0-106">種類</span><span class="sxs-lookup"><span data-stu-id="815e0-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="815e0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="815e0-107">reportRefreshDate</span></span> | <span data-ttu-id="815e0-108">日付</span><span class="sxs-lookup"><span data-stu-id="815e0-108">Date</span></span>   |
| <span data-ttu-id="815e0-109">web</span><span class="sxs-lookup"><span data-stu-id="815e0-109">web</span></span>               | <span data-ttu-id="815e0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="815e0-110">Int64</span></span>  |
| <span data-ttu-id="815e0-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="815e0-111">windowsPhone</span></span>      | <span data-ttu-id="815e0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="815e0-112">Int64</span></span>  |
| <span data-ttu-id="815e0-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="815e0-113">androidPhone</span></span>      | <span data-ttu-id="815e0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="815e0-114">Int64</span></span>  |
| <span data-ttu-id="815e0-115">ios</span><span class="sxs-lookup"><span data-stu-id="815e0-115">ios</span></span>               | <span data-ttu-id="815e0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="815e0-116">Int64</span></span>  |
| <span data-ttu-id="815e0-117">Mac</span><span class="sxs-lookup"><span data-stu-id="815e0-117">mac</span></span>               | <span data-ttu-id="815e0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="815e0-118">Int64</span></span>  |
| <span data-ttu-id="815e0-119">windows</span><span class="sxs-lookup"><span data-stu-id="815e0-119">windows</span></span>           | <span data-ttu-id="815e0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="815e0-120">Int64</span></span>  |
| <span data-ttu-id="815e0-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="815e0-121">reportPeriod</span></span>      | <span data-ttu-id="815e0-122">String</span><span class="sxs-lookup"><span data-stu-id="815e0-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="815e0-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="815e0-123">JSON representation</span></span>

<span data-ttu-id="815e0-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="815e0-124">The following is a JSON representation of the resource.</span></span>

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
