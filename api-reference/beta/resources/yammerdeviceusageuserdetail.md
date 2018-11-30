---
title: yammerDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 8812b61d974815fd1cdf1bbe1549a21193e5a2f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073767"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="14467-103">yammerDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14467-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="14467-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14467-104">Properties</span></span>

| <span data-ttu-id="14467-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14467-105">Property</span></span>          | <span data-ttu-id="14467-106">型</span><span class="sxs-lookup"><span data-stu-id="14467-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="14467-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="14467-107">reportRefreshDate</span></span> | <span data-ttu-id="14467-108">Date</span><span class="sxs-lookup"><span data-stu-id="14467-108">Date</span></span>    |
| <span data-ttu-id="14467-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="14467-109">userPrincipalName</span></span> | <span data-ttu-id="14467-110">String</span><span class="sxs-lookup"><span data-stu-id="14467-110">String</span></span>  |
| <span data-ttu-id="14467-111">displayName</span><span class="sxs-lookup"><span data-stu-id="14467-111">displayName</span></span>       | <span data-ttu-id="14467-112">String</span><span class="sxs-lookup"><span data-stu-id="14467-112">String</span></span>  |
| <span data-ttu-id="14467-113">userState</span><span class="sxs-lookup"><span data-stu-id="14467-113">userState</span></span>         | <span data-ttu-id="14467-114">String</span><span class="sxs-lookup"><span data-stu-id="14467-114">String</span></span>  |
| <span data-ttu-id="14467-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="14467-115">stateChangeDate</span></span>   | <span data-ttu-id="14467-116">Date</span><span class="sxs-lookup"><span data-stu-id="14467-116">Date</span></span>    |
| <span data-ttu-id="14467-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="14467-117">lastActivityDate</span></span>  | <span data-ttu-id="14467-118">Date</span><span class="sxs-lookup"><span data-stu-id="14467-118">Date</span></span>    |
| <span data-ttu-id="14467-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="14467-119">usedWeb</span></span>           | <span data-ttu-id="14467-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="14467-120">Boolean</span></span> |
| <span data-ttu-id="14467-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="14467-121">usedWindowsPhone</span></span>  | <span data-ttu-id="14467-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="14467-122">Boolean</span></span> |
| <span data-ttu-id="14467-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="14467-123">usedAndroidPhone</span></span>  | <span data-ttu-id="14467-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="14467-124">Boolean</span></span> |
| <span data-ttu-id="14467-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="14467-125">usediPhone</span></span>        | <span data-ttu-id="14467-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="14467-126">Boolean</span></span> |
| <span data-ttu-id="14467-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="14467-127">usediPad</span></span>          | <span data-ttu-id="14467-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="14467-128">Boolean</span></span> |
| <span data-ttu-id="14467-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="14467-129">usedOthers</span></span>        | <span data-ttu-id="14467-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="14467-130">Boolean</span></span> |
| <span data-ttu-id="14467-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="14467-131">reportPeriod</span></span>      | <span data-ttu-id="14467-132">String</span><span class="sxs-lookup"><span data-stu-id="14467-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="14467-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14467-133">JSON representation</span></span>

<span data-ttu-id="14467-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14467-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
