---
title: mailboxUsageQuotaStatusMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: ac6c597cad9d28f985da97d6f55a5726ebbf491e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069374"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="91ab1-103">mailboxUsageQuotaStatusMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91ab1-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="91ab1-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91ab1-104">Properties</span></span>

| <span data-ttu-id="91ab1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91ab1-105">Property</span></span>              | <span data-ttu-id="91ab1-106">型</span><span class="sxs-lookup"><span data-stu-id="91ab1-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="91ab1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="91ab1-107">reportRefreshDate</span></span>     | <span data-ttu-id="91ab1-108">Date</span><span class="sxs-lookup"><span data-stu-id="91ab1-108">Date</span></span>   |
| <span data-ttu-id="91ab1-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="91ab1-109">underLimit</span></span>            | <span data-ttu-id="91ab1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="91ab1-110">Int64</span></span>  |
| <span data-ttu-id="91ab1-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="91ab1-111">warningIssued</span></span>         | <span data-ttu-id="91ab1-112">Int64</span><span class="sxs-lookup"><span data-stu-id="91ab1-112">Int64</span></span>  |
| <span data-ttu-id="91ab1-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="91ab1-113">sendProhibited</span></span>        | <span data-ttu-id="91ab1-114">Int64</span><span class="sxs-lookup"><span data-stu-id="91ab1-114">Int64</span></span>  |
| <span data-ttu-id="91ab1-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="91ab1-115">sendReceiveProhibited</span></span> | <span data-ttu-id="91ab1-116">Int64</span><span class="sxs-lookup"><span data-stu-id="91ab1-116">Int64</span></span>  |
| <span data-ttu-id="91ab1-117">不確定</span><span class="sxs-lookup"><span data-stu-id="91ab1-117">indeterminate</span></span>         | <span data-ttu-id="91ab1-118">Int64</span><span class="sxs-lookup"><span data-stu-id="91ab1-118">Int64</span></span>  |
| <span data-ttu-id="91ab1-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="91ab1-119">reportDate</span></span>            | <span data-ttu-id="91ab1-120">Date</span><span class="sxs-lookup"><span data-stu-id="91ab1-120">Date</span></span>   |
| <span data-ttu-id="91ab1-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="91ab1-121">reportPeriod</span></span>          | <span data-ttu-id="91ab1-122">String</span><span class="sxs-lookup"><span data-stu-id="91ab1-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91ab1-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91ab1-123">JSON representation</span></span>

<span data-ttu-id="91ab1-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91ab1-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
