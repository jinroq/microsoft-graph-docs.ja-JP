---
title: yammerDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: ad8707d33c4200ea6729205819871d890929f001
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889034"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="5d6fc-103">yammerDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d6fc-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5d6fc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d6fc-104">Properties</span></span>

| <span data-ttu-id="5d6fc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d6fc-105">Property</span></span>          | <span data-ttu-id="5d6fc-106">種類</span><span class="sxs-lookup"><span data-stu-id="5d6fc-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5d6fc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5d6fc-107">reportRefreshDate</span></span> | <span data-ttu-id="5d6fc-108">日付</span><span class="sxs-lookup"><span data-stu-id="5d6fc-108">Date</span></span>   |
| <span data-ttu-id="5d6fc-109">web</span><span class="sxs-lookup"><span data-stu-id="5d6fc-109">web</span></span>               | <span data-ttu-id="5d6fc-110">Int32</span><span class="sxs-lookup"><span data-stu-id="5d6fc-110">Int32</span></span>  |
| <span data-ttu-id="5d6fc-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5d6fc-111">windowsPhone</span></span>      | <span data-ttu-id="5d6fc-112">Int32</span><span class="sxs-lookup"><span data-stu-id="5d6fc-112">Int32</span></span>  |
| <span data-ttu-id="5d6fc-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="5d6fc-113">androidPhone</span></span>      | <span data-ttu-id="5d6fc-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5d6fc-114">Int32</span></span>  |
| <span data-ttu-id="5d6fc-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="5d6fc-115">iPhone</span></span>            | <span data-ttu-id="5d6fc-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5d6fc-116">Int32</span></span>  |
| <span data-ttu-id="5d6fc-117">iPad</span><span class="sxs-lookup"><span data-stu-id="5d6fc-117">iPad</span></span>              | <span data-ttu-id="5d6fc-118">Int32</span><span class="sxs-lookup"><span data-stu-id="5d6fc-118">Int32</span></span>  |
| <span data-ttu-id="5d6fc-119">その他の</span><span class="sxs-lookup"><span data-stu-id="5d6fc-119">other</span></span>             | <span data-ttu-id="5d6fc-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5d6fc-120">Int32</span></span>  |
| <span data-ttu-id="5d6fc-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5d6fc-121">reportPeriod</span></span>      | <span data-ttu-id="5d6fc-122">String</span><span class="sxs-lookup"><span data-stu-id="5d6fc-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5d6fc-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d6fc-123">JSON representation</span></span>

<span data-ttu-id="5d6fc-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5d6fc-124">The following is a JSON representation of the resource.</span></span>

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
