---
title: yammerDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 937691487046e2e77cc26b2c1f1a154966e1681b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936348"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="8ae0b-103">yammerDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ae0b-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8ae0b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ae0b-104">Properties</span></span>

| <span data-ttu-id="8ae0b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ae0b-105">Property</span></span>          | <span data-ttu-id="8ae0b-106">種類</span><span class="sxs-lookup"><span data-stu-id="8ae0b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8ae0b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8ae0b-107">reportRefreshDate</span></span> | <span data-ttu-id="8ae0b-108">日付</span><span class="sxs-lookup"><span data-stu-id="8ae0b-108">Date</span></span>   |
| <span data-ttu-id="8ae0b-109">web</span><span class="sxs-lookup"><span data-stu-id="8ae0b-109">web</span></span>               | <span data-ttu-id="8ae0b-110">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae0b-110">Int32</span></span>  |
| <span data-ttu-id="8ae0b-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="8ae0b-111">windowsPhone</span></span>      | <span data-ttu-id="8ae0b-112">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae0b-112">Int32</span></span>  |
| <span data-ttu-id="8ae0b-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="8ae0b-113">androidPhone</span></span>      | <span data-ttu-id="8ae0b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae0b-114">Int32</span></span>  |
| <span data-ttu-id="8ae0b-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="8ae0b-115">iPhone</span></span>            | <span data-ttu-id="8ae0b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae0b-116">Int32</span></span>  |
| <span data-ttu-id="8ae0b-117">iPad</span><span class="sxs-lookup"><span data-stu-id="8ae0b-117">iPad</span></span>              | <span data-ttu-id="8ae0b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae0b-118">Int32</span></span>  |
| <span data-ttu-id="8ae0b-119">その他の</span><span class="sxs-lookup"><span data-stu-id="8ae0b-119">other</span></span>             | <span data-ttu-id="8ae0b-120">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae0b-120">Int32</span></span>  |
| <span data-ttu-id="8ae0b-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8ae0b-121">reportPeriod</span></span>      | <span data-ttu-id="8ae0b-122">String</span><span class="sxs-lookup"><span data-stu-id="8ae0b-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8ae0b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ae0b-123">JSON representation</span></span>

<span data-ttu-id="8ae0b-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ae0b-124">The following is a JSON representation of the resource.</span></span>

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
