---
title: mailboxUsageMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 4e18993590d6de893b78db511037eb28ec1cc0cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814813"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="f4b88-103">mailboxUsageMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4b88-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f4b88-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4b88-104">Properties</span></span>

| <span data-ttu-id="f4b88-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4b88-105">Property</span></span>          | <span data-ttu-id="f4b88-106">種類</span><span class="sxs-lookup"><span data-stu-id="f4b88-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f4b88-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f4b88-107">reportRefreshDate</span></span> | <span data-ttu-id="f4b88-108">日付</span><span class="sxs-lookup"><span data-stu-id="f4b88-108">Date</span></span>   |
| <span data-ttu-id="f4b88-109">total</span><span class="sxs-lookup"><span data-stu-id="f4b88-109">total</span></span>             | <span data-ttu-id="f4b88-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f4b88-110">Int64</span></span>  |
| <span data-ttu-id="f4b88-111">アクティブです</span><span class="sxs-lookup"><span data-stu-id="f4b88-111">active</span></span>            | <span data-ttu-id="f4b88-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f4b88-112">Int64</span></span>  |
| <span data-ttu-id="f4b88-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="f4b88-113">reportDate</span></span>        | <span data-ttu-id="f4b88-114">日付</span><span class="sxs-lookup"><span data-stu-id="f4b88-114">Date</span></span>   |
| <span data-ttu-id="f4b88-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f4b88-115">reportPeriod</span></span>      | <span data-ttu-id="f4b88-116">String</span><span class="sxs-lookup"><span data-stu-id="f4b88-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4b88-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4b88-117">JSON representation</span></span>

<span data-ttu-id="f4b88-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4b88-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
