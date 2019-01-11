---
title: skypeForBusinessPeerToPeerActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 4baf218ed9398a8f208c4d1d44a28579773dea6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874474"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="04462-103">skypeForBusinessPeerToPeerActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04462-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="04462-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04462-104">Properties</span></span>

| <span data-ttu-id="04462-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04462-105">Property</span></span>          | <span data-ttu-id="04462-106">種類</span><span class="sxs-lookup"><span data-stu-id="04462-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="04462-107">im</span><span class="sxs-lookup"><span data-stu-id="04462-107">im</span></span>                | <span data-ttu-id="04462-108">Int64</span><span class="sxs-lookup"><span data-stu-id="04462-108">Int64</span></span>  |
| <span data-ttu-id="04462-109">audio</span><span class="sxs-lookup"><span data-stu-id="04462-109">audio</span></span>             | <span data-ttu-id="04462-110">Int64</span><span class="sxs-lookup"><span data-stu-id="04462-110">Int64</span></span>  |
| <span data-ttu-id="04462-111">video</span><span class="sxs-lookup"><span data-stu-id="04462-111">video</span></span>             | <span data-ttu-id="04462-112">Int64</span><span class="sxs-lookup"><span data-stu-id="04462-112">Int64</span></span>  |
| <span data-ttu-id="04462-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="04462-113">appSharing</span></span>        | <span data-ttu-id="04462-114">Int64</span><span class="sxs-lookup"><span data-stu-id="04462-114">Int64</span></span>  |
| <span data-ttu-id="04462-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="04462-115">fileTransfer</span></span>      | <span data-ttu-id="04462-116">Int64</span><span class="sxs-lookup"><span data-stu-id="04462-116">Int64</span></span>  |
| <span data-ttu-id="04462-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="04462-117">reportRefreshDate</span></span> | <span data-ttu-id="04462-118">日付</span><span class="sxs-lookup"><span data-stu-id="04462-118">Date</span></span>   |
| <span data-ttu-id="04462-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="04462-119">reportDate</span></span>        | <span data-ttu-id="04462-120">日付</span><span class="sxs-lookup"><span data-stu-id="04462-120">Date</span></span>   |
| <span data-ttu-id="04462-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="04462-121">reportPeriod</span></span>      | <span data-ttu-id="04462-122">String</span><span class="sxs-lookup"><span data-stu-id="04462-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="04462-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04462-123">JSON representation</span></span>

<span data-ttu-id="04462-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="04462-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
