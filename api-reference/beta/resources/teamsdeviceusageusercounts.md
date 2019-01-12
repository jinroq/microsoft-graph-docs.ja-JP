---
title: teamsDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 671dfada02b9c16d3392d0a97023b82020fd1218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987399"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="8d733-103">teamsDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d733-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8d733-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d733-104">Properties</span></span>

| <span data-ttu-id="8d733-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d733-105">Property</span></span>          | <span data-ttu-id="8d733-106">種類</span><span class="sxs-lookup"><span data-stu-id="8d733-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8d733-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8d733-107">reportRefreshDate</span></span> | <span data-ttu-id="8d733-108">日付</span><span class="sxs-lookup"><span data-stu-id="8d733-108">Date</span></span>   |
| <span data-ttu-id="8d733-109">web</span><span class="sxs-lookup"><span data-stu-id="8d733-109">web</span></span>               | <span data-ttu-id="8d733-110">Int64</span><span class="sxs-lookup"><span data-stu-id="8d733-110">Int64</span></span>  |
| <span data-ttu-id="8d733-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="8d733-111">windowsPhone</span></span>      | <span data-ttu-id="8d733-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8d733-112">Int64</span></span>  |
| <span data-ttu-id="8d733-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="8d733-113">androidPhone</span></span>      | <span data-ttu-id="8d733-114">Int64</span><span class="sxs-lookup"><span data-stu-id="8d733-114">Int64</span></span>  |
| <span data-ttu-id="8d733-115">ios</span><span class="sxs-lookup"><span data-stu-id="8d733-115">ios</span></span>               | <span data-ttu-id="8d733-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8d733-116">Int64</span></span>  |
| <span data-ttu-id="8d733-117">Mac</span><span class="sxs-lookup"><span data-stu-id="8d733-117">mac</span></span>               | <span data-ttu-id="8d733-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8d733-118">Int64</span></span>  |
| <span data-ttu-id="8d733-119">windows</span><span class="sxs-lookup"><span data-stu-id="8d733-119">windows</span></span>           | <span data-ttu-id="8d733-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8d733-120">Int64</span></span>  |
| <span data-ttu-id="8d733-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="8d733-121">reportDate</span></span>        | <span data-ttu-id="8d733-122">日付</span><span class="sxs-lookup"><span data-stu-id="8d733-122">Date</span></span>   |
| <span data-ttu-id="8d733-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8d733-123">reportPeriod</span></span>      | <span data-ttu-id="8d733-124">String</span><span class="sxs-lookup"><span data-stu-id="8d733-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d733-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d733-125">JSON representation</span></span>

<span data-ttu-id="8d733-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d733-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
