---
title: teamsdevice使い方 user計数リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 671dfada02b9c16d3392d0a97023b82020fd1218
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553597"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="2ad8c-103">teamsdevice使い方 user計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ad8c-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2ad8c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ad8c-104">Properties</span></span>

| <span data-ttu-id="2ad8c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ad8c-105">Property</span></span>          | <span data-ttu-id="2ad8c-106">型</span><span class="sxs-lookup"><span data-stu-id="2ad8c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2ad8c-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="2ad8c-107">reportRefreshDate</span></span> | <span data-ttu-id="2ad8c-108">Date</span><span class="sxs-lookup"><span data-stu-id="2ad8c-108">Date</span></span>   |
| <span data-ttu-id="2ad8c-109">web</span><span class="sxs-lookup"><span data-stu-id="2ad8c-109">web</span></span>               | <span data-ttu-id="2ad8c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad8c-110">Int64</span></span>  |
| <span data-ttu-id="2ad8c-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="2ad8c-111">windowsPhone</span></span>      | <span data-ttu-id="2ad8c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad8c-112">Int64</span></span>  |
| <span data-ttu-id="2ad8c-113">androidphone</span><span class="sxs-lookup"><span data-stu-id="2ad8c-113">androidPhone</span></span>      | <span data-ttu-id="2ad8c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad8c-114">Int64</span></span>  |
| <span data-ttu-id="2ad8c-115">ios</span><span class="sxs-lookup"><span data-stu-id="2ad8c-115">ios</span></span>               | <span data-ttu-id="2ad8c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad8c-116">Int64</span></span>  |
| <span data-ttu-id="2ad8c-117">Mac</span><span class="sxs-lookup"><span data-stu-id="2ad8c-117">mac</span></span>               | <span data-ttu-id="2ad8c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad8c-118">Int64</span></span>  |
| <span data-ttu-id="2ad8c-119">ws</span><span class="sxs-lookup"><span data-stu-id="2ad8c-119">windows</span></span>           | <span data-ttu-id="2ad8c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad8c-120">Int64</span></span>  |
| <span data-ttu-id="2ad8c-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="2ad8c-121">reportDate</span></span>        | <span data-ttu-id="2ad8c-122">Date</span><span class="sxs-lookup"><span data-stu-id="2ad8c-122">Date</span></span>   |
| <span data-ttu-id="2ad8c-123">reportperiod</span><span class="sxs-lookup"><span data-stu-id="2ad8c-123">reportPeriod</span></span>      | <span data-ttu-id="2ad8c-124">String</span><span class="sxs-lookup"><span data-stu-id="2ad8c-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2ad8c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ad8c-125">JSON representation</span></span>

<span data-ttu-id="2ad8c-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2ad8c-126">The following is a JSON representation of the resource.</span></span>

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
