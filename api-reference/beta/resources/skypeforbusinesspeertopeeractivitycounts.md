---
title: skypeForBusinessPeerToPeerActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4075af51edb747146a764f8337e3ab2e4734caa4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964866"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="0b00e-103">skypeForBusinessPeerToPeerActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b00e-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0b00e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b00e-104">Properties</span></span>

| <span data-ttu-id="0b00e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b00e-105">Property</span></span>          | <span data-ttu-id="0b00e-106">型</span><span class="sxs-lookup"><span data-stu-id="0b00e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0b00e-107">im</span><span class="sxs-lookup"><span data-stu-id="0b00e-107">im</span></span>                | <span data-ttu-id="0b00e-108">Int64</span><span class="sxs-lookup"><span data-stu-id="0b00e-108">Int64</span></span>  |
| <span data-ttu-id="0b00e-109">audio</span><span class="sxs-lookup"><span data-stu-id="0b00e-109">audio</span></span>             | <span data-ttu-id="0b00e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="0b00e-110">Int64</span></span>  |
| <span data-ttu-id="0b00e-111">video</span><span class="sxs-lookup"><span data-stu-id="0b00e-111">video</span></span>             | <span data-ttu-id="0b00e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0b00e-112">Int64</span></span>  |
| <span data-ttu-id="0b00e-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="0b00e-113">appSharing</span></span>        | <span data-ttu-id="0b00e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0b00e-114">Int64</span></span>  |
| <span data-ttu-id="0b00e-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="0b00e-115">fileTransfer</span></span>      | <span data-ttu-id="0b00e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0b00e-116">Int64</span></span>  |
| <span data-ttu-id="0b00e-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0b00e-117">reportRefreshDate</span></span> | <span data-ttu-id="0b00e-118">日付</span><span class="sxs-lookup"><span data-stu-id="0b00e-118">Date</span></span>   |
| <span data-ttu-id="0b00e-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="0b00e-119">reportDate</span></span>        | <span data-ttu-id="0b00e-120">日付</span><span class="sxs-lookup"><span data-stu-id="0b00e-120">Date</span></span>   |
| <span data-ttu-id="0b00e-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0b00e-121">reportPeriod</span></span>      | <span data-ttu-id="0b00e-122">String</span><span class="sxs-lookup"><span data-stu-id="0b00e-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0b00e-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b00e-123">JSON representation</span></span>

<span data-ttu-id="0b00e-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b00e-124">The following is a JSON representation of the resource.</span></span>

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
