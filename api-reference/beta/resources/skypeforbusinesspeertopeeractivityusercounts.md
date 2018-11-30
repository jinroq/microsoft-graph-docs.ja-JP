---
title: skypeForBusinessPeerToPeerActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: ad3b409f3abc4cc9e7476825f9dbf5b7c2120d92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071477"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="f3e4d-103">skypeForBusinessPeerToPeerActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3e4d-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f3e4d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3e4d-104">Properties</span></span>

| <span data-ttu-id="f3e4d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3e4d-105">Property</span></span>          | <span data-ttu-id="f3e4d-106">型</span><span class="sxs-lookup"><span data-stu-id="f3e4d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f3e4d-107">im</span><span class="sxs-lookup"><span data-stu-id="f3e4d-107">im</span></span>                | <span data-ttu-id="f3e4d-108">Int64</span><span class="sxs-lookup"><span data-stu-id="f3e4d-108">Int64</span></span>  |
| <span data-ttu-id="f3e4d-109">audio</span><span class="sxs-lookup"><span data-stu-id="f3e4d-109">audio</span></span>             | <span data-ttu-id="f3e4d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f3e4d-110">Int64</span></span>  |
| <span data-ttu-id="f3e4d-111">video</span><span class="sxs-lookup"><span data-stu-id="f3e4d-111">video</span></span>             | <span data-ttu-id="f3e4d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f3e4d-112">Int64</span></span>  |
| <span data-ttu-id="f3e4d-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="f3e4d-113">appSharing</span></span>        | <span data-ttu-id="f3e4d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f3e4d-114">Int64</span></span>  |
| <span data-ttu-id="f3e4d-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="f3e4d-115">fileTransfer</span></span>      | <span data-ttu-id="f3e4d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f3e4d-116">Int64</span></span>  |
| <span data-ttu-id="f3e4d-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f3e4d-117">reportRefreshDate</span></span> | <span data-ttu-id="f3e4d-118">Date</span><span class="sxs-lookup"><span data-stu-id="f3e4d-118">Date</span></span>   |
| <span data-ttu-id="f3e4d-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="f3e4d-119">reportDate</span></span>        | <span data-ttu-id="f3e4d-120">Date</span><span class="sxs-lookup"><span data-stu-id="f3e4d-120">Date</span></span>   |
| <span data-ttu-id="f3e4d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f3e4d-121">reportPeriod</span></span>      | <span data-ttu-id="f3e4d-122">String</span><span class="sxs-lookup"><span data-stu-id="f3e4d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f3e4d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3e4d-123">JSON representation</span></span>

<span data-ttu-id="f3e4d-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f3e4d-124">The following is a JSON representation of the resource.</span></span>

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
