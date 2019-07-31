---
title: Teamsdevice使い方 User計数リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99cb675880962591d6298062f979f0930bc0a15d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964397"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="5c533-103">Teamsdevice使い方 User計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c533-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5c533-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c533-104">Properties</span></span>

| <span data-ttu-id="5c533-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c533-105">Property</span></span>          | <span data-ttu-id="5c533-106">型</span><span class="sxs-lookup"><span data-stu-id="5c533-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5c533-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5c533-107">reportRefreshDate</span></span> | <span data-ttu-id="5c533-108">日付</span><span class="sxs-lookup"><span data-stu-id="5c533-108">Date</span></span>   |
| <span data-ttu-id="5c533-109">Web</span><span class="sxs-lookup"><span data-stu-id="5c533-109">web</span></span>               | <span data-ttu-id="5c533-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5c533-110">Int64</span></span>  |
| <span data-ttu-id="5c533-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5c533-111">windowsPhone</span></span>      | <span data-ttu-id="5c533-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5c533-112">Int64</span></span>  |
| <span data-ttu-id="5c533-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="5c533-113">androidPhone</span></span>      | <span data-ttu-id="5c533-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5c533-114">Int64</span></span>  |
| <span data-ttu-id="5c533-115">ios</span><span class="sxs-lookup"><span data-stu-id="5c533-115">ios</span></span>               | <span data-ttu-id="5c533-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5c533-116">Int64</span></span>  |
| <span data-ttu-id="5c533-117">Mac</span><span class="sxs-lookup"><span data-stu-id="5c533-117">mac</span></span>               | <span data-ttu-id="5c533-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5c533-118">Int64</span></span>  |
| <span data-ttu-id="5c533-119">ws</span><span class="sxs-lookup"><span data-stu-id="5c533-119">windows</span></span>           | <span data-ttu-id="5c533-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5c533-120">Int64</span></span>  |
| <span data-ttu-id="5c533-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="5c533-121">reportDate</span></span>        | <span data-ttu-id="5c533-122">日付</span><span class="sxs-lookup"><span data-stu-id="5c533-122">Date</span></span>   |
| <span data-ttu-id="5c533-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5c533-123">reportPeriod</span></span>      | <span data-ttu-id="5c533-124">String</span><span class="sxs-lookup"><span data-stu-id="5c533-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5c533-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c533-125">JSON representation</span></span>

<span data-ttu-id="5c533-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c533-126">The following is a JSON representation of the resource.</span></span>

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
