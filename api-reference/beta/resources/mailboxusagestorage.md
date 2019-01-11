---
title: mailboxUsageStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: dcabfab0e8a64f2d74442f7d7464708501a59b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840741"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="62ff9-103">mailboxUsageStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62ff9-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="62ff9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62ff9-104">Properties</span></span>

| <span data-ttu-id="62ff9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62ff9-105">Property</span></span>           | <span data-ttu-id="62ff9-106">種類</span><span class="sxs-lookup"><span data-stu-id="62ff9-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="62ff9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="62ff9-107">reportRefreshDate</span></span>  | <span data-ttu-id="62ff9-108">日付</span><span class="sxs-lookup"><span data-stu-id="62ff9-108">Date</span></span>   |
| <span data-ttu-id="62ff9-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="62ff9-109">storageUsedInBytes</span></span> | <span data-ttu-id="62ff9-110">Int64</span><span class="sxs-lookup"><span data-stu-id="62ff9-110">Int64</span></span>  |
| <span data-ttu-id="62ff9-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="62ff9-111">reportDate</span></span>         | <span data-ttu-id="62ff9-112">日付</span><span class="sxs-lookup"><span data-stu-id="62ff9-112">Date</span></span>   |
| <span data-ttu-id="62ff9-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="62ff9-113">reportPeriod</span></span>       | <span data-ttu-id="62ff9-114">String</span><span class="sxs-lookup"><span data-stu-id="62ff9-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62ff9-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62ff9-115">JSON representation</span></span>

<span data-ttu-id="62ff9-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62ff9-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
