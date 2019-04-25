---
title: skypeForBusinessPeerToPeerActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 4baf218ed9398a8f208c4d1d44a28579773dea6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523456"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="ff734-103">skypeForBusinessPeerToPeerActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff734-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ff734-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff734-104">Properties</span></span>

| <span data-ttu-id="ff734-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff734-105">Property</span></span>          | <span data-ttu-id="ff734-106">型</span><span class="sxs-lookup"><span data-stu-id="ff734-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ff734-107">im</span><span class="sxs-lookup"><span data-stu-id="ff734-107">im</span></span>                | <span data-ttu-id="ff734-108">Int64</span><span class="sxs-lookup"><span data-stu-id="ff734-108">Int64</span></span>  |
| <span data-ttu-id="ff734-109">audio</span><span class="sxs-lookup"><span data-stu-id="ff734-109">audio</span></span>             | <span data-ttu-id="ff734-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ff734-110">Int64</span></span>  |
| <span data-ttu-id="ff734-111">video</span><span class="sxs-lookup"><span data-stu-id="ff734-111">video</span></span>             | <span data-ttu-id="ff734-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ff734-112">Int64</span></span>  |
| <span data-ttu-id="ff734-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="ff734-113">appSharing</span></span>        | <span data-ttu-id="ff734-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ff734-114">Int64</span></span>  |
| <span data-ttu-id="ff734-115">filetransfer</span><span class="sxs-lookup"><span data-stu-id="ff734-115">fileTransfer</span></span>      | <span data-ttu-id="ff734-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ff734-116">Int64</span></span>  |
| <span data-ttu-id="ff734-117">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="ff734-117">reportRefreshDate</span></span> | <span data-ttu-id="ff734-118">Date</span><span class="sxs-lookup"><span data-stu-id="ff734-118">Date</span></span>   |
| <span data-ttu-id="ff734-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="ff734-119">reportDate</span></span>        | <span data-ttu-id="ff734-120">Date</span><span class="sxs-lookup"><span data-stu-id="ff734-120">Date</span></span>   |
| <span data-ttu-id="ff734-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="ff734-121">reportPeriod</span></span>      | <span data-ttu-id="ff734-122">String</span><span class="sxs-lookup"><span data-stu-id="ff734-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff734-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff734-123">JSON representation</span></span>

<span data-ttu-id="ff734-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff734-124">The following is a JSON representation of the resource.</span></span>

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
