---
title: skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 3658bec2d99c5098b970e35240221dbf954beba6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581262"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="c5cf4-103">skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5cf4-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c5cf4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5cf4-104">Properties</span></span>

| <span data-ttu-id="c5cf4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5cf4-105">Property</span></span>          | <span data-ttu-id="c5cf4-106">型</span><span class="sxs-lookup"><span data-stu-id="c5cf4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c5cf4-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="c5cf4-107">reportRefreshDate</span></span> | <span data-ttu-id="c5cf4-108">Date</span><span class="sxs-lookup"><span data-stu-id="c5cf4-108">Date</span></span>   |
| <span data-ttu-id="c5cf4-109">ws</span><span class="sxs-lookup"><span data-stu-id="c5cf4-109">windows</span></span>           | <span data-ttu-id="c5cf4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c5cf4-110">Int64</span></span>  |
| <span data-ttu-id="c5cf4-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="c5cf4-111">windowsPhone</span></span>      | <span data-ttu-id="c5cf4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c5cf4-112">Int64</span></span>  |
| <span data-ttu-id="c5cf4-113">androidphone</span><span class="sxs-lookup"><span data-stu-id="c5cf4-113">androidPhone</span></span>      | <span data-ttu-id="c5cf4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c5cf4-114">Int64</span></span>  |
| <span data-ttu-id="c5cf4-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="c5cf4-115">iPhone</span></span>            | <span data-ttu-id="c5cf4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c5cf4-116">Int64</span></span>  |
| <span data-ttu-id="c5cf4-117">iPad</span><span class="sxs-lookup"><span data-stu-id="c5cf4-117">iPad</span></span>              | <span data-ttu-id="c5cf4-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c5cf4-118">Int64</span></span>  |
| <span data-ttu-id="c5cf4-119">reportperiod</span><span class="sxs-lookup"><span data-stu-id="c5cf4-119">reportPeriod</span></span>      | <span data-ttu-id="c5cf4-120">String</span><span class="sxs-lookup"><span data-stu-id="c5cf4-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5cf4-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5cf4-121">JSON representation</span></span>

<span data-ttu-id="c5cf4-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5cf4-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportPeriod": "String"
}
```
