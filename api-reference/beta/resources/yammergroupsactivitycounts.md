---
title: yammerGroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 404dcd44baac005374634db097b79c10c86ae78f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577285"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="13487-103">yammerGroupsActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13487-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="13487-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13487-104">Properties</span></span>

| <span data-ttu-id="13487-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13487-105">Property</span></span>          | <span data-ttu-id="13487-106">型</span><span class="sxs-lookup"><span data-stu-id="13487-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="13487-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="13487-107">reportRefreshDate</span></span> | <span data-ttu-id="13487-108">日付</span><span class="sxs-lookup"><span data-stu-id="13487-108">Date</span></span>   |
| <span data-ttu-id="13487-109">気に入られました</span><span class="sxs-lookup"><span data-stu-id="13487-109">liked</span></span>             | <span data-ttu-id="13487-110">Int64</span><span class="sxs-lookup"><span data-stu-id="13487-110">Int64</span></span>  |
| <span data-ttu-id="13487-111">転記</span><span class="sxs-lookup"><span data-stu-id="13487-111">posted</span></span>            | <span data-ttu-id="13487-112">Int64</span><span class="sxs-lookup"><span data-stu-id="13487-112">Int64</span></span>  |
| <span data-ttu-id="13487-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="13487-113">read</span></span>              | <span data-ttu-id="13487-114">Int64</span><span class="sxs-lookup"><span data-stu-id="13487-114">Int64</span></span>  |
| <span data-ttu-id="13487-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="13487-115">reportDate</span></span>        | <span data-ttu-id="13487-116">日付</span><span class="sxs-lookup"><span data-stu-id="13487-116">Date</span></span>   |
| <span data-ttu-id="13487-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="13487-117">reportPeriod</span></span>      | <span data-ttu-id="13487-118">String</span><span class="sxs-lookup"><span data-stu-id="13487-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13487-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13487-119">JSON representation</span></span>

<span data-ttu-id="13487-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13487-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
