---
title: yammerDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 7faec83d113da3f412c913177a717fdc69504310
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069971"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="b8e24-103">yammerDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8e24-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b8e24-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8e24-104">Properties</span></span>

| <span data-ttu-id="b8e24-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8e24-105">Property</span></span>          | <span data-ttu-id="b8e24-106">型</span><span class="sxs-lookup"><span data-stu-id="b8e24-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b8e24-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b8e24-107">reportRefreshDate</span></span> | <span data-ttu-id="b8e24-108">Date</span><span class="sxs-lookup"><span data-stu-id="b8e24-108">Date</span></span>   |
| <span data-ttu-id="b8e24-109">web</span><span class="sxs-lookup"><span data-stu-id="b8e24-109">web</span></span>               | <span data-ttu-id="b8e24-110">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e24-110">Int32</span></span>  |
| <span data-ttu-id="b8e24-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="b8e24-111">windowsPhone</span></span>      | <span data-ttu-id="b8e24-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e24-112">Int32</span></span>  |
| <span data-ttu-id="b8e24-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="b8e24-113">androidPhone</span></span>      | <span data-ttu-id="b8e24-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e24-114">Int32</span></span>  |
| <span data-ttu-id="b8e24-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="b8e24-115">iPhone</span></span>            | <span data-ttu-id="b8e24-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e24-116">Int32</span></span>  |
| <span data-ttu-id="b8e24-117">iPad</span><span class="sxs-lookup"><span data-stu-id="b8e24-117">iPad</span></span>              | <span data-ttu-id="b8e24-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e24-118">Int32</span></span>  |
| <span data-ttu-id="b8e24-119">その他の</span><span class="sxs-lookup"><span data-stu-id="b8e24-119">other</span></span>             | <span data-ttu-id="b8e24-120">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e24-120">Int32</span></span>  |
| <span data-ttu-id="b8e24-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="b8e24-121">reportDate</span></span>        | <span data-ttu-id="b8e24-122">Date</span><span class="sxs-lookup"><span data-stu-id="b8e24-122">Date</span></span>   |
| <span data-ttu-id="b8e24-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b8e24-123">reportPeriod</span></span>      | <span data-ttu-id="b8e24-124">String</span><span class="sxs-lookup"><span data-stu-id="b8e24-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b8e24-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8e24-125">JSON representation</span></span>

<span data-ttu-id="b8e24-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8e24-126">The following is a JSON representation of the resource.</span></span>

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
