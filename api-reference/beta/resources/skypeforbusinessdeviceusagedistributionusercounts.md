---
title: skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b5c90db3ec241017781d52bbb623d728a7959445
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964943"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="61597-103">skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61597-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="61597-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61597-104">Properties</span></span>

| <span data-ttu-id="61597-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61597-105">Property</span></span>          | <span data-ttu-id="61597-106">型</span><span class="sxs-lookup"><span data-stu-id="61597-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="61597-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="61597-107">reportRefreshDate</span></span> | <span data-ttu-id="61597-108">日付</span><span class="sxs-lookup"><span data-stu-id="61597-108">Date</span></span>   |
| <span data-ttu-id="61597-109">ws</span><span class="sxs-lookup"><span data-stu-id="61597-109">windows</span></span>           | <span data-ttu-id="61597-110">Int64</span><span class="sxs-lookup"><span data-stu-id="61597-110">Int64</span></span>  |
| <span data-ttu-id="61597-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="61597-111">windowsPhone</span></span>      | <span data-ttu-id="61597-112">Int64</span><span class="sxs-lookup"><span data-stu-id="61597-112">Int64</span></span>  |
| <span data-ttu-id="61597-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="61597-113">androidPhone</span></span>      | <span data-ttu-id="61597-114">Int64</span><span class="sxs-lookup"><span data-stu-id="61597-114">Int64</span></span>  |
| <span data-ttu-id="61597-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="61597-115">iPhone</span></span>            | <span data-ttu-id="61597-116">Int64</span><span class="sxs-lookup"><span data-stu-id="61597-116">Int64</span></span>  |
| <span data-ttu-id="61597-117">iPad</span><span class="sxs-lookup"><span data-stu-id="61597-117">iPad</span></span>              | <span data-ttu-id="61597-118">Int64</span><span class="sxs-lookup"><span data-stu-id="61597-118">Int64</span></span>  |
| <span data-ttu-id="61597-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="61597-119">reportPeriod</span></span>      | <span data-ttu-id="61597-120">String</span><span class="sxs-lookup"><span data-stu-id="61597-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61597-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61597-121">JSON representation</span></span>

<span data-ttu-id="61597-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61597-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportPeriod": "String"
}
```
