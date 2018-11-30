---
title: mailboxUsageStorage リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 8cc26c5d3cc30529857ed3273f8ee66c7373327a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068171"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="b5874-103">mailboxUsageStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5874-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b5874-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5874-104">Properties</span></span>

| <span data-ttu-id="b5874-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5874-105">Property</span></span>           | <span data-ttu-id="b5874-106">型</span><span class="sxs-lookup"><span data-stu-id="b5874-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="b5874-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b5874-107">reportRefreshDate</span></span>  | <span data-ttu-id="b5874-108">Date</span><span class="sxs-lookup"><span data-stu-id="b5874-108">Date</span></span>   |
| <span data-ttu-id="b5874-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="b5874-109">storageUsedInBytes</span></span> | <span data-ttu-id="b5874-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b5874-110">Int64</span></span>  |
| <span data-ttu-id="b5874-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="b5874-111">reportDate</span></span>         | <span data-ttu-id="b5874-112">Date</span><span class="sxs-lookup"><span data-stu-id="b5874-112">Date</span></span>   |
| <span data-ttu-id="b5874-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b5874-113">reportPeriod</span></span>       | <span data-ttu-id="b5874-114">String</span><span class="sxs-lookup"><span data-stu-id="b5874-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b5874-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5874-115">JSON representation</span></span>

<span data-ttu-id="b5874-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b5874-116">The following is a JSON representation of the resource.</span></span>

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
