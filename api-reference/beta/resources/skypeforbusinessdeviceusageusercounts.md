---
title: skypeForBusinessDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: d98590e83637e45d35f135c56f2c0b8ff7d282bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866928"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="f93a9-103">skypeForBusinessDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f93a9-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f93a9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f93a9-104">Properties</span></span>

| <span data-ttu-id="f93a9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f93a9-105">Property</span></span>          | <span data-ttu-id="f93a9-106">種類</span><span class="sxs-lookup"><span data-stu-id="f93a9-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f93a9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f93a9-107">reportRefreshDate</span></span> | <span data-ttu-id="f93a9-108">日付</span><span class="sxs-lookup"><span data-stu-id="f93a9-108">Date</span></span>   |
| <span data-ttu-id="f93a9-109">windows</span><span class="sxs-lookup"><span data-stu-id="f93a9-109">windows</span></span>           | <span data-ttu-id="f93a9-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f93a9-110">Int64</span></span>  |
| <span data-ttu-id="f93a9-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="f93a9-111">windowsPhone</span></span>      | <span data-ttu-id="f93a9-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f93a9-112">Int64</span></span>  |
| <span data-ttu-id="f93a9-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="f93a9-113">androidPhone</span></span>      | <span data-ttu-id="f93a9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f93a9-114">Int64</span></span>  |
| <span data-ttu-id="f93a9-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="f93a9-115">iPhone</span></span>            | <span data-ttu-id="f93a9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f93a9-116">Int64</span></span>  |
| <span data-ttu-id="f93a9-117">iPad</span><span class="sxs-lookup"><span data-stu-id="f93a9-117">iPad</span></span>              | <span data-ttu-id="f93a9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f93a9-118">Int64</span></span>  |
| <span data-ttu-id="f93a9-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="f93a9-119">reportDate</span></span>        | <span data-ttu-id="f93a9-120">日付</span><span class="sxs-lookup"><span data-stu-id="f93a9-120">Date</span></span>   |
| <span data-ttu-id="f93a9-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f93a9-121">reportPeriod</span></span>      | <span data-ttu-id="f93a9-122">String</span><span class="sxs-lookup"><span data-stu-id="f93a9-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f93a9-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f93a9-123">JSON representation</span></span>

<span data-ttu-id="f93a9-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f93a9-124">The following is a JSON representation of the resource.</span></span>

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
