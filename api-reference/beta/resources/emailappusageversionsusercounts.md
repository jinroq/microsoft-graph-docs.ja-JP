---
title: emailAppUsageVersionsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 18b86708071f1fab573571703dbb5bc253fcf2ce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972139"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="8d7c9-103">emailAppUsageVersionsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d7c9-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8d7c9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d7c9-104">Properties</span></span>

| <span data-ttu-id="8d7c9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d7c9-105">Property</span></span>          | <span data-ttu-id="8d7c9-106">型</span><span class="sxs-lookup"><span data-stu-id="8d7c9-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8d7c9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8d7c9-107">reportRefreshDate</span></span> | <span data-ttu-id="8d7c9-108">日付</span><span class="sxs-lookup"><span data-stu-id="8d7c9-108">Date</span></span>   |
| <span data-ttu-id="8d7c9-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="8d7c9-109">outlook2016</span></span>       | <span data-ttu-id="8d7c9-110">Int64</span><span class="sxs-lookup"><span data-stu-id="8d7c9-110">Int64</span></span>  |
| <span data-ttu-id="8d7c9-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="8d7c9-111">outlook2013</span></span>       | <span data-ttu-id="8d7c9-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8d7c9-112">Int64</span></span>  |
| <span data-ttu-id="8d7c9-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="8d7c9-113">outlook2010</span></span>       | <span data-ttu-id="8d7c9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="8d7c9-114">Int64</span></span>  |
| <span data-ttu-id="8d7c9-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="8d7c9-115">outlook2007</span></span>       | <span data-ttu-id="8d7c9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8d7c9-116">Int64</span></span>  |
| <span data-ttu-id="8d7c9-117">変換</span><span class="sxs-lookup"><span data-stu-id="8d7c9-117">undetermined</span></span>      | <span data-ttu-id="8d7c9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8d7c9-118">Int64</span></span>  |
| <span data-ttu-id="8d7c9-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8d7c9-119">reportPeriod</span></span>      | <span data-ttu-id="8d7c9-120">String</span><span class="sxs-lookup"><span data-stu-id="8d7c9-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d7c9-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d7c9-121">JSON representation</span></span>

<span data-ttu-id="8d7c9-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d7c9-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
