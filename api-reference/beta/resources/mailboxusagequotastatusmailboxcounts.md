---
title: mailboxUsageQuotaStatusMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921235"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="22b3b-103">mailboxUsageQuotaStatusMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22b3b-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="22b3b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22b3b-104">Properties</span></span>

| <span data-ttu-id="22b3b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22b3b-105">Property</span></span>              | <span data-ttu-id="22b3b-106">種類</span><span class="sxs-lookup"><span data-stu-id="22b3b-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="22b3b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="22b3b-107">reportRefreshDate</span></span>     | <span data-ttu-id="22b3b-108">日付</span><span class="sxs-lookup"><span data-stu-id="22b3b-108">Date</span></span>   |
| <span data-ttu-id="22b3b-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="22b3b-109">underLimit</span></span>            | <span data-ttu-id="22b3b-110">Int64</span><span class="sxs-lookup"><span data-stu-id="22b3b-110">Int64</span></span>  |
| <span data-ttu-id="22b3b-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="22b3b-111">warningIssued</span></span>         | <span data-ttu-id="22b3b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="22b3b-112">Int64</span></span>  |
| <span data-ttu-id="22b3b-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="22b3b-113">sendProhibited</span></span>        | <span data-ttu-id="22b3b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="22b3b-114">Int64</span></span>  |
| <span data-ttu-id="22b3b-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="22b3b-115">sendReceiveProhibited</span></span> | <span data-ttu-id="22b3b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="22b3b-116">Int64</span></span>  |
| <span data-ttu-id="22b3b-117">不確定</span><span class="sxs-lookup"><span data-stu-id="22b3b-117">indeterminate</span></span>         | <span data-ttu-id="22b3b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="22b3b-118">Int64</span></span>  |
| <span data-ttu-id="22b3b-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="22b3b-119">reportDate</span></span>            | <span data-ttu-id="22b3b-120">日付</span><span class="sxs-lookup"><span data-stu-id="22b3b-120">Date</span></span>   |
| <span data-ttu-id="22b3b-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="22b3b-121">reportPeriod</span></span>          | <span data-ttu-id="22b3b-122">String</span><span class="sxs-lookup"><span data-stu-id="22b3b-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="22b3b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22b3b-123">JSON representation</span></span>

<span data-ttu-id="22b3b-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="22b3b-124">The following is a JSON representation of the resource.</span></span>

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
