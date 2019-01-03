---
title: teamsDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
ms.openlocfilehash: 1255a8e1e92bb461d5c100c72e9030f57db5f8fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306511"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="6532a-103">teamsDeviceUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6532a-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6532a-104">Properties</span><span class="sxs-lookup"><span data-stu-id="6532a-104">Properties</span></span>

| <span data-ttu-id="6532a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6532a-105">Property</span></span>          | <span data-ttu-id="6532a-106">種類</span><span class="sxs-lookup"><span data-stu-id="6532a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6532a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6532a-107">reportRefreshDate</span></span> | <span data-ttu-id="6532a-108">日付</span><span class="sxs-lookup"><span data-stu-id="6532a-108">Date</span></span>   |
| <span data-ttu-id="6532a-109">web</span><span class="sxs-lookup"><span data-stu-id="6532a-109">web</span></span>               | <span data-ttu-id="6532a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6532a-110">Int64</span></span>  |
| <span data-ttu-id="6532a-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="6532a-111">windowsPhone</span></span>      | <span data-ttu-id="6532a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6532a-112">Int64</span></span>  |
| <span data-ttu-id="6532a-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="6532a-113">androidPhone</span></span>      | <span data-ttu-id="6532a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6532a-114">Int64</span></span>  |
| <span data-ttu-id="6532a-115">ios</span><span class="sxs-lookup"><span data-stu-id="6532a-115">ios</span></span>               | <span data-ttu-id="6532a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6532a-116">Int64</span></span>  |
| <span data-ttu-id="6532a-117">Mac</span><span class="sxs-lookup"><span data-stu-id="6532a-117">mac</span></span>               | <span data-ttu-id="6532a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6532a-118">Int64</span></span>  |
| <span data-ttu-id="6532a-119">windows</span><span class="sxs-lookup"><span data-stu-id="6532a-119">windows</span></span>           | <span data-ttu-id="6532a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6532a-120">Int64</span></span>  |
| <span data-ttu-id="6532a-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="6532a-121">reportDate</span></span>        | <span data-ttu-id="6532a-122">日付</span><span class="sxs-lookup"><span data-stu-id="6532a-122">Date</span></span>   |
| <span data-ttu-id="6532a-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6532a-123">reportPeriod</span></span>      | <span data-ttu-id="6532a-124">String</span><span class="sxs-lookup"><span data-stu-id="6532a-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6532a-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6532a-125">JSON representation</span></span>

<span data-ttu-id="6532a-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6532a-126">The following is a JSON representation of the resource.</span></span>

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