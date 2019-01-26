---
title: yammerDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1797facecb5047badb35c0a4d876680e817cc643
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576802"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="fbcc5-103">yammerDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbcc5-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fbcc5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbcc5-104">Properties</span></span>

| <span data-ttu-id="fbcc5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbcc5-105">Property</span></span>          | <span data-ttu-id="fbcc5-106">型</span><span class="sxs-lookup"><span data-stu-id="fbcc5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fbcc5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fbcc5-107">reportRefreshDate</span></span> | <span data-ttu-id="fbcc5-108">日付</span><span class="sxs-lookup"><span data-stu-id="fbcc5-108">Date</span></span>   |
| <span data-ttu-id="fbcc5-109">web</span><span class="sxs-lookup"><span data-stu-id="fbcc5-109">web</span></span>               | <span data-ttu-id="fbcc5-110">Int32</span><span class="sxs-lookup"><span data-stu-id="fbcc5-110">Int32</span></span>  |
| <span data-ttu-id="fbcc5-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="fbcc5-111">windowsPhone</span></span>      | <span data-ttu-id="fbcc5-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fbcc5-112">Int32</span></span>  |
| <span data-ttu-id="fbcc5-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="fbcc5-113">androidPhone</span></span>      | <span data-ttu-id="fbcc5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="fbcc5-114">Int32</span></span>  |
| <span data-ttu-id="fbcc5-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="fbcc5-115">iPhone</span></span>            | <span data-ttu-id="fbcc5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fbcc5-116">Int32</span></span>  |
| <span data-ttu-id="fbcc5-117">iPad</span><span class="sxs-lookup"><span data-stu-id="fbcc5-117">iPad</span></span>              | <span data-ttu-id="fbcc5-118">Int32</span><span class="sxs-lookup"><span data-stu-id="fbcc5-118">Int32</span></span>  |
| <span data-ttu-id="fbcc5-119">その他の</span><span class="sxs-lookup"><span data-stu-id="fbcc5-119">other</span></span>             | <span data-ttu-id="fbcc5-120">Int32</span><span class="sxs-lookup"><span data-stu-id="fbcc5-120">Int32</span></span>  |
| <span data-ttu-id="fbcc5-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fbcc5-121">reportPeriod</span></span>      | <span data-ttu-id="fbcc5-122">String</span><span class="sxs-lookup"><span data-stu-id="fbcc5-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fbcc5-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbcc5-123">JSON representation</span></span>

<span data-ttu-id="fbcc5-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fbcc5-124">The following is a JSON representation of the resource.</span></span>

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
