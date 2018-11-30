---
title: mailboxUsageDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: af49fac7c6286c7e9f9ce1e6d7ffdede225b4072
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068129"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="50e95-103">mailboxUsageDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50e95-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="50e95-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50e95-104">Properties</span></span>

| <span data-ttu-id="50e95-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50e95-105">Property</span></span>                        | <span data-ttu-id="50e95-106">型</span><span class="sxs-lookup"><span data-stu-id="50e95-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="50e95-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="50e95-107">reportRefreshDate</span></span>               | <span data-ttu-id="50e95-108">Date</span><span class="sxs-lookup"><span data-stu-id="50e95-108">Date</span></span>    |
| <span data-ttu-id="50e95-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="50e95-109">userPrincipalName</span></span>               | <span data-ttu-id="50e95-110">String</span><span class="sxs-lookup"><span data-stu-id="50e95-110">String</span></span>  |
| <span data-ttu-id="50e95-111">displayName</span><span class="sxs-lookup"><span data-stu-id="50e95-111">displayName</span></span>                     | <span data-ttu-id="50e95-112">String</span><span class="sxs-lookup"><span data-stu-id="50e95-112">String</span></span>  |
| <span data-ttu-id="50e95-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="50e95-113">isDeleted</span></span>                       | <span data-ttu-id="50e95-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="50e95-114">Boolean</span></span> |
| <span data-ttu-id="50e95-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="50e95-115">deletedDate</span></span>                     | <span data-ttu-id="50e95-116">Date</span><span class="sxs-lookup"><span data-stu-id="50e95-116">Date</span></span>    |
| <span data-ttu-id="50e95-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="50e95-117">createdDate</span></span>                     | <span data-ttu-id="50e95-118">Date</span><span class="sxs-lookup"><span data-stu-id="50e95-118">Date</span></span>    |
| <span data-ttu-id="50e95-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="50e95-119">lastActivityDate</span></span>                | <span data-ttu-id="50e95-120">Date</span><span class="sxs-lookup"><span data-stu-id="50e95-120">Date</span></span>    |
| <span data-ttu-id="50e95-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="50e95-121">itemCount</span></span>                       | <span data-ttu-id="50e95-122">Int64</span><span class="sxs-lookup"><span data-stu-id="50e95-122">Int64</span></span>   |
| <span data-ttu-id="50e95-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="50e95-123">storageUsedInBytes</span></span>              | <span data-ttu-id="50e95-124">Int64</span><span class="sxs-lookup"><span data-stu-id="50e95-124">Int64</span></span>   |
| <span data-ttu-id="50e95-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="50e95-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="50e95-126">Int64</span><span class="sxs-lookup"><span data-stu-id="50e95-126">Int64</span></span>   |
| <span data-ttu-id="50e95-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="50e95-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="50e95-128">Int64</span><span class="sxs-lookup"><span data-stu-id="50e95-128">Int64</span></span>   |
| <span data-ttu-id="50e95-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="50e95-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="50e95-130">Int64</span><span class="sxs-lookup"><span data-stu-id="50e95-130">Int64</span></span>   |
| <span data-ttu-id="50e95-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="50e95-131">reportPeriod</span></span>                    | <span data-ttu-id="50e95-132">String</span><span class="sxs-lookup"><span data-stu-id="50e95-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="50e95-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50e95-133">JSON representation</span></span>

<span data-ttu-id="50e95-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="50e95-134">The following is a JSON representation of the resource.</span></span>

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
