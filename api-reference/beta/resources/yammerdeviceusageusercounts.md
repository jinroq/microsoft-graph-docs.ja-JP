---
title: yammerDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 63bd3e150e822d3c356f4409c2920e4998e53ec2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577327"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="a29de-103">yammerDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a29de-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a29de-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a29de-104">Properties</span></span>

| <span data-ttu-id="a29de-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a29de-105">Property</span></span>          | <span data-ttu-id="a29de-106">型</span><span class="sxs-lookup"><span data-stu-id="a29de-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a29de-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a29de-107">reportRefreshDate</span></span> | <span data-ttu-id="a29de-108">日付</span><span class="sxs-lookup"><span data-stu-id="a29de-108">Date</span></span>   |
| <span data-ttu-id="a29de-109">web</span><span class="sxs-lookup"><span data-stu-id="a29de-109">web</span></span>               | <span data-ttu-id="a29de-110">Int32</span><span class="sxs-lookup"><span data-stu-id="a29de-110">Int32</span></span>  |
| <span data-ttu-id="a29de-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="a29de-111">windowsPhone</span></span>      | <span data-ttu-id="a29de-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a29de-112">Int32</span></span>  |
| <span data-ttu-id="a29de-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="a29de-113">androidPhone</span></span>      | <span data-ttu-id="a29de-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a29de-114">Int32</span></span>  |
| <span data-ttu-id="a29de-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="a29de-115">iPhone</span></span>            | <span data-ttu-id="a29de-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a29de-116">Int32</span></span>  |
| <span data-ttu-id="a29de-117">iPad</span><span class="sxs-lookup"><span data-stu-id="a29de-117">iPad</span></span>              | <span data-ttu-id="a29de-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a29de-118">Int32</span></span>  |
| <span data-ttu-id="a29de-119">その他の</span><span class="sxs-lookup"><span data-stu-id="a29de-119">other</span></span>             | <span data-ttu-id="a29de-120">Int32</span><span class="sxs-lookup"><span data-stu-id="a29de-120">Int32</span></span>  |
| <span data-ttu-id="a29de-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="a29de-121">reportDate</span></span>        | <span data-ttu-id="a29de-122">日付</span><span class="sxs-lookup"><span data-stu-id="a29de-122">Date</span></span>   |
| <span data-ttu-id="a29de-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a29de-123">reportPeriod</span></span>      | <span data-ttu-id="a29de-124">String</span><span class="sxs-lookup"><span data-stu-id="a29de-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a29de-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a29de-125">JSON representation</span></span>

<span data-ttu-id="a29de-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a29de-126">The following is a JSON representation of the resource.</span></span>

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
