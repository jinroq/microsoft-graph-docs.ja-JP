---
title: yammerDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6832d4c1829c6fd7ce679fe12511b694cc999b95
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963781"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="c1fde-103">yammerDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1fde-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c1fde-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1fde-104">Properties</span></span>

| <span data-ttu-id="c1fde-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1fde-105">Property</span></span>          | <span data-ttu-id="c1fde-106">型</span><span class="sxs-lookup"><span data-stu-id="c1fde-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c1fde-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c1fde-107">reportRefreshDate</span></span> | <span data-ttu-id="c1fde-108">日付</span><span class="sxs-lookup"><span data-stu-id="c1fde-108">Date</span></span>   |
| <span data-ttu-id="c1fde-109">Web</span><span class="sxs-lookup"><span data-stu-id="c1fde-109">web</span></span>               | <span data-ttu-id="c1fde-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c1fde-110">Int32</span></span>  |
| <span data-ttu-id="c1fde-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="c1fde-111">windowsPhone</span></span>      | <span data-ttu-id="c1fde-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c1fde-112">Int32</span></span>  |
| <span data-ttu-id="c1fde-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="c1fde-113">androidPhone</span></span>      | <span data-ttu-id="c1fde-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c1fde-114">Int32</span></span>  |
| <span data-ttu-id="c1fde-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="c1fde-115">iPhone</span></span>            | <span data-ttu-id="c1fde-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c1fde-116">Int32</span></span>  |
| <span data-ttu-id="c1fde-117">iPad</span><span class="sxs-lookup"><span data-stu-id="c1fde-117">iPad</span></span>              | <span data-ttu-id="c1fde-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c1fde-118">Int32</span></span>  |
| <span data-ttu-id="c1fde-119">も</span><span class="sxs-lookup"><span data-stu-id="c1fde-119">other</span></span>             | <span data-ttu-id="c1fde-120">Int32</span><span class="sxs-lookup"><span data-stu-id="c1fde-120">Int32</span></span>  |
| <span data-ttu-id="c1fde-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="c1fde-121">reportDate</span></span>        | <span data-ttu-id="c1fde-122">日付</span><span class="sxs-lookup"><span data-stu-id="c1fde-122">Date</span></span>   |
| <span data-ttu-id="c1fde-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c1fde-123">reportPeriod</span></span>      | <span data-ttu-id="c1fde-124">String</span><span class="sxs-lookup"><span data-stu-id="c1fde-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c1fde-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1fde-125">JSON representation</span></span>

<span data-ttu-id="c1fde-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c1fde-126">The following is a JSON representation of the resource.</span></span>

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
