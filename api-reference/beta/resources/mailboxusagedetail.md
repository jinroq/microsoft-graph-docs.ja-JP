---
title: mailboxUsageDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 25cb41e38138a677bfc6636b035003bb8fc5858c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818012"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="5907d-103">mailboxUsageDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5907d-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5907d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5907d-104">Properties</span></span>

| <span data-ttu-id="5907d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5907d-105">Property</span></span>                        | <span data-ttu-id="5907d-106">種類</span><span class="sxs-lookup"><span data-stu-id="5907d-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="5907d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5907d-107">reportRefreshDate</span></span>               | <span data-ttu-id="5907d-108">日付</span><span class="sxs-lookup"><span data-stu-id="5907d-108">Date</span></span>    |
| <span data-ttu-id="5907d-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5907d-109">userPrincipalName</span></span>               | <span data-ttu-id="5907d-110">String</span><span class="sxs-lookup"><span data-stu-id="5907d-110">String</span></span>  |
| <span data-ttu-id="5907d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5907d-111">displayName</span></span>                     | <span data-ttu-id="5907d-112">String</span><span class="sxs-lookup"><span data-stu-id="5907d-112">String</span></span>  |
| <span data-ttu-id="5907d-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5907d-113">isDeleted</span></span>                       | <span data-ttu-id="5907d-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="5907d-114">Boolean</span></span> |
| <span data-ttu-id="5907d-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="5907d-115">deletedDate</span></span>                     | <span data-ttu-id="5907d-116">日付</span><span class="sxs-lookup"><span data-stu-id="5907d-116">Date</span></span>    |
| <span data-ttu-id="5907d-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="5907d-117">createdDate</span></span>                     | <span data-ttu-id="5907d-118">日付</span><span class="sxs-lookup"><span data-stu-id="5907d-118">Date</span></span>    |
| <span data-ttu-id="5907d-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="5907d-119">lastActivityDate</span></span>                | <span data-ttu-id="5907d-120">日付</span><span class="sxs-lookup"><span data-stu-id="5907d-120">Date</span></span>    |
| <span data-ttu-id="5907d-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="5907d-121">itemCount</span></span>                       | <span data-ttu-id="5907d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5907d-122">Int64</span></span>   |
| <span data-ttu-id="5907d-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="5907d-123">storageUsedInBytes</span></span>              | <span data-ttu-id="5907d-124">Int64</span><span class="sxs-lookup"><span data-stu-id="5907d-124">Int64</span></span>   |
| <span data-ttu-id="5907d-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="5907d-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="5907d-126">Int64</span><span class="sxs-lookup"><span data-stu-id="5907d-126">Int64</span></span>   |
| <span data-ttu-id="5907d-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="5907d-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="5907d-128">Int64</span><span class="sxs-lookup"><span data-stu-id="5907d-128">Int64</span></span>   |
| <span data-ttu-id="5907d-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="5907d-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="5907d-130">Int64</span><span class="sxs-lookup"><span data-stu-id="5907d-130">Int64</span></span>   |
| <span data-ttu-id="5907d-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5907d-131">reportPeriod</span></span>                    | <span data-ttu-id="5907d-132">String</span><span class="sxs-lookup"><span data-stu-id="5907d-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5907d-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5907d-133">JSON representation</span></span>

<span data-ttu-id="5907d-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5907d-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
