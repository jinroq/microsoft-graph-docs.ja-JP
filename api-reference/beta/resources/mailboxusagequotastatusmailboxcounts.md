---
title: mailboxUsageQuotaStatusMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457131"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="515dd-103">mailboxUsageQuotaStatusMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="515dd-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="515dd-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="515dd-104">Properties</span></span>

| <span data-ttu-id="515dd-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="515dd-105">Property</span></span>              | <span data-ttu-id="515dd-106">型</span><span class="sxs-lookup"><span data-stu-id="515dd-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="515dd-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="515dd-107">reportRefreshDate</span></span>     | <span data-ttu-id="515dd-108">日付</span><span class="sxs-lookup"><span data-stu-id="515dd-108">Date</span></span>   |
| <span data-ttu-id="515dd-109">過小制限</span><span class="sxs-lookup"><span data-stu-id="515dd-109">underLimit</span></span>            | <span data-ttu-id="515dd-110">Int64</span><span class="sxs-lookup"><span data-stu-id="515dd-110">Int64</span></span>  |
| <span data-ttu-id="515dd-111">警告の発行</span><span class="sxs-lookup"><span data-stu-id="515dd-111">warningIssued</span></span>         | <span data-ttu-id="515dd-112">Int64</span><span class="sxs-lookup"><span data-stu-id="515dd-112">Int64</span></span>  |
| <span data-ttu-id="515dd-113">sendprohibited</span><span class="sxs-lookup"><span data-stu-id="515dd-113">sendProhibited</span></span>        | <span data-ttu-id="515dd-114">Int64</span><span class="sxs-lookup"><span data-stu-id="515dd-114">Int64</span></span>  |
| <span data-ttu-id="515dd-115">sendreceiveprohibited</span><span class="sxs-lookup"><span data-stu-id="515dd-115">sendReceiveProhibited</span></span> | <span data-ttu-id="515dd-116">Int64</span><span class="sxs-lookup"><span data-stu-id="515dd-116">Int64</span></span>  |
| <span data-ttu-id="515dd-117">不特定</span><span class="sxs-lookup"><span data-stu-id="515dd-117">indeterminate</span></span>         | <span data-ttu-id="515dd-118">Int64</span><span class="sxs-lookup"><span data-stu-id="515dd-118">Int64</span></span>  |
| <span data-ttu-id="515dd-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="515dd-119">reportDate</span></span>            | <span data-ttu-id="515dd-120">日付</span><span class="sxs-lookup"><span data-stu-id="515dd-120">Date</span></span>   |
| <span data-ttu-id="515dd-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="515dd-121">reportPeriod</span></span>          | <span data-ttu-id="515dd-122">String</span><span class="sxs-lookup"><span data-stu-id="515dd-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="515dd-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="515dd-123">JSON representation</span></span>

<span data-ttu-id="515dd-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="515dd-124">The following is a JSON representation of the resource.</span></span>

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
