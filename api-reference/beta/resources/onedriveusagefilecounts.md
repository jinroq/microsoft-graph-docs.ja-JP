---
title: oneDriveUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7e3a52d082d1acdd2e685008d60e6594615f57a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941024"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="af7e7-103">oneDriveUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="af7e7-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="af7e7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af7e7-104">Properties</span></span>

| <span data-ttu-id="af7e7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af7e7-105">Property</span></span>          | <span data-ttu-id="af7e7-106">種類</span><span class="sxs-lookup"><span data-stu-id="af7e7-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="af7e7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="af7e7-107">reportRefreshDate</span></span> | <span data-ttu-id="af7e7-108">日付</span><span class="sxs-lookup"><span data-stu-id="af7e7-108">Date</span></span>   |
| <span data-ttu-id="af7e7-109">ある</span><span class="sxs-lookup"><span data-stu-id="af7e7-109">siteType</span></span>          | <span data-ttu-id="af7e7-110">String</span><span class="sxs-lookup"><span data-stu-id="af7e7-110">String</span></span> |
| <span data-ttu-id="af7e7-111">total</span><span class="sxs-lookup"><span data-stu-id="af7e7-111">total</span></span>             | <span data-ttu-id="af7e7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="af7e7-112">Int64</span></span>  |
| <span data-ttu-id="af7e7-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="af7e7-113">active</span></span>            | <span data-ttu-id="af7e7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="af7e7-114">Int64</span></span>  |
| <span data-ttu-id="af7e7-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="af7e7-115">reportDate</span></span>        | <span data-ttu-id="af7e7-116">日付</span><span class="sxs-lookup"><span data-stu-id="af7e7-116">Date</span></span>   |
| <span data-ttu-id="af7e7-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="af7e7-117">reportPeriod</span></span>      | <span data-ttu-id="af7e7-118">String</span><span class="sxs-lookup"><span data-stu-id="af7e7-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="af7e7-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="af7e7-119">JSON representation</span></span>

<span data-ttu-id="af7e7-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="af7e7-120">The following is a JSON representation of the resource.</span></span>

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
