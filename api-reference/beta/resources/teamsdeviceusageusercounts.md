---
title: teamsDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 9640af67efc18f0a70c636673169e884ce82d971
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073765"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="5ea1c-103">teamsDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ea1c-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5ea1c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ea1c-104">Properties</span></span>

| <span data-ttu-id="5ea1c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ea1c-105">Property</span></span>          | <span data-ttu-id="5ea1c-106">型</span><span class="sxs-lookup"><span data-stu-id="5ea1c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5ea1c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5ea1c-107">reportRefreshDate</span></span> | <span data-ttu-id="5ea1c-108">Date</span><span class="sxs-lookup"><span data-stu-id="5ea1c-108">Date</span></span>   |
| <span data-ttu-id="5ea1c-109">web</span><span class="sxs-lookup"><span data-stu-id="5ea1c-109">web</span></span>               | <span data-ttu-id="5ea1c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea1c-110">Int64</span></span>  |
| <span data-ttu-id="5ea1c-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5ea1c-111">windowsPhone</span></span>      | <span data-ttu-id="5ea1c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea1c-112">Int64</span></span>  |
| <span data-ttu-id="5ea1c-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="5ea1c-113">androidPhone</span></span>      | <span data-ttu-id="5ea1c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea1c-114">Int64</span></span>  |
| <span data-ttu-id="5ea1c-115">ios</span><span class="sxs-lookup"><span data-stu-id="5ea1c-115">ios</span></span>               | <span data-ttu-id="5ea1c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea1c-116">Int64</span></span>  |
| <span data-ttu-id="5ea1c-117">Mac</span><span class="sxs-lookup"><span data-stu-id="5ea1c-117">mac</span></span>               | <span data-ttu-id="5ea1c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea1c-118">Int64</span></span>  |
| <span data-ttu-id="5ea1c-119">windows</span><span class="sxs-lookup"><span data-stu-id="5ea1c-119">windows</span></span>           | <span data-ttu-id="5ea1c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea1c-120">Int64</span></span>  |
| <span data-ttu-id="5ea1c-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="5ea1c-121">reportDate</span></span>        | <span data-ttu-id="5ea1c-122">Date</span><span class="sxs-lookup"><span data-stu-id="5ea1c-122">Date</span></span>   |
| <span data-ttu-id="5ea1c-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5ea1c-123">reportPeriod</span></span>      | <span data-ttu-id="5ea1c-124">String</span><span class="sxs-lookup"><span data-stu-id="5ea1c-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ea1c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ea1c-125">JSON representation</span></span>

<span data-ttu-id="5ea1c-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ea1c-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
