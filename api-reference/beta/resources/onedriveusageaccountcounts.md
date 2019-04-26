---
title: onedrive のアカウント数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: dd70875c272f63a1c9a7988c001225c2d200e0c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554850"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="c5a4f-103">onedrive のアカウント数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5a4f-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c5a4f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5a4f-104">Properties</span></span>

| <span data-ttu-id="c5a4f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5a4f-105">Property</span></span>          | <span data-ttu-id="c5a4f-106">型</span><span class="sxs-lookup"><span data-stu-id="c5a4f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c5a4f-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="c5a4f-107">reportRefreshDate</span></span> | <span data-ttu-id="c5a4f-108">Date</span><span class="sxs-lookup"><span data-stu-id="c5a4f-108">Date</span></span>   |
| <span data-ttu-id="c5a4f-109">sitetype</span><span class="sxs-lookup"><span data-stu-id="c5a4f-109">siteType</span></span>          | <span data-ttu-id="c5a4f-110">String</span><span class="sxs-lookup"><span data-stu-id="c5a4f-110">String</span></span> |
| <span data-ttu-id="c5a4f-111">total</span><span class="sxs-lookup"><span data-stu-id="c5a4f-111">total</span></span>             | <span data-ttu-id="c5a4f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c5a4f-112">Int64</span></span>  |
| <span data-ttu-id="c5a4f-113">active</span><span class="sxs-lookup"><span data-stu-id="c5a4f-113">active</span></span>            | <span data-ttu-id="c5a4f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c5a4f-114">Int64</span></span>  |
| <span data-ttu-id="c5a4f-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="c5a4f-115">reportDate</span></span>        | <span data-ttu-id="c5a4f-116">Date</span><span class="sxs-lookup"><span data-stu-id="c5a4f-116">Date</span></span>   |
| <span data-ttu-id="c5a4f-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="c5a4f-117">reportPeriod</span></span>      | <span data-ttu-id="c5a4f-118">String</span><span class="sxs-lookup"><span data-stu-id="c5a4f-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5a4f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5a4f-119">JSON representation</span></span>

<span data-ttu-id="c5a4f-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5a4f-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
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
