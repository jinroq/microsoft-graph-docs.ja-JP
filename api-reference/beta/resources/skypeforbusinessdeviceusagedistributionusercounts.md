---
title: skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 1534051455d805cf3bc9fabbb301ffde5be85ad9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074497"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="25345-103">skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25345-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="25345-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25345-104">Properties</span></span>

| <span data-ttu-id="25345-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25345-105">Property</span></span>          | <span data-ttu-id="25345-106">型</span><span class="sxs-lookup"><span data-stu-id="25345-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="25345-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="25345-107">reportRefreshDate</span></span> | <span data-ttu-id="25345-108">Date</span><span class="sxs-lookup"><span data-stu-id="25345-108">Date</span></span>   |
| <span data-ttu-id="25345-109">windows</span><span class="sxs-lookup"><span data-stu-id="25345-109">windows</span></span>           | <span data-ttu-id="25345-110">Int64</span><span class="sxs-lookup"><span data-stu-id="25345-110">Int64</span></span>  |
| <span data-ttu-id="25345-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="25345-111">windowsPhone</span></span>      | <span data-ttu-id="25345-112">Int64</span><span class="sxs-lookup"><span data-stu-id="25345-112">Int64</span></span>  |
| <span data-ttu-id="25345-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="25345-113">androidPhone</span></span>      | <span data-ttu-id="25345-114">Int64</span><span class="sxs-lookup"><span data-stu-id="25345-114">Int64</span></span>  |
| <span data-ttu-id="25345-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="25345-115">iPhone</span></span>            | <span data-ttu-id="25345-116">Int64</span><span class="sxs-lookup"><span data-stu-id="25345-116">Int64</span></span>  |
| <span data-ttu-id="25345-117">iPad</span><span class="sxs-lookup"><span data-stu-id="25345-117">iPad</span></span>              | <span data-ttu-id="25345-118">Int64</span><span class="sxs-lookup"><span data-stu-id="25345-118">Int64</span></span>  |
| <span data-ttu-id="25345-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="25345-119">reportPeriod</span></span>      | <span data-ttu-id="25345-120">String</span><span class="sxs-lookup"><span data-stu-id="25345-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="25345-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25345-121">JSON representation</span></span>

<span data-ttu-id="25345-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="25345-122">The following is a JSON representation of the resource.</span></span>

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
