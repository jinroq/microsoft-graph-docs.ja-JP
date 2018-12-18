---
title: teamsDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
ms.openlocfilehash: 01b9f67f30a7b2f13aac65cbcd4795792ee0aaa0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345851"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="5134d-103">teamsDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5134d-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5134d-104">Properties</span><span class="sxs-lookup"><span data-stu-id="5134d-104">Properties</span></span>

| <span data-ttu-id="5134d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5134d-105">Property</span></span>          | <span data-ttu-id="5134d-106">種類</span><span class="sxs-lookup"><span data-stu-id="5134d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5134d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5134d-107">reportRefreshDate</span></span> | <span data-ttu-id="5134d-108">日付</span><span class="sxs-lookup"><span data-stu-id="5134d-108">Date</span></span>   |
| <span data-ttu-id="5134d-109">web</span><span class="sxs-lookup"><span data-stu-id="5134d-109">web</span></span>               | <span data-ttu-id="5134d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5134d-110">Int64</span></span>  |
| <span data-ttu-id="5134d-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5134d-111">windowsPhone</span></span>      | <span data-ttu-id="5134d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5134d-112">Int64</span></span>  |
| <span data-ttu-id="5134d-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="5134d-113">androidPhone</span></span>      | <span data-ttu-id="5134d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5134d-114">Int64</span></span>  |
| <span data-ttu-id="5134d-115">ios</span><span class="sxs-lookup"><span data-stu-id="5134d-115">ios</span></span>               | <span data-ttu-id="5134d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5134d-116">Int64</span></span>  |
| <span data-ttu-id="5134d-117">Mac</span><span class="sxs-lookup"><span data-stu-id="5134d-117">mac</span></span>               | <span data-ttu-id="5134d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5134d-118">Int64</span></span>  |
| <span data-ttu-id="5134d-119">windows</span><span class="sxs-lookup"><span data-stu-id="5134d-119">windows</span></span>           | <span data-ttu-id="5134d-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5134d-120">Int64</span></span>  |
| <span data-ttu-id="5134d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5134d-121">reportPeriod</span></span>      | <span data-ttu-id="5134d-122">String</span><span class="sxs-lookup"><span data-stu-id="5134d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5134d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5134d-123">JSON representation</span></span>

<span data-ttu-id="5134d-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5134d-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```
