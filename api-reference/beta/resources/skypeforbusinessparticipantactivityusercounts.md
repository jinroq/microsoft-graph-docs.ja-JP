---
title: skypeForBusinessParticipantActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f6feb87de8b62dcf4f958a5c2bc6aaeda3ef454d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008111"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="3c60a-103">skypeForBusinessParticipantActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c60a-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3c60a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c60a-104">Properties</span></span>

| <span data-ttu-id="3c60a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c60a-105">Property</span></span>          | <span data-ttu-id="3c60a-106">型</span><span class="sxs-lookup"><span data-stu-id="3c60a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3c60a-107">im</span><span class="sxs-lookup"><span data-stu-id="3c60a-107">im</span></span>                | <span data-ttu-id="3c60a-108">Int64</span><span class="sxs-lookup"><span data-stu-id="3c60a-108">Int64</span></span>  |
| <span data-ttu-id="3c60a-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="3c60a-109">audioVideo</span></span>        | <span data-ttu-id="3c60a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="3c60a-110">Int64</span></span>  |
| <span data-ttu-id="3c60a-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="3c60a-111">appSharing</span></span>        | <span data-ttu-id="3c60a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3c60a-112">Int64</span></span>  |
| <span data-ttu-id="3c60a-113">Web</span><span class="sxs-lookup"><span data-stu-id="3c60a-113">web</span></span>               | <span data-ttu-id="3c60a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3c60a-114">Int64</span></span>  |
| <span data-ttu-id="3c60a-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="3c60a-115">dialInOut3rdParty</span></span> | <span data-ttu-id="3c60a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3c60a-116">Int64</span></span>  |
| <span data-ttu-id="3c60a-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3c60a-117">reportRefreshDate</span></span> | <span data-ttu-id="3c60a-118">日付</span><span class="sxs-lookup"><span data-stu-id="3c60a-118">Date</span></span>   |
| <span data-ttu-id="3c60a-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="3c60a-119">reportDate</span></span>        | <span data-ttu-id="3c60a-120">日付</span><span class="sxs-lookup"><span data-stu-id="3c60a-120">Date</span></span>   |
| <span data-ttu-id="3c60a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3c60a-121">reportPeriod</span></span>      | <span data-ttu-id="3c60a-122">String</span><span class="sxs-lookup"><span data-stu-id="3c60a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3c60a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c60a-123">JSON representation</span></span>

<span data-ttu-id="3c60a-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3c60a-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 196, 
  "appSharing": 196, 
  "web": 196, 
  "dialInOut3rdParty": 196, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
