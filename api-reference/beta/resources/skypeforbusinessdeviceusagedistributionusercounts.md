---
title: skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 3658bec2d99c5098b970e35240221dbf954beba6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884435"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="f56a1-103">skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f56a1-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f56a1-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f56a1-104">Properties</span></span>

| <span data-ttu-id="f56a1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f56a1-105">Property</span></span>          | <span data-ttu-id="f56a1-106">種類</span><span class="sxs-lookup"><span data-stu-id="f56a1-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f56a1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f56a1-107">reportRefreshDate</span></span> | <span data-ttu-id="f56a1-108">日付</span><span class="sxs-lookup"><span data-stu-id="f56a1-108">Date</span></span>   |
| <span data-ttu-id="f56a1-109">windows</span><span class="sxs-lookup"><span data-stu-id="f56a1-109">windows</span></span>           | <span data-ttu-id="f56a1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f56a1-110">Int64</span></span>  |
| <span data-ttu-id="f56a1-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="f56a1-111">windowsPhone</span></span>      | <span data-ttu-id="f56a1-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f56a1-112">Int64</span></span>  |
| <span data-ttu-id="f56a1-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="f56a1-113">androidPhone</span></span>      | <span data-ttu-id="f56a1-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f56a1-114">Int64</span></span>  |
| <span data-ttu-id="f56a1-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="f56a1-115">iPhone</span></span>            | <span data-ttu-id="f56a1-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f56a1-116">Int64</span></span>  |
| <span data-ttu-id="f56a1-117">iPad</span><span class="sxs-lookup"><span data-stu-id="f56a1-117">iPad</span></span>              | <span data-ttu-id="f56a1-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f56a1-118">Int64</span></span>  |
| <span data-ttu-id="f56a1-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f56a1-119">reportPeriod</span></span>      | <span data-ttu-id="f56a1-120">String</span><span class="sxs-lookup"><span data-stu-id="f56a1-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f56a1-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f56a1-121">JSON representation</span></span>

<span data-ttu-id="f56a1-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f56a1-122">The following is a JSON representation of the resource.</span></span>

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
