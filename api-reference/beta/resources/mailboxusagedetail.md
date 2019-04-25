---
title: mailboxUsageDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63b4b997a0ae559338fffd2acfabaa35dcc306e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581269"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="36b44-103">mailboxUsageDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="36b44-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="36b44-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36b44-104">Properties</span></span>

| <span data-ttu-id="36b44-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36b44-105">Property</span></span>                        | <span data-ttu-id="36b44-106">型</span><span class="sxs-lookup"><span data-stu-id="36b44-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="36b44-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="36b44-107">reportRefreshDate</span></span>               | <span data-ttu-id="36b44-108">Date</span><span class="sxs-lookup"><span data-stu-id="36b44-108">Date</span></span>    |
| <span data-ttu-id="36b44-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="36b44-109">userPrincipalName</span></span>               | <span data-ttu-id="36b44-110">String</span><span class="sxs-lookup"><span data-stu-id="36b44-110">String</span></span>  |
| <span data-ttu-id="36b44-111">displayName</span><span class="sxs-lookup"><span data-stu-id="36b44-111">displayName</span></span>                     | <span data-ttu-id="36b44-112">String</span><span class="sxs-lookup"><span data-stu-id="36b44-112">String</span></span>  |
| <span data-ttu-id="36b44-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="36b44-113">isDeleted</span></span>                       | <span data-ttu-id="36b44-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="36b44-114">Boolean</span></span> |
| <span data-ttu-id="36b44-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="36b44-115">deletedDate</span></span>                     | <span data-ttu-id="36b44-116">Date</span><span class="sxs-lookup"><span data-stu-id="36b44-116">Date</span></span>    |
| <span data-ttu-id="36b44-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="36b44-117">createdDate</span></span>                     | <span data-ttu-id="36b44-118">Date</span><span class="sxs-lookup"><span data-stu-id="36b44-118">Date</span></span>    |
| <span data-ttu-id="36b44-119">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="36b44-119">lastActivityDate</span></span>                | <span data-ttu-id="36b44-120">Date</span><span class="sxs-lookup"><span data-stu-id="36b44-120">Date</span></span>    |
| <span data-ttu-id="36b44-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="36b44-121">itemCount</span></span>                       | <span data-ttu-id="36b44-122">Int64</span><span class="sxs-lookup"><span data-stu-id="36b44-122">Int64</span></span>   |
| <span data-ttu-id="36b44-123">storageused inbytes</span><span class="sxs-lookup"><span data-stu-id="36b44-123">storageUsedInBytes</span></span>              | <span data-ttu-id="36b44-124">Int64</span><span class="sxs-lookup"><span data-stu-id="36b44-124">Int64</span></span>   |
| <span data-ttu-id="36b44-125">warnings ewarnings quot/バイト</span><span class="sxs-lookup"><span data-stu-id="36b44-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="36b44-126">Int64</span><span class="sxs-lookup"><span data-stu-id="36b44-126">Int64</span></span>   |
| <span data-ttu-id="36b44-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="36b44-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="36b44-128">Int64</span><span class="sxs-lookup"><span data-stu-id="36b44-128">Int64</span></span>   |
| <span data-ttu-id="36b44-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="36b44-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="36b44-130">Int64</span><span class="sxs-lookup"><span data-stu-id="36b44-130">Int64</span></span>   |
| <span data-ttu-id="36b44-131">reportperiod</span><span class="sxs-lookup"><span data-stu-id="36b44-131">reportPeriod</span></span>                    | <span data-ttu-id="36b44-132">String</span><span class="sxs-lookup"><span data-stu-id="36b44-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="36b44-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36b44-133">JSON representation</span></span>

<span data-ttu-id="36b44-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36b44-134">The following is a JSON representation of the resource.</span></span>

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
