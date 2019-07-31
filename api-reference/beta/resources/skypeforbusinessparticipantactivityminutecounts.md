---
title: skypeForBusinessParticipantActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4e732b9358eec99d73152f7f50f38eb3cb767e4c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964880"
---
# <a name="skypeforbusinessparticipantactivityminutecounts-resource-type"></a><span data-ttu-id="cd56b-103">skypeForBusinessParticipantActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cd56b-103">skypeForBusinessParticipantActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cd56b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd56b-104">Properties</span></span>

| <span data-ttu-id="cd56b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd56b-105">Property</span></span>          | <span data-ttu-id="cd56b-106">型</span><span class="sxs-lookup"><span data-stu-id="cd56b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="cd56b-107">audioVideo</span><span class="sxs-lookup"><span data-stu-id="cd56b-107">audioVideo</span></span>        | <span data-ttu-id="cd56b-108">Int64</span><span class="sxs-lookup"><span data-stu-id="cd56b-108">Int64</span></span>  |
| <span data-ttu-id="cd56b-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cd56b-109">reportRefreshDate</span></span> | <span data-ttu-id="cd56b-110">日付</span><span class="sxs-lookup"><span data-stu-id="cd56b-110">Date</span></span>   |
| <span data-ttu-id="cd56b-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="cd56b-111">reportDate</span></span>        | <span data-ttu-id="cd56b-112">日付</span><span class="sxs-lookup"><span data-stu-id="cd56b-112">Date</span></span>   |
| <span data-ttu-id="cd56b-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cd56b-113">reportPeriod</span></span>      | <span data-ttu-id="cd56b-114">String</span><span class="sxs-lookup"><span data-stu-id="cd56b-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cd56b-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cd56b-115">JSON representation</span></span>

<span data-ttu-id="cd56b-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cd56b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts"
} -->

```json
{
  "audiovideo": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
