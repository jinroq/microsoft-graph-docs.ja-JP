---
title: yammerDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: d3fbfaeac312096393c3c5a2d406327551cbaa33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867950"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="80493-103">yammerDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80493-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="80493-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80493-104">Properties</span></span>

| <span data-ttu-id="80493-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80493-105">Property</span></span>          | <span data-ttu-id="80493-106">種類</span><span class="sxs-lookup"><span data-stu-id="80493-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="80493-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="80493-107">reportRefreshDate</span></span> | <span data-ttu-id="80493-108">日付</span><span class="sxs-lookup"><span data-stu-id="80493-108">Date</span></span>   |
| <span data-ttu-id="80493-109">web</span><span class="sxs-lookup"><span data-stu-id="80493-109">web</span></span>               | <span data-ttu-id="80493-110">Int32</span><span class="sxs-lookup"><span data-stu-id="80493-110">Int32</span></span>  |
| <span data-ttu-id="80493-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="80493-111">windowsPhone</span></span>      | <span data-ttu-id="80493-112">Int32</span><span class="sxs-lookup"><span data-stu-id="80493-112">Int32</span></span>  |
| <span data-ttu-id="80493-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="80493-113">androidPhone</span></span>      | <span data-ttu-id="80493-114">Int32</span><span class="sxs-lookup"><span data-stu-id="80493-114">Int32</span></span>  |
| <span data-ttu-id="80493-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="80493-115">iPhone</span></span>            | <span data-ttu-id="80493-116">Int32</span><span class="sxs-lookup"><span data-stu-id="80493-116">Int32</span></span>  |
| <span data-ttu-id="80493-117">iPad</span><span class="sxs-lookup"><span data-stu-id="80493-117">iPad</span></span>              | <span data-ttu-id="80493-118">Int32</span><span class="sxs-lookup"><span data-stu-id="80493-118">Int32</span></span>  |
| <span data-ttu-id="80493-119">その他の</span><span class="sxs-lookup"><span data-stu-id="80493-119">other</span></span>             | <span data-ttu-id="80493-120">Int32</span><span class="sxs-lookup"><span data-stu-id="80493-120">Int32</span></span>  |
| <span data-ttu-id="80493-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="80493-121">reportDate</span></span>        | <span data-ttu-id="80493-122">日付</span><span class="sxs-lookup"><span data-stu-id="80493-122">Date</span></span>   |
| <span data-ttu-id="80493-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="80493-123">reportPeriod</span></span>      | <span data-ttu-id="80493-124">String</span><span class="sxs-lookup"><span data-stu-id="80493-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="80493-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80493-125">JSON representation</span></span>

<span data-ttu-id="80493-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="80493-126">The following is a JSON representation of the resource.</span></span>

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
