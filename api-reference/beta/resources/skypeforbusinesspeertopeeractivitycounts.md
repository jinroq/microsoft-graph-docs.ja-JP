---
title: skypeForBusinessPeerToPeerActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: cdc8ec2a63c4a03ac8b77bedba06c6addfba4584
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069802"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="000ec-103">skypeForBusinessPeerToPeerActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="000ec-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="000ec-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="000ec-104">Properties</span></span>

| <span data-ttu-id="000ec-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="000ec-105">Property</span></span>          | <span data-ttu-id="000ec-106">型</span><span class="sxs-lookup"><span data-stu-id="000ec-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="000ec-107">im</span><span class="sxs-lookup"><span data-stu-id="000ec-107">im</span></span>                | <span data-ttu-id="000ec-108">Int64</span><span class="sxs-lookup"><span data-stu-id="000ec-108">Int64</span></span>  |
| <span data-ttu-id="000ec-109">audio</span><span class="sxs-lookup"><span data-stu-id="000ec-109">audio</span></span>             | <span data-ttu-id="000ec-110">Int64</span><span class="sxs-lookup"><span data-stu-id="000ec-110">Int64</span></span>  |
| <span data-ttu-id="000ec-111">video</span><span class="sxs-lookup"><span data-stu-id="000ec-111">video</span></span>             | <span data-ttu-id="000ec-112">Int64</span><span class="sxs-lookup"><span data-stu-id="000ec-112">Int64</span></span>  |
| <span data-ttu-id="000ec-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="000ec-113">appSharing</span></span>        | <span data-ttu-id="000ec-114">Int64</span><span class="sxs-lookup"><span data-stu-id="000ec-114">Int64</span></span>  |
| <span data-ttu-id="000ec-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="000ec-115">fileTransfer</span></span>      | <span data-ttu-id="000ec-116">Int64</span><span class="sxs-lookup"><span data-stu-id="000ec-116">Int64</span></span>  |
| <span data-ttu-id="000ec-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="000ec-117">reportRefreshDate</span></span> | <span data-ttu-id="000ec-118">Date</span><span class="sxs-lookup"><span data-stu-id="000ec-118">Date</span></span>   |
| <span data-ttu-id="000ec-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="000ec-119">reportDate</span></span>        | <span data-ttu-id="000ec-120">Date</span><span class="sxs-lookup"><span data-stu-id="000ec-120">Date</span></span>   |
| <span data-ttu-id="000ec-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="000ec-121">reportPeriod</span></span>      | <span data-ttu-id="000ec-122">String</span><span class="sxs-lookup"><span data-stu-id="000ec-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="000ec-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="000ec-123">JSON representation</span></span>

<span data-ttu-id="000ec-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="000ec-124">The following is a JSON representation of the resource.</span></span>

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
