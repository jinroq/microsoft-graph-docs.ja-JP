---
title: teamsDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1842d2edc9e527d577b6a44e61443018f8309c17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007614"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="522f4-103">teamsDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="522f4-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="522f4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="522f4-104">Properties</span></span>

| <span data-ttu-id="522f4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="522f4-105">Property</span></span>          | <span data-ttu-id="522f4-106">型</span><span class="sxs-lookup"><span data-stu-id="522f4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="522f4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="522f4-107">reportRefreshDate</span></span> | <span data-ttu-id="522f4-108">日付</span><span class="sxs-lookup"><span data-stu-id="522f4-108">Date</span></span>   |
| <span data-ttu-id="522f4-109">Web</span><span class="sxs-lookup"><span data-stu-id="522f4-109">web</span></span>               | <span data-ttu-id="522f4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="522f4-110">Int64</span></span>  |
| <span data-ttu-id="522f4-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="522f4-111">windowsPhone</span></span>      | <span data-ttu-id="522f4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="522f4-112">Int64</span></span>  |
| <span data-ttu-id="522f4-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="522f4-113">androidPhone</span></span>      | <span data-ttu-id="522f4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="522f4-114">Int64</span></span>  |
| <span data-ttu-id="522f4-115">ios</span><span class="sxs-lookup"><span data-stu-id="522f4-115">ios</span></span>               | <span data-ttu-id="522f4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="522f4-116">Int64</span></span>  |
| <span data-ttu-id="522f4-117">Mac</span><span class="sxs-lookup"><span data-stu-id="522f4-117">mac</span></span>               | <span data-ttu-id="522f4-118">Int64</span><span class="sxs-lookup"><span data-stu-id="522f4-118">Int64</span></span>  |
| <span data-ttu-id="522f4-119">ws</span><span class="sxs-lookup"><span data-stu-id="522f4-119">windows</span></span>           | <span data-ttu-id="522f4-120">Int64</span><span class="sxs-lookup"><span data-stu-id="522f4-120">Int64</span></span>  |
| <span data-ttu-id="522f4-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="522f4-121">reportPeriod</span></span>      | <span data-ttu-id="522f4-122">String</span><span class="sxs-lookup"><span data-stu-id="522f4-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="522f4-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="522f4-123">JSON representation</span></span>

<span data-ttu-id="522f4-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="522f4-124">The following is a JSON representation of the resource.</span></span>

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
