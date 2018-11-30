---
title: teamsDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: b039320e389e1a61832089991b2368b27e51c475
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066736"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="f470a-103">teamsDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f470a-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f470a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f470a-104">Properties</span></span>

| <span data-ttu-id="f470a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f470a-105">Property</span></span>          | <span data-ttu-id="f470a-106">型</span><span class="sxs-lookup"><span data-stu-id="f470a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f470a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f470a-107">reportRefreshDate</span></span> | <span data-ttu-id="f470a-108">Date</span><span class="sxs-lookup"><span data-stu-id="f470a-108">Date</span></span>   |
| <span data-ttu-id="f470a-109">web</span><span class="sxs-lookup"><span data-stu-id="f470a-109">web</span></span>               | <span data-ttu-id="f470a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f470a-110">Int64</span></span>  |
| <span data-ttu-id="f470a-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="f470a-111">windowsPhone</span></span>      | <span data-ttu-id="f470a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f470a-112">Int64</span></span>  |
| <span data-ttu-id="f470a-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="f470a-113">androidPhone</span></span>      | <span data-ttu-id="f470a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f470a-114">Int64</span></span>  |
| <span data-ttu-id="f470a-115">ios</span><span class="sxs-lookup"><span data-stu-id="f470a-115">ios</span></span>               | <span data-ttu-id="f470a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f470a-116">Int64</span></span>  |
| <span data-ttu-id="f470a-117">Mac</span><span class="sxs-lookup"><span data-stu-id="f470a-117">mac</span></span>               | <span data-ttu-id="f470a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f470a-118">Int64</span></span>  |
| <span data-ttu-id="f470a-119">windows</span><span class="sxs-lookup"><span data-stu-id="f470a-119">windows</span></span>           | <span data-ttu-id="f470a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f470a-120">Int64</span></span>  |
| <span data-ttu-id="f470a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f470a-121">reportPeriod</span></span>      | <span data-ttu-id="f470a-122">String</span><span class="sxs-lookup"><span data-stu-id="f470a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f470a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f470a-123">JSON representation</span></span>

<span data-ttu-id="f470a-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f470a-124">The following is a JSON representation of the resource.</span></span>

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
