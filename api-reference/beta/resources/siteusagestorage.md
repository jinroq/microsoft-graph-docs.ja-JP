---
title: Siteの種類ストレージリソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1ed15d4efb1c9a0fa81fdd79faeb9542d8093aab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008230"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="c7d0d-103">Siteの種類ストレージリソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7d0d-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c7d0d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7d0d-104">Properties</span></span>

| <span data-ttu-id="c7d0d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7d0d-105">Property</span></span>           | <span data-ttu-id="c7d0d-106">型</span><span class="sxs-lookup"><span data-stu-id="c7d0d-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="c7d0d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c7d0d-107">reportRefreshDate</span></span>  | <span data-ttu-id="c7d0d-108">日付</span><span class="sxs-lookup"><span data-stu-id="c7d0d-108">Date</span></span>   |
| <span data-ttu-id="c7d0d-109">siteType</span><span class="sxs-lookup"><span data-stu-id="c7d0d-109">siteType</span></span>           | <span data-ttu-id="c7d0d-110">String</span><span class="sxs-lookup"><span data-stu-id="c7d0d-110">String</span></span> |
| <span data-ttu-id="c7d0d-111">Storageused Inbytes</span><span class="sxs-lookup"><span data-stu-id="c7d0d-111">storageUsedInBytes</span></span> | <span data-ttu-id="c7d0d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c7d0d-112">Int64</span></span>  |
| <span data-ttu-id="c7d0d-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="c7d0d-113">reportDate</span></span>         | <span data-ttu-id="c7d0d-114">日付</span><span class="sxs-lookup"><span data-stu-id="c7d0d-114">Date</span></span>   |
| <span data-ttu-id="c7d0d-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c7d0d-115">reportPeriod</span></span>       | <span data-ttu-id="c7d0d-116">String</span><span class="sxs-lookup"><span data-stu-id="c7d0d-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7d0d-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7d0d-117">JSON representation</span></span>

<span data-ttu-id="c7d0d-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7d0d-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
