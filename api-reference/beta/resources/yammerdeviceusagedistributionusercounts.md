---
title: yammerDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6dcfef0f86913ee1afe98681b71f9210216dd416
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006981"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="edc0d-103">yammerDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="edc0d-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="edc0d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="edc0d-104">Properties</span></span>

| <span data-ttu-id="edc0d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="edc0d-105">Property</span></span>          | <span data-ttu-id="edc0d-106">型</span><span class="sxs-lookup"><span data-stu-id="edc0d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="edc0d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="edc0d-107">reportRefreshDate</span></span> | <span data-ttu-id="edc0d-108">日付</span><span class="sxs-lookup"><span data-stu-id="edc0d-108">Date</span></span>   |
| <span data-ttu-id="edc0d-109">Web</span><span class="sxs-lookup"><span data-stu-id="edc0d-109">web</span></span>               | <span data-ttu-id="edc0d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="edc0d-110">Int32</span></span>  |
| <span data-ttu-id="edc0d-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="edc0d-111">windowsPhone</span></span>      | <span data-ttu-id="edc0d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="edc0d-112">Int32</span></span>  |
| <span data-ttu-id="edc0d-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="edc0d-113">androidPhone</span></span>      | <span data-ttu-id="edc0d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="edc0d-114">Int32</span></span>  |
| <span data-ttu-id="edc0d-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="edc0d-115">iPhone</span></span>            | <span data-ttu-id="edc0d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="edc0d-116">Int32</span></span>  |
| <span data-ttu-id="edc0d-117">iPad</span><span class="sxs-lookup"><span data-stu-id="edc0d-117">iPad</span></span>              | <span data-ttu-id="edc0d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="edc0d-118">Int32</span></span>  |
| <span data-ttu-id="edc0d-119">も</span><span class="sxs-lookup"><span data-stu-id="edc0d-119">other</span></span>             | <span data-ttu-id="edc0d-120">Int32</span><span class="sxs-lookup"><span data-stu-id="edc0d-120">Int32</span></span>  |
| <span data-ttu-id="edc0d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="edc0d-121">reportPeriod</span></span>      | <span data-ttu-id="edc0d-122">String</span><span class="sxs-lookup"><span data-stu-id="edc0d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="edc0d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="edc0d-123">JSON representation</span></span>

<span data-ttu-id="edc0d-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="edc0d-124">The following is a JSON representation of the resource.</span></span>

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
