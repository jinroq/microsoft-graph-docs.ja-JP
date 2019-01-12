---
title: teamsDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d398782cef79cdf92bc56502f7c6cbf1bcdee99d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979286"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="8edc0-103">teamsDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8edc0-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8edc0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8edc0-104">Properties</span></span>

| <span data-ttu-id="8edc0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8edc0-105">Property</span></span>          | <span data-ttu-id="8edc0-106">種類</span><span class="sxs-lookup"><span data-stu-id="8edc0-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8edc0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8edc0-107">reportRefreshDate</span></span> | <span data-ttu-id="8edc0-108">日付</span><span class="sxs-lookup"><span data-stu-id="8edc0-108">Date</span></span>   |
| <span data-ttu-id="8edc0-109">web</span><span class="sxs-lookup"><span data-stu-id="8edc0-109">web</span></span>               | <span data-ttu-id="8edc0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="8edc0-110">Int64</span></span>  |
| <span data-ttu-id="8edc0-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="8edc0-111">windowsPhone</span></span>      | <span data-ttu-id="8edc0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8edc0-112">Int64</span></span>  |
| <span data-ttu-id="8edc0-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="8edc0-113">androidPhone</span></span>      | <span data-ttu-id="8edc0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="8edc0-114">Int64</span></span>  |
| <span data-ttu-id="8edc0-115">ios</span><span class="sxs-lookup"><span data-stu-id="8edc0-115">ios</span></span>               | <span data-ttu-id="8edc0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8edc0-116">Int64</span></span>  |
| <span data-ttu-id="8edc0-117">Mac</span><span class="sxs-lookup"><span data-stu-id="8edc0-117">mac</span></span>               | <span data-ttu-id="8edc0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8edc0-118">Int64</span></span>  |
| <span data-ttu-id="8edc0-119">windows</span><span class="sxs-lookup"><span data-stu-id="8edc0-119">windows</span></span>           | <span data-ttu-id="8edc0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8edc0-120">Int64</span></span>  |
| <span data-ttu-id="8edc0-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8edc0-121">reportPeriod</span></span>      | <span data-ttu-id="8edc0-122">String</span><span class="sxs-lookup"><span data-stu-id="8edc0-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8edc0-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8edc0-123">JSON representation</span></span>

<span data-ttu-id="8edc0-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8edc0-124">The following is a JSON representation of the resource.</span></span>

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
