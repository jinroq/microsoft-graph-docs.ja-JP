---
title: oneDriveUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: bf0b46c01167ac1d103b54386aabd981d99116cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009392"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="b81d4-103">oneDriveUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b81d4-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b81d4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b81d4-104">Properties</span></span>

| <span data-ttu-id="b81d4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b81d4-105">Property</span></span>          | <span data-ttu-id="b81d4-106">型</span><span class="sxs-lookup"><span data-stu-id="b81d4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b81d4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b81d4-107">reportRefreshDate</span></span> | <span data-ttu-id="b81d4-108">日付</span><span class="sxs-lookup"><span data-stu-id="b81d4-108">Date</span></span>   |
| <span data-ttu-id="b81d4-109">siteType</span><span class="sxs-lookup"><span data-stu-id="b81d4-109">siteType</span></span>          | <span data-ttu-id="b81d4-110">String</span><span class="sxs-lookup"><span data-stu-id="b81d4-110">String</span></span> |
| <span data-ttu-id="b81d4-111">total</span><span class="sxs-lookup"><span data-stu-id="b81d4-111">total</span></span>             | <span data-ttu-id="b81d4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b81d4-112">Int64</span></span>  |
| <span data-ttu-id="b81d4-113">active</span><span class="sxs-lookup"><span data-stu-id="b81d4-113">active</span></span>            | <span data-ttu-id="b81d4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b81d4-114">Int64</span></span>  |
| <span data-ttu-id="b81d4-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="b81d4-115">reportDate</span></span>        | <span data-ttu-id="b81d4-116">日付</span><span class="sxs-lookup"><span data-stu-id="b81d4-116">Date</span></span>   |
| <span data-ttu-id="b81d4-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b81d4-117">reportPeriod</span></span>      | <span data-ttu-id="b81d4-118">String</span><span class="sxs-lookup"><span data-stu-id="b81d4-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b81d4-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b81d4-119">JSON representation</span></span>

<span data-ttu-id="b81d4-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b81d4-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
