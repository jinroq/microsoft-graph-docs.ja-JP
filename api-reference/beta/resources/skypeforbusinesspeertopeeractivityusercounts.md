---
title: skypeForBusinessPeerToPeerActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 619e581fcdd25dda10be7210aefe5db8e4dcd8b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503885"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="1c215-103">skypeForBusinessPeerToPeerActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c215-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1c215-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c215-104">Properties</span></span>

| <span data-ttu-id="1c215-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c215-105">Property</span></span>          | <span data-ttu-id="1c215-106">型</span><span class="sxs-lookup"><span data-stu-id="1c215-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1c215-107">im</span><span class="sxs-lookup"><span data-stu-id="1c215-107">im</span></span>                | <span data-ttu-id="1c215-108">Int64</span><span class="sxs-lookup"><span data-stu-id="1c215-108">Int64</span></span>  |
| <span data-ttu-id="1c215-109">audio</span><span class="sxs-lookup"><span data-stu-id="1c215-109">audio</span></span>             | <span data-ttu-id="1c215-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1c215-110">Int64</span></span>  |
| <span data-ttu-id="1c215-111">video</span><span class="sxs-lookup"><span data-stu-id="1c215-111">video</span></span>             | <span data-ttu-id="1c215-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1c215-112">Int64</span></span>  |
| <span data-ttu-id="1c215-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="1c215-113">appSharing</span></span>        | <span data-ttu-id="1c215-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1c215-114">Int64</span></span>  |
| <span data-ttu-id="1c215-115">filetransfer</span><span class="sxs-lookup"><span data-stu-id="1c215-115">fileTransfer</span></span>      | <span data-ttu-id="1c215-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1c215-116">Int64</span></span>  |
| <span data-ttu-id="1c215-117">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="1c215-117">reportRefreshDate</span></span> | <span data-ttu-id="1c215-118">Date</span><span class="sxs-lookup"><span data-stu-id="1c215-118">Date</span></span>   |
| <span data-ttu-id="1c215-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="1c215-119">reportDate</span></span>        | <span data-ttu-id="1c215-120">Date</span><span class="sxs-lookup"><span data-stu-id="1c215-120">Date</span></span>   |
| <span data-ttu-id="1c215-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="1c215-121">reportPeriod</span></span>      | <span data-ttu-id="1c215-122">String</span><span class="sxs-lookup"><span data-stu-id="1c215-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c215-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c215-123">JSON representation</span></span>

<span data-ttu-id="1c215-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c215-124">The following is a JSON representation of the resource.</span></span>

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
