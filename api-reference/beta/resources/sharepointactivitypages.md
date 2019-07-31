---
title: sharePointActivityPages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: a3d54e388d5a43489cac285a481b6ca1137aeba5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965097"
---
# <a name="sharepointactivitypages-resource-type"></a><span data-ttu-id="e5698-103">sharePointActivityPages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5698-103">sharePointActivityPages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e5698-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5698-104">Properties</span></span>

| <span data-ttu-id="e5698-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5698-105">Property</span></span>          | <span data-ttu-id="e5698-106">型</span><span class="sxs-lookup"><span data-stu-id="e5698-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e5698-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e5698-107">reportRefreshDate</span></span> | <span data-ttu-id="e5698-108">日付</span><span class="sxs-lookup"><span data-stu-id="e5698-108">Date</span></span>   |
| <span data-ttu-id="e5698-109">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="e5698-109">visitedPageCount</span></span>  | <span data-ttu-id="e5698-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e5698-110">Int64</span></span>  |
| <span data-ttu-id="e5698-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="e5698-111">reportDate</span></span>        | <span data-ttu-id="e5698-112">日付</span><span class="sxs-lookup"><span data-stu-id="e5698-112">Date</span></span>   |
| <span data-ttu-id="e5698-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e5698-113">reportPeriod</span></span>      | <span data-ttu-id="e5698-114">String</span><span class="sxs-lookup"><span data-stu-id="e5698-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e5698-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5698-115">JSON representation</span></span>

<span data-ttu-id="e5698-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e5698-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPageCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
