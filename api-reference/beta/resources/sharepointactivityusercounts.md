---
title: sharePointActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 97fbcb8c611bd497a7bf6613a5bde53738aff5e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008454"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="76a7f-103">sharePointActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76a7f-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="76a7f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76a7f-104">Properties</span></span>

| <span data-ttu-id="76a7f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76a7f-105">Property</span></span>          | <span data-ttu-id="76a7f-106">型</span><span class="sxs-lookup"><span data-stu-id="76a7f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="76a7f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="76a7f-107">reportRefreshDate</span></span> | <span data-ttu-id="76a7f-108">日付</span><span class="sxs-lookup"><span data-stu-id="76a7f-108">Date</span></span>   |
| <span data-ttu-id="76a7f-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="76a7f-109">visitedPage</span></span>       | <span data-ttu-id="76a7f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="76a7f-110">Int64</span></span>  |
| <span data-ttu-id="76a7f-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="76a7f-111">viewedOrEdited</span></span>    | <span data-ttu-id="76a7f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="76a7f-112">Int64</span></span>  |
| <span data-ttu-id="76a7f-113">同期</span><span class="sxs-lookup"><span data-stu-id="76a7f-113">synced</span></span>            | <span data-ttu-id="76a7f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="76a7f-114">Int64</span></span>  |
| <span data-ttu-id="76a7f-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="76a7f-115">sharedInternally</span></span>  | <span data-ttu-id="76a7f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="76a7f-116">Int64</span></span>  |
| <span data-ttu-id="76a7f-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="76a7f-117">sharedExternally</span></span>  | <span data-ttu-id="76a7f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="76a7f-118">Int64</span></span>  |
| <span data-ttu-id="76a7f-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="76a7f-119">reportDate</span></span>        | <span data-ttu-id="76a7f-120">日付</span><span class="sxs-lookup"><span data-stu-id="76a7f-120">Date</span></span>   |
| <span data-ttu-id="76a7f-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="76a7f-121">reportPeriod</span></span>      | <span data-ttu-id="76a7f-122">String</span><span class="sxs-lookup"><span data-stu-id="76a7f-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76a7f-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76a7f-123">JSON representation</span></span>

<span data-ttu-id="76a7f-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76a7f-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPage": 1024, 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
