---
title: yammerGroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 4c342686ce2397a5d3b1dd697002fb44e16f3b11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006921"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a><span data-ttu-id="48091-103">yammerGroupsActivityGroupCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48091-103">yammerGroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="48091-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48091-104">Properties</span></span>

| <span data-ttu-id="48091-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48091-105">Property</span></span>          | <span data-ttu-id="48091-106">型</span><span class="sxs-lookup"><span data-stu-id="48091-106">Type</span></span>   | <span data-ttu-id="48091-107">説明</span><span class="sxs-lookup"><span data-stu-id="48091-107">Description</span></span> |
| :---------------- | :----- | :---------- |
| <span data-ttu-id="48091-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="48091-108">reportRefreshDate</span></span> | <span data-ttu-id="48091-109">日付</span><span class="sxs-lookup"><span data-stu-id="48091-109">Date</span></span>   |             |
| <span data-ttu-id="48091-110">total</span><span class="sxs-lookup"><span data-stu-id="48091-110">total</span></span>             | <span data-ttu-id="48091-111">Int64</span><span class="sxs-lookup"><span data-stu-id="48091-111">Int64</span></span>  |             |
| <span data-ttu-id="48091-112">active</span><span class="sxs-lookup"><span data-stu-id="48091-112">active</span></span>            | <span data-ttu-id="48091-113">Int64</span><span class="sxs-lookup"><span data-stu-id="48091-113">Int64</span></span>  |             |
| <span data-ttu-id="48091-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="48091-114">reportDate</span></span>        | <span data-ttu-id="48091-115">日付</span><span class="sxs-lookup"><span data-stu-id="48091-115">Date</span></span>   |             |
| <span data-ttu-id="48091-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="48091-116">reportPeriod</span></span>      | <span data-ttu-id="48091-117">String</span><span class="sxs-lookup"><span data-stu-id="48091-117">String</span></span> |             |

## <a name="json-representation"></a><span data-ttu-id="48091-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48091-118">JSON representation</span></span>

<span data-ttu-id="48091-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="48091-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "String", 
  "reportPeriod": "String"
}
```
