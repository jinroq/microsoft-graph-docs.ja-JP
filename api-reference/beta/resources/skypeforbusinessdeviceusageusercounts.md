---
title: skypeForBusinessDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 3ae63d942ef21152e54f3bf5234d1b9d8df9649b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068115"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="7a52f-103">skypeForBusinessDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a52f-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7a52f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a52f-104">Properties</span></span>

| <span data-ttu-id="7a52f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a52f-105">Property</span></span>          | <span data-ttu-id="7a52f-106">型</span><span class="sxs-lookup"><span data-stu-id="7a52f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7a52f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7a52f-107">reportRefreshDate</span></span> | <span data-ttu-id="7a52f-108">Date</span><span class="sxs-lookup"><span data-stu-id="7a52f-108">Date</span></span>   |
| <span data-ttu-id="7a52f-109">windows</span><span class="sxs-lookup"><span data-stu-id="7a52f-109">windows</span></span>           | <span data-ttu-id="7a52f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7a52f-110">Int64</span></span>  |
| <span data-ttu-id="7a52f-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="7a52f-111">windowsPhone</span></span>      | <span data-ttu-id="7a52f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7a52f-112">Int64</span></span>  |
| <span data-ttu-id="7a52f-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="7a52f-113">androidPhone</span></span>      | <span data-ttu-id="7a52f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7a52f-114">Int64</span></span>  |
| <span data-ttu-id="7a52f-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="7a52f-115">iPhone</span></span>            | <span data-ttu-id="7a52f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7a52f-116">Int64</span></span>  |
| <span data-ttu-id="7a52f-117">iPad</span><span class="sxs-lookup"><span data-stu-id="7a52f-117">iPad</span></span>              | <span data-ttu-id="7a52f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7a52f-118">Int64</span></span>  |
| <span data-ttu-id="7a52f-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="7a52f-119">reportDate</span></span>        | <span data-ttu-id="7a52f-120">Date</span><span class="sxs-lookup"><span data-stu-id="7a52f-120">Date</span></span>   |
| <span data-ttu-id="7a52f-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7a52f-121">reportPeriod</span></span>      | <span data-ttu-id="7a52f-122">String</span><span class="sxs-lookup"><span data-stu-id="7a52f-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a52f-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a52f-123">JSON representation</span></span>

<span data-ttu-id="7a52f-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7a52f-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
