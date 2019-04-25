---
title: yammerDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 63bd3e150e822d3c356f4409c2920e4998e53ec2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551520"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="6ea51-103">yammerDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ea51-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6ea51-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ea51-104">Properties</span></span>

| <span data-ttu-id="6ea51-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ea51-105">Property</span></span>          | <span data-ttu-id="6ea51-106">型</span><span class="sxs-lookup"><span data-stu-id="6ea51-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6ea51-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="6ea51-107">reportRefreshDate</span></span> | <span data-ttu-id="6ea51-108">Date</span><span class="sxs-lookup"><span data-stu-id="6ea51-108">Date</span></span>   |
| <span data-ttu-id="6ea51-109">web</span><span class="sxs-lookup"><span data-stu-id="6ea51-109">web</span></span>               | <span data-ttu-id="6ea51-110">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea51-110">Int32</span></span>  |
| <span data-ttu-id="6ea51-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="6ea51-111">windowsPhone</span></span>      | <span data-ttu-id="6ea51-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea51-112">Int32</span></span>  |
| <span data-ttu-id="6ea51-113">androidphone</span><span class="sxs-lookup"><span data-stu-id="6ea51-113">androidPhone</span></span>      | <span data-ttu-id="6ea51-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea51-114">Int32</span></span>  |
| <span data-ttu-id="6ea51-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="6ea51-115">iPhone</span></span>            | <span data-ttu-id="6ea51-116">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea51-116">Int32</span></span>  |
| <span data-ttu-id="6ea51-117">iPad</span><span class="sxs-lookup"><span data-stu-id="6ea51-117">iPad</span></span>              | <span data-ttu-id="6ea51-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea51-118">Int32</span></span>  |
| <span data-ttu-id="6ea51-119">も</span><span class="sxs-lookup"><span data-stu-id="6ea51-119">other</span></span>             | <span data-ttu-id="6ea51-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea51-120">Int32</span></span>  |
| <span data-ttu-id="6ea51-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="6ea51-121">reportDate</span></span>        | <span data-ttu-id="6ea51-122">Date</span><span class="sxs-lookup"><span data-stu-id="6ea51-122">Date</span></span>   |
| <span data-ttu-id="6ea51-123">reportperiod</span><span class="sxs-lookup"><span data-stu-id="6ea51-123">reportPeriod</span></span>      | <span data-ttu-id="6ea51-124">String</span><span class="sxs-lookup"><span data-stu-id="6ea51-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ea51-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ea51-125">JSON representation</span></span>

<span data-ttu-id="6ea51-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ea51-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
