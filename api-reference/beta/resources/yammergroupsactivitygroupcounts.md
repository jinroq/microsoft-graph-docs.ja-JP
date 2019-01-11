---
title: yammerGroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 71c80f167c59f2452210575ca1c1be6608f0d203
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860950"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a><span data-ttu-id="44837-103">yammerGroupsActivityGroupCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44837-103">yammerGroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="44837-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44837-104">Properties</span></span>

| <span data-ttu-id="44837-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44837-105">Property</span></span>          | <span data-ttu-id="44837-106">種類</span><span class="sxs-lookup"><span data-stu-id="44837-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="44837-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="44837-107">reportRefreshDate</span></span> | <span data-ttu-id="44837-108">日付</span><span class="sxs-lookup"><span data-stu-id="44837-108">Date</span></span>   |
| <span data-ttu-id="44837-109">total</span><span class="sxs-lookup"><span data-stu-id="44837-109">total</span></span>             | <span data-ttu-id="44837-110">Int64</span><span class="sxs-lookup"><span data-stu-id="44837-110">Int64</span></span>  |
| <span data-ttu-id="44837-111">アクティブです</span><span class="sxs-lookup"><span data-stu-id="44837-111">active</span></span>            | <span data-ttu-id="44837-112">Int64</span><span class="sxs-lookup"><span data-stu-id="44837-112">Int64</span></span>  |
| <span data-ttu-id="44837-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="44837-113">reportDate</span></span>        | <span data-ttu-id="44837-114">日付</span><span class="sxs-lookup"><span data-stu-id="44837-114">Date</span></span>   |
| <span data-ttu-id="44837-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="44837-115">reportPeriod</span></span>      | <span data-ttu-id="44837-116">String</span><span class="sxs-lookup"><span data-stu-id="44837-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44837-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44837-117">JSON representation</span></span>

<span data-ttu-id="44837-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44837-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
