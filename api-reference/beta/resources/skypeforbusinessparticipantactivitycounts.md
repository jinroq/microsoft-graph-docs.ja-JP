---
title: skypeForBusinessParticipantActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9e070dd3dc4687ee70f3189812e5f55ea90d718a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008125"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="25710-103">skypeForBusinessParticipantActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25710-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="25710-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25710-104">Properties</span></span>

| <span data-ttu-id="25710-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25710-105">Property</span></span>          | <span data-ttu-id="25710-106">型</span><span class="sxs-lookup"><span data-stu-id="25710-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="25710-107">im</span><span class="sxs-lookup"><span data-stu-id="25710-107">im</span></span>                | <span data-ttu-id="25710-108">Int64</span><span class="sxs-lookup"><span data-stu-id="25710-108">Int64</span></span>  |
| <span data-ttu-id="25710-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="25710-109">audioVideo</span></span>        | <span data-ttu-id="25710-110">Int64</span><span class="sxs-lookup"><span data-stu-id="25710-110">Int64</span></span>  |
| <span data-ttu-id="25710-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="25710-111">appSharing</span></span>        | <span data-ttu-id="25710-112">Int64</span><span class="sxs-lookup"><span data-stu-id="25710-112">Int64</span></span>  |
| <span data-ttu-id="25710-113">Web</span><span class="sxs-lookup"><span data-stu-id="25710-113">web</span></span>               | <span data-ttu-id="25710-114">Int64</span><span class="sxs-lookup"><span data-stu-id="25710-114">Int64</span></span>  |
| <span data-ttu-id="25710-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="25710-115">dialInOut3rdParty</span></span> | <span data-ttu-id="25710-116">Int64</span><span class="sxs-lookup"><span data-stu-id="25710-116">Int64</span></span>  |
| <span data-ttu-id="25710-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="25710-117">reportRefreshDate</span></span> | <span data-ttu-id="25710-118">日付</span><span class="sxs-lookup"><span data-stu-id="25710-118">Date</span></span>   |
| <span data-ttu-id="25710-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="25710-119">reportDate</span></span>        | <span data-ttu-id="25710-120">日付</span><span class="sxs-lookup"><span data-stu-id="25710-120">Date</span></span>   |
| <span data-ttu-id="25710-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="25710-121">reportPeriod</span></span>      | <span data-ttu-id="25710-122">String</span><span class="sxs-lookup"><span data-stu-id="25710-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="25710-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25710-123">JSON representation</span></span>

<span data-ttu-id="25710-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="25710-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
