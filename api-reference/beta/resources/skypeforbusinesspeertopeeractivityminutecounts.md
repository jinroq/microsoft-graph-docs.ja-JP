---
title: skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 5377e8d8f2ec145f5aee590409206de75e915d9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073322"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="9f838-103">skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f838-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9f838-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f838-104">Properties</span></span>

| <span data-ttu-id="9f838-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f838-105">Property</span></span>          | <span data-ttu-id="9f838-106">型</span><span class="sxs-lookup"><span data-stu-id="9f838-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="9f838-107">audio</span><span class="sxs-lookup"><span data-stu-id="9f838-107">audio</span></span>             | <span data-ttu-id="9f838-108">Int64</span><span class="sxs-lookup"><span data-stu-id="9f838-108">Int64</span></span>  |
| <span data-ttu-id="9f838-109">video</span><span class="sxs-lookup"><span data-stu-id="9f838-109">video</span></span>             | <span data-ttu-id="9f838-110">Int64</span><span class="sxs-lookup"><span data-stu-id="9f838-110">Int64</span></span>  |
| <span data-ttu-id="9f838-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9f838-111">reportRefreshDate</span></span> | <span data-ttu-id="9f838-112">Date</span><span class="sxs-lookup"><span data-stu-id="9f838-112">Date</span></span>   |
| <span data-ttu-id="9f838-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="9f838-113">reportDate</span></span>        | <span data-ttu-id="9f838-114">Date</span><span class="sxs-lookup"><span data-stu-id="9f838-114">Date</span></span>   |
| <span data-ttu-id="9f838-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9f838-115">reportPeriod</span></span>      | <span data-ttu-id="9f838-116">String</span><span class="sxs-lookup"><span data-stu-id="9f838-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f838-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f838-117">JSON representation</span></span>

<span data-ttu-id="9f838-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9f838-118">The following is a JSON representation of the resource.</span></span>

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
