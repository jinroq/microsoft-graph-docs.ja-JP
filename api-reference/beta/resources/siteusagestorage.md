---
title: siteの種類ストレージリソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583201"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="0f0da-103">siteの種類ストレージリソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f0da-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0f0da-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f0da-104">Properties</span></span>

| <span data-ttu-id="0f0da-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f0da-105">Property</span></span>           | <span data-ttu-id="0f0da-106">型</span><span class="sxs-lookup"><span data-stu-id="0f0da-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="0f0da-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="0f0da-107">reportRefreshDate</span></span>  | <span data-ttu-id="0f0da-108">Date</span><span class="sxs-lookup"><span data-stu-id="0f0da-108">Date</span></span>   |
| <span data-ttu-id="0f0da-109">sitetype</span><span class="sxs-lookup"><span data-stu-id="0f0da-109">siteType</span></span>           | <span data-ttu-id="0f0da-110">String</span><span class="sxs-lookup"><span data-stu-id="0f0da-110">String</span></span> |
| <span data-ttu-id="0f0da-111">storageused inbytes</span><span class="sxs-lookup"><span data-stu-id="0f0da-111">storageUsedInBytes</span></span> | <span data-ttu-id="0f0da-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0f0da-112">Int64</span></span>  |
| <span data-ttu-id="0f0da-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="0f0da-113">reportDate</span></span>         | <span data-ttu-id="0f0da-114">Date</span><span class="sxs-lookup"><span data-stu-id="0f0da-114">Date</span></span>   |
| <span data-ttu-id="0f0da-115">reportperiod</span><span class="sxs-lookup"><span data-stu-id="0f0da-115">reportPeriod</span></span>       | <span data-ttu-id="0f0da-116">String</span><span class="sxs-lookup"><span data-stu-id="0f0da-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f0da-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f0da-117">JSON representation</span></span>

<span data-ttu-id="0f0da-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0f0da-118">The following is a JSON representation of the resource.</span></span>

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
