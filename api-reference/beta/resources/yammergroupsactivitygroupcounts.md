---
title: yammerGroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ae47231c7d2ee1b517e8fe64869fbee625d549e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987791"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a><span data-ttu-id="35535-103">yammerGroupsActivityGroupCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35535-103">yammerGroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="35535-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35535-104">Properties</span></span>

| <span data-ttu-id="35535-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35535-105">Property</span></span>          | <span data-ttu-id="35535-106">種類</span><span class="sxs-lookup"><span data-stu-id="35535-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="35535-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="35535-107">reportRefreshDate</span></span> | <span data-ttu-id="35535-108">日付</span><span class="sxs-lookup"><span data-stu-id="35535-108">Date</span></span>   |
| <span data-ttu-id="35535-109">total</span><span class="sxs-lookup"><span data-stu-id="35535-109">total</span></span>             | <span data-ttu-id="35535-110">Int64</span><span class="sxs-lookup"><span data-stu-id="35535-110">Int64</span></span>  |
| <span data-ttu-id="35535-111">アクティブです</span><span class="sxs-lookup"><span data-stu-id="35535-111">active</span></span>            | <span data-ttu-id="35535-112">Int64</span><span class="sxs-lookup"><span data-stu-id="35535-112">Int64</span></span>  |
| <span data-ttu-id="35535-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="35535-113">reportDate</span></span>        | <span data-ttu-id="35535-114">日付</span><span class="sxs-lookup"><span data-stu-id="35535-114">Date</span></span>   |
| <span data-ttu-id="35535-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="35535-115">reportPeriod</span></span>      | <span data-ttu-id="35535-116">String</span><span class="sxs-lookup"><span data-stu-id="35535-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35535-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35535-117">JSON representation</span></span>

<span data-ttu-id="35535-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="35535-118">The following is a JSON representation of the resource.</span></span>

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
