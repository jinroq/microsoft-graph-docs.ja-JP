---
title: skypeforbusinessactivitycounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: e59bd33b1709780bac9726ee716ef9d81ef33c1f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568160"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="2f4a6-103">skypeforbusinessactivitycounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f4a6-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2f4a6-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f4a6-104">Properties</span></span>

| <span data-ttu-id="2f4a6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f4a6-105">Property</span></span>          | <span data-ttu-id="2f4a6-106">型</span><span class="sxs-lookup"><span data-stu-id="2f4a6-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2f4a6-107">peertopeer</span><span class="sxs-lookup"><span data-stu-id="2f4a6-107">peerToPeer</span></span>        | <span data-ttu-id="2f4a6-108">Int64</span><span class="sxs-lookup"><span data-stu-id="2f4a6-108">Int64</span></span>  |
| <span data-ttu-id="2f4a6-109">別</span><span class="sxs-lookup"><span data-stu-id="2f4a6-109">organized</span></span>         | <span data-ttu-id="2f4a6-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2f4a6-110">Int64</span></span>  |
| <span data-ttu-id="2f4a6-111">参加した</span><span class="sxs-lookup"><span data-stu-id="2f4a6-111">participated</span></span>      | <span data-ttu-id="2f4a6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2f4a6-112">Int64</span></span>  |
| <span data-ttu-id="2f4a6-113">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="2f4a6-113">reportRefreshDate</span></span> | <span data-ttu-id="2f4a6-114">Date</span><span class="sxs-lookup"><span data-stu-id="2f4a6-114">Date</span></span>   |
| <span data-ttu-id="2f4a6-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="2f4a6-115">reportDate</span></span>        | <span data-ttu-id="2f4a6-116">Date</span><span class="sxs-lookup"><span data-stu-id="2f4a6-116">Date</span></span>   |
| <span data-ttu-id="2f4a6-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="2f4a6-117">reportPeriod</span></span>      | <span data-ttu-id="2f4a6-118">String</span><span class="sxs-lookup"><span data-stu-id="2f4a6-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f4a6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f4a6-119">JSON representation</span></span>

<span data-ttu-id="2f4a6-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f4a6-120">The following is a JSON representation of the resource.</span></span>

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
