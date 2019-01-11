---
title: mailboxUsageQuotaStatusMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: b87bb1ce91626f9151d294e2243bba72ba72346b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835224"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="0ef37-103">mailboxUsageQuotaStatusMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ef37-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0ef37-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ef37-104">Properties</span></span>

| <span data-ttu-id="0ef37-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ef37-105">Property</span></span>              | <span data-ttu-id="0ef37-106">種類</span><span class="sxs-lookup"><span data-stu-id="0ef37-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="0ef37-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0ef37-107">reportRefreshDate</span></span>     | <span data-ttu-id="0ef37-108">日付</span><span class="sxs-lookup"><span data-stu-id="0ef37-108">Date</span></span>   |
| <span data-ttu-id="0ef37-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="0ef37-109">underLimit</span></span>            | <span data-ttu-id="0ef37-110">Int64</span><span class="sxs-lookup"><span data-stu-id="0ef37-110">Int64</span></span>  |
| <span data-ttu-id="0ef37-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="0ef37-111">warningIssued</span></span>         | <span data-ttu-id="0ef37-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0ef37-112">Int64</span></span>  |
| <span data-ttu-id="0ef37-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="0ef37-113">sendProhibited</span></span>        | <span data-ttu-id="0ef37-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0ef37-114">Int64</span></span>  |
| <span data-ttu-id="0ef37-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="0ef37-115">sendReceiveProhibited</span></span> | <span data-ttu-id="0ef37-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0ef37-116">Int64</span></span>  |
| <span data-ttu-id="0ef37-117">不確定</span><span class="sxs-lookup"><span data-stu-id="0ef37-117">indeterminate</span></span>         | <span data-ttu-id="0ef37-118">Int64</span><span class="sxs-lookup"><span data-stu-id="0ef37-118">Int64</span></span>  |
| <span data-ttu-id="0ef37-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="0ef37-119">reportDate</span></span>            | <span data-ttu-id="0ef37-120">日付</span><span class="sxs-lookup"><span data-stu-id="0ef37-120">Date</span></span>   |
| <span data-ttu-id="0ef37-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0ef37-121">reportPeriod</span></span>          | <span data-ttu-id="0ef37-122">String</span><span class="sxs-lookup"><span data-stu-id="0ef37-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ef37-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ef37-123">JSON representation</span></span>

<span data-ttu-id="0ef37-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0ef37-124">The following is a JSON representation of the resource.</span></span>

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
