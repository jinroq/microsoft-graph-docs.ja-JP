---
title: yammerDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: f98c8831c147a82985d1e59b5559d88e1a4824c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069969"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="2493d-103">yammerDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2493d-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2493d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2493d-104">Properties</span></span>

| <span data-ttu-id="2493d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2493d-105">Property</span></span>          | <span data-ttu-id="2493d-106">型</span><span class="sxs-lookup"><span data-stu-id="2493d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2493d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2493d-107">reportRefreshDate</span></span> | <span data-ttu-id="2493d-108">Date</span><span class="sxs-lookup"><span data-stu-id="2493d-108">Date</span></span>   |
| <span data-ttu-id="2493d-109">web</span><span class="sxs-lookup"><span data-stu-id="2493d-109">web</span></span>               | <span data-ttu-id="2493d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="2493d-110">Int32</span></span>  |
| <span data-ttu-id="2493d-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="2493d-111">windowsPhone</span></span>      | <span data-ttu-id="2493d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="2493d-112">Int32</span></span>  |
| <span data-ttu-id="2493d-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="2493d-113">androidPhone</span></span>      | <span data-ttu-id="2493d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="2493d-114">Int32</span></span>  |
| <span data-ttu-id="2493d-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="2493d-115">iPhone</span></span>            | <span data-ttu-id="2493d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="2493d-116">Int32</span></span>  |
| <span data-ttu-id="2493d-117">iPad</span><span class="sxs-lookup"><span data-stu-id="2493d-117">iPad</span></span>              | <span data-ttu-id="2493d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2493d-118">Int32</span></span>  |
| <span data-ttu-id="2493d-119">その他の</span><span class="sxs-lookup"><span data-stu-id="2493d-119">other</span></span>             | <span data-ttu-id="2493d-120">Int32</span><span class="sxs-lookup"><span data-stu-id="2493d-120">Int32</span></span>  |
| <span data-ttu-id="2493d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2493d-121">reportPeriod</span></span>      | <span data-ttu-id="2493d-122">String</span><span class="sxs-lookup"><span data-stu-id="2493d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2493d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2493d-123">JSON representation</span></span>

<span data-ttu-id="2493d-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2493d-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportPeriod": "String"
}
```
