---
title: oneDriveUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: ec428179cb35755e545aded70929eccd9d558fec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829534"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="0affa-103">oneDriveUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0affa-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0affa-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0affa-104">Properties</span></span>

| <span data-ttu-id="0affa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0affa-105">Property</span></span>          | <span data-ttu-id="0affa-106">種類</span><span class="sxs-lookup"><span data-stu-id="0affa-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0affa-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0affa-107">reportRefreshDate</span></span> | <span data-ttu-id="0affa-108">日付</span><span class="sxs-lookup"><span data-stu-id="0affa-108">Date</span></span>   |
| <span data-ttu-id="0affa-109">ある</span><span class="sxs-lookup"><span data-stu-id="0affa-109">siteType</span></span>          | <span data-ttu-id="0affa-110">String</span><span class="sxs-lookup"><span data-stu-id="0affa-110">String</span></span> |
| <span data-ttu-id="0affa-111">total</span><span class="sxs-lookup"><span data-stu-id="0affa-111">total</span></span>             | <span data-ttu-id="0affa-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0affa-112">Int64</span></span>  |
| <span data-ttu-id="0affa-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="0affa-113">active</span></span>            | <span data-ttu-id="0affa-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0affa-114">Int64</span></span>  |
| <span data-ttu-id="0affa-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="0affa-115">reportDate</span></span>        | <span data-ttu-id="0affa-116">日付</span><span class="sxs-lookup"><span data-stu-id="0affa-116">Date</span></span>   |
| <span data-ttu-id="0affa-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0affa-117">reportPeriod</span></span>      | <span data-ttu-id="0affa-118">String</span><span class="sxs-lookup"><span data-stu-id="0affa-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0affa-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0affa-119">JSON representation</span></span>

<span data-ttu-id="0affa-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0affa-120">The following is a JSON representation of the resource.</span></span>

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
