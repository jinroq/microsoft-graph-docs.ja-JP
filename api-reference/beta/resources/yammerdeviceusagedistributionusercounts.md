---
title: yammerDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1797facecb5047badb35c0a4d876680e817cc643
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555081"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="614d4-103">yammerDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="614d4-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="614d4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="614d4-104">Properties</span></span>

| <span data-ttu-id="614d4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="614d4-105">Property</span></span>          | <span data-ttu-id="614d4-106">型</span><span class="sxs-lookup"><span data-stu-id="614d4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="614d4-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="614d4-107">reportRefreshDate</span></span> | <span data-ttu-id="614d4-108">Date</span><span class="sxs-lookup"><span data-stu-id="614d4-108">Date</span></span>   |
| <span data-ttu-id="614d4-109">web</span><span class="sxs-lookup"><span data-stu-id="614d4-109">web</span></span>               | <span data-ttu-id="614d4-110">Int32</span><span class="sxs-lookup"><span data-stu-id="614d4-110">Int32</span></span>  |
| <span data-ttu-id="614d4-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="614d4-111">windowsPhone</span></span>      | <span data-ttu-id="614d4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="614d4-112">Int32</span></span>  |
| <span data-ttu-id="614d4-113">androidphone</span><span class="sxs-lookup"><span data-stu-id="614d4-113">androidPhone</span></span>      | <span data-ttu-id="614d4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="614d4-114">Int32</span></span>  |
| <span data-ttu-id="614d4-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="614d4-115">iPhone</span></span>            | <span data-ttu-id="614d4-116">Int32</span><span class="sxs-lookup"><span data-stu-id="614d4-116">Int32</span></span>  |
| <span data-ttu-id="614d4-117">iPad</span><span class="sxs-lookup"><span data-stu-id="614d4-117">iPad</span></span>              | <span data-ttu-id="614d4-118">Int32</span><span class="sxs-lookup"><span data-stu-id="614d4-118">Int32</span></span>  |
| <span data-ttu-id="614d4-119">も</span><span class="sxs-lookup"><span data-stu-id="614d4-119">other</span></span>             | <span data-ttu-id="614d4-120">Int32</span><span class="sxs-lookup"><span data-stu-id="614d4-120">Int32</span></span>  |
| <span data-ttu-id="614d4-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="614d4-121">reportPeriod</span></span>      | <span data-ttu-id="614d4-122">String</span><span class="sxs-lookup"><span data-stu-id="614d4-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="614d4-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="614d4-123">JSON representation</span></span>

<span data-ttu-id="614d4-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="614d4-124">The following is a JSON representation of the resource.</span></span>

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
