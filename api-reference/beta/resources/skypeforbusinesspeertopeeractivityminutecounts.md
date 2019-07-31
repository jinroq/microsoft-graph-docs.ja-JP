---
title: skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2fcea49c157a04dd48eda0f1645eab08540a917e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008062"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="0f19e-103">skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f19e-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0f19e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f19e-104">Properties</span></span>

| <span data-ttu-id="0f19e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f19e-105">Property</span></span>          | <span data-ttu-id="0f19e-106">型</span><span class="sxs-lookup"><span data-stu-id="0f19e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0f19e-107">audio</span><span class="sxs-lookup"><span data-stu-id="0f19e-107">audio</span></span>             | <span data-ttu-id="0f19e-108">Int64</span><span class="sxs-lookup"><span data-stu-id="0f19e-108">Int64</span></span>  |
| <span data-ttu-id="0f19e-109">video</span><span class="sxs-lookup"><span data-stu-id="0f19e-109">video</span></span>             | <span data-ttu-id="0f19e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="0f19e-110">Int64</span></span>  |
| <span data-ttu-id="0f19e-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0f19e-111">reportRefreshDate</span></span> | <span data-ttu-id="0f19e-112">日付</span><span class="sxs-lookup"><span data-stu-id="0f19e-112">Date</span></span>   |
| <span data-ttu-id="0f19e-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="0f19e-113">reportDate</span></span>        | <span data-ttu-id="0f19e-114">日付</span><span class="sxs-lookup"><span data-stu-id="0f19e-114">Date</span></span>   |
| <span data-ttu-id="0f19e-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0f19e-115">reportPeriod</span></span>      | <span data-ttu-id="0f19e-116">String</span><span class="sxs-lookup"><span data-stu-id="0f19e-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f19e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f19e-117">JSON representation</span></span>

<span data-ttu-id="0f19e-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0f19e-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024, 
  "video": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
