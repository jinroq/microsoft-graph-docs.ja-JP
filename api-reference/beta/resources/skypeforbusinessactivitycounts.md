---
title: skypeForBusinessActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c4f97f8377ec5693be1cc477ab40119675a24908
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008202"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="98cd2-103">skypeForBusinessActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98cd2-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="98cd2-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98cd2-104">Properties</span></span>

| <span data-ttu-id="98cd2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98cd2-105">Property</span></span>          | <span data-ttu-id="98cd2-106">型</span><span class="sxs-lookup"><span data-stu-id="98cd2-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="98cd2-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="98cd2-107">peerToPeer</span></span>        | <span data-ttu-id="98cd2-108">Int64</span><span class="sxs-lookup"><span data-stu-id="98cd2-108">Int64</span></span>  |
| <span data-ttu-id="98cd2-109">別</span><span class="sxs-lookup"><span data-stu-id="98cd2-109">organized</span></span>         | <span data-ttu-id="98cd2-110">Int64</span><span class="sxs-lookup"><span data-stu-id="98cd2-110">Int64</span></span>  |
| <span data-ttu-id="98cd2-111">参加した</span><span class="sxs-lookup"><span data-stu-id="98cd2-111">participated</span></span>      | <span data-ttu-id="98cd2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="98cd2-112">Int64</span></span>  |
| <span data-ttu-id="98cd2-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="98cd2-113">reportRefreshDate</span></span> | <span data-ttu-id="98cd2-114">日付</span><span class="sxs-lookup"><span data-stu-id="98cd2-114">Date</span></span>   |
| <span data-ttu-id="98cd2-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="98cd2-115">reportDate</span></span>        | <span data-ttu-id="98cd2-116">日付</span><span class="sxs-lookup"><span data-stu-id="98cd2-116">Date</span></span>   |
| <span data-ttu-id="98cd2-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="98cd2-117">reportPeriod</span></span>      | <span data-ttu-id="98cd2-118">String</span><span class="sxs-lookup"><span data-stu-id="98cd2-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="98cd2-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98cd2-119">JSON representation</span></span>

<span data-ttu-id="98cd2-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98cd2-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
