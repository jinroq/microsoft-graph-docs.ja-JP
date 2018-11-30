---
title: mailboxUsageMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 8f5b5080255a12c474cb8ab5c078c4f991089c31
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073473"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="b37de-103">mailboxUsageMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b37de-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b37de-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b37de-104">Properties</span></span>

| <span data-ttu-id="b37de-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b37de-105">Property</span></span>          | <span data-ttu-id="b37de-106">型</span><span class="sxs-lookup"><span data-stu-id="b37de-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b37de-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b37de-107">reportRefreshDate</span></span> | <span data-ttu-id="b37de-108">Date</span><span class="sxs-lookup"><span data-stu-id="b37de-108">Date</span></span>   |
| <span data-ttu-id="b37de-109">total</span><span class="sxs-lookup"><span data-stu-id="b37de-109">total</span></span>             | <span data-ttu-id="b37de-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b37de-110">Int64</span></span>  |
| <span data-ttu-id="b37de-111">アクティブです</span><span class="sxs-lookup"><span data-stu-id="b37de-111">active</span></span>            | <span data-ttu-id="b37de-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b37de-112">Int64</span></span>  |
| <span data-ttu-id="b37de-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="b37de-113">reportDate</span></span>        | <span data-ttu-id="b37de-114">Date</span><span class="sxs-lookup"><span data-stu-id="b37de-114">Date</span></span>   |
| <span data-ttu-id="b37de-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b37de-115">reportPeriod</span></span>      | <span data-ttu-id="b37de-116">String</span><span class="sxs-lookup"><span data-stu-id="b37de-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b37de-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b37de-117">JSON representation</span></span>

<span data-ttu-id="b37de-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b37de-118">The following is a JSON representation of the resource.</span></span>

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
