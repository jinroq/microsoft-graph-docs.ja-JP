---
title: Skypeforbusinessdevice使い方 User計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 04f14ce10a93d8bff870613e644b80f554d26573
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008209"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="8bb90-103">Skypeforbusinessdevice使い方 User計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8bb90-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8bb90-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bb90-104">Properties</span></span>

| <span data-ttu-id="8bb90-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bb90-105">Property</span></span>          | <span data-ttu-id="8bb90-106">型</span><span class="sxs-lookup"><span data-stu-id="8bb90-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8bb90-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8bb90-107">reportRefreshDate</span></span> | <span data-ttu-id="8bb90-108">日付</span><span class="sxs-lookup"><span data-stu-id="8bb90-108">Date</span></span>   |
| <span data-ttu-id="8bb90-109">ws</span><span class="sxs-lookup"><span data-stu-id="8bb90-109">windows</span></span>           | <span data-ttu-id="8bb90-110">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb90-110">Int64</span></span>  |
| <span data-ttu-id="8bb90-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="8bb90-111">windowsPhone</span></span>      | <span data-ttu-id="8bb90-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb90-112">Int64</span></span>  |
| <span data-ttu-id="8bb90-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="8bb90-113">androidPhone</span></span>      | <span data-ttu-id="8bb90-114">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb90-114">Int64</span></span>  |
| <span data-ttu-id="8bb90-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="8bb90-115">iPhone</span></span>            | <span data-ttu-id="8bb90-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb90-116">Int64</span></span>  |
| <span data-ttu-id="8bb90-117">iPad</span><span class="sxs-lookup"><span data-stu-id="8bb90-117">iPad</span></span>              | <span data-ttu-id="8bb90-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb90-118">Int64</span></span>  |
| <span data-ttu-id="8bb90-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="8bb90-119">reportDate</span></span>        | <span data-ttu-id="8bb90-120">日付</span><span class="sxs-lookup"><span data-stu-id="8bb90-120">Date</span></span>   |
| <span data-ttu-id="8bb90-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8bb90-121">reportPeriod</span></span>      | <span data-ttu-id="8bb90-122">String</span><span class="sxs-lookup"><span data-stu-id="8bb90-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8bb90-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8bb90-123">JSON representation</span></span>

<span data-ttu-id="8bb90-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bb90-124">The following is a JSON representation of the resource.</span></span>

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
