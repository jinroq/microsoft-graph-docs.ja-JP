---
title: skypeForBusinessPeerToPeerActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 619e581fcdd25dda10be7210aefe5db8e4dcd8b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828638"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="52e83-103">skypeForBusinessPeerToPeerActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52e83-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="52e83-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52e83-104">Properties</span></span>

| <span data-ttu-id="52e83-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52e83-105">Property</span></span>          | <span data-ttu-id="52e83-106">種類</span><span class="sxs-lookup"><span data-stu-id="52e83-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="52e83-107">im</span><span class="sxs-lookup"><span data-stu-id="52e83-107">im</span></span>                | <span data-ttu-id="52e83-108">Int64</span><span class="sxs-lookup"><span data-stu-id="52e83-108">Int64</span></span>  |
| <span data-ttu-id="52e83-109">audio</span><span class="sxs-lookup"><span data-stu-id="52e83-109">audio</span></span>             | <span data-ttu-id="52e83-110">Int64</span><span class="sxs-lookup"><span data-stu-id="52e83-110">Int64</span></span>  |
| <span data-ttu-id="52e83-111">video</span><span class="sxs-lookup"><span data-stu-id="52e83-111">video</span></span>             | <span data-ttu-id="52e83-112">Int64</span><span class="sxs-lookup"><span data-stu-id="52e83-112">Int64</span></span>  |
| <span data-ttu-id="52e83-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="52e83-113">appSharing</span></span>        | <span data-ttu-id="52e83-114">Int64</span><span class="sxs-lookup"><span data-stu-id="52e83-114">Int64</span></span>  |
| <span data-ttu-id="52e83-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="52e83-115">fileTransfer</span></span>      | <span data-ttu-id="52e83-116">Int64</span><span class="sxs-lookup"><span data-stu-id="52e83-116">Int64</span></span>  |
| <span data-ttu-id="52e83-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="52e83-117">reportRefreshDate</span></span> | <span data-ttu-id="52e83-118">日付</span><span class="sxs-lookup"><span data-stu-id="52e83-118">Date</span></span>   |
| <span data-ttu-id="52e83-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="52e83-119">reportDate</span></span>        | <span data-ttu-id="52e83-120">日付</span><span class="sxs-lookup"><span data-stu-id="52e83-120">Date</span></span>   |
| <span data-ttu-id="52e83-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="52e83-121">reportPeriod</span></span>      | <span data-ttu-id="52e83-122">String</span><span class="sxs-lookup"><span data-stu-id="52e83-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52e83-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52e83-123">JSON representation</span></span>

<span data-ttu-id="52e83-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52e83-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
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
