---
title: mailboxUsageMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e9da6a72c3c2d79323041e683702a7af2e4699c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941311"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="a6aab-103">mailboxUsageMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6aab-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a6aab-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6aab-104">Properties</span></span>

| <span data-ttu-id="a6aab-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6aab-105">Property</span></span>          | <span data-ttu-id="a6aab-106">種類</span><span class="sxs-lookup"><span data-stu-id="a6aab-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a6aab-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a6aab-107">reportRefreshDate</span></span> | <span data-ttu-id="a6aab-108">日付</span><span class="sxs-lookup"><span data-stu-id="a6aab-108">Date</span></span>   |
| <span data-ttu-id="a6aab-109">total</span><span class="sxs-lookup"><span data-stu-id="a6aab-109">total</span></span>             | <span data-ttu-id="a6aab-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a6aab-110">Int64</span></span>  |
| <span data-ttu-id="a6aab-111">アクティブです</span><span class="sxs-lookup"><span data-stu-id="a6aab-111">active</span></span>            | <span data-ttu-id="a6aab-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a6aab-112">Int64</span></span>  |
| <span data-ttu-id="a6aab-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="a6aab-113">reportDate</span></span>        | <span data-ttu-id="a6aab-114">日付</span><span class="sxs-lookup"><span data-stu-id="a6aab-114">Date</span></span>   |
| <span data-ttu-id="a6aab-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a6aab-115">reportPeriod</span></span>      | <span data-ttu-id="a6aab-116">String</span><span class="sxs-lookup"><span data-stu-id="a6aab-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6aab-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6aab-117">JSON representation</span></span>

<span data-ttu-id="a6aab-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6aab-118">The following is a JSON representation of the resource.</span></span>

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
