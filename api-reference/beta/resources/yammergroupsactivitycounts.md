---
title: yammerGroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: db9dfaa8c107acfa2c0f28fba2cfd06f242b166c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950831"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="15315-103">yammerGroupsActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15315-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="15315-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15315-104">Properties</span></span>

| <span data-ttu-id="15315-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15315-105">Property</span></span>          | <span data-ttu-id="15315-106">種類</span><span class="sxs-lookup"><span data-stu-id="15315-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="15315-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="15315-107">reportRefreshDate</span></span> | <span data-ttu-id="15315-108">日付</span><span class="sxs-lookup"><span data-stu-id="15315-108">Date</span></span>   |
| <span data-ttu-id="15315-109">気に入られました</span><span class="sxs-lookup"><span data-stu-id="15315-109">liked</span></span>             | <span data-ttu-id="15315-110">Int64</span><span class="sxs-lookup"><span data-stu-id="15315-110">Int64</span></span>  |
| <span data-ttu-id="15315-111">転記</span><span class="sxs-lookup"><span data-stu-id="15315-111">posted</span></span>            | <span data-ttu-id="15315-112">Int64</span><span class="sxs-lookup"><span data-stu-id="15315-112">Int64</span></span>  |
| <span data-ttu-id="15315-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="15315-113">read</span></span>              | <span data-ttu-id="15315-114">Int64</span><span class="sxs-lookup"><span data-stu-id="15315-114">Int64</span></span>  |
| <span data-ttu-id="15315-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="15315-115">reportDate</span></span>        | <span data-ttu-id="15315-116">日付</span><span class="sxs-lookup"><span data-stu-id="15315-116">Date</span></span>   |
| <span data-ttu-id="15315-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="15315-117">reportPeriod</span></span>      | <span data-ttu-id="15315-118">String</span><span class="sxs-lookup"><span data-stu-id="15315-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15315-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15315-119">JSON representation</span></span>

<span data-ttu-id="15315-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15315-120">The following is a JSON representation of the resource.</span></span>

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
