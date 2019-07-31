---
title: mailboxUsageQuotaStatusMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1e8fafe9a3cdce4519cf5755337b016fa587cd06
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966903"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="387bf-103">mailboxUsageQuotaStatusMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="387bf-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="387bf-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="387bf-104">Properties</span></span>

| <span data-ttu-id="387bf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="387bf-105">Property</span></span>              | <span data-ttu-id="387bf-106">型</span><span class="sxs-lookup"><span data-stu-id="387bf-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="387bf-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="387bf-107">reportRefreshDate</span></span>     | <span data-ttu-id="387bf-108">日付</span><span class="sxs-lookup"><span data-stu-id="387bf-108">Date</span></span>   |
| <span data-ttu-id="387bf-109">過小制限</span><span class="sxs-lookup"><span data-stu-id="387bf-109">underLimit</span></span>            | <span data-ttu-id="387bf-110">Int64</span><span class="sxs-lookup"><span data-stu-id="387bf-110">Int64</span></span>  |
| <span data-ttu-id="387bf-111">警告の発行</span><span class="sxs-lookup"><span data-stu-id="387bf-111">warningIssued</span></span>         | <span data-ttu-id="387bf-112">Int64</span><span class="sxs-lookup"><span data-stu-id="387bf-112">Int64</span></span>  |
| <span data-ttu-id="387bf-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="387bf-113">sendProhibited</span></span>        | <span data-ttu-id="387bf-114">Int64</span><span class="sxs-lookup"><span data-stu-id="387bf-114">Int64</span></span>  |
| <span data-ttu-id="387bf-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="387bf-115">sendReceiveProhibited</span></span> | <span data-ttu-id="387bf-116">Int64</span><span class="sxs-lookup"><span data-stu-id="387bf-116">Int64</span></span>  |
| <span data-ttu-id="387bf-117">不特定</span><span class="sxs-lookup"><span data-stu-id="387bf-117">indeterminate</span></span>         | <span data-ttu-id="387bf-118">Int64</span><span class="sxs-lookup"><span data-stu-id="387bf-118">Int64</span></span>  |
| <span data-ttu-id="387bf-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="387bf-119">reportDate</span></span>            | <span data-ttu-id="387bf-120">日付</span><span class="sxs-lookup"><span data-stu-id="387bf-120">Date</span></span>   |
| <span data-ttu-id="387bf-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="387bf-121">reportPeriod</span></span>          | <span data-ttu-id="387bf-122">String</span><span class="sxs-lookup"><span data-stu-id="387bf-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="387bf-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="387bf-123">JSON representation</span></span>

<span data-ttu-id="387bf-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="387bf-124">The following is a JSON representation of the resource.</span></span>

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
