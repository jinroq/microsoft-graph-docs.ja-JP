---
title: yammerDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 0f4d543ec8a96eaa4e237a1db1367efdc625c4e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892016"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="a942d-103">yammerDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a942d-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a942d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a942d-104">Properties</span></span>

| <span data-ttu-id="a942d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a942d-105">Property</span></span>          | <span data-ttu-id="a942d-106">種類</span><span class="sxs-lookup"><span data-stu-id="a942d-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="a942d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a942d-107">reportRefreshDate</span></span> | <span data-ttu-id="a942d-108">日付</span><span class="sxs-lookup"><span data-stu-id="a942d-108">Date</span></span>    |
| <span data-ttu-id="a942d-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a942d-109">userPrincipalName</span></span> | <span data-ttu-id="a942d-110">String</span><span class="sxs-lookup"><span data-stu-id="a942d-110">String</span></span>  |
| <span data-ttu-id="a942d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a942d-111">displayName</span></span>       | <span data-ttu-id="a942d-112">String</span><span class="sxs-lookup"><span data-stu-id="a942d-112">String</span></span>  |
| <span data-ttu-id="a942d-113">userState</span><span class="sxs-lookup"><span data-stu-id="a942d-113">userState</span></span>         | <span data-ttu-id="a942d-114">String</span><span class="sxs-lookup"><span data-stu-id="a942d-114">String</span></span>  |
| <span data-ttu-id="a942d-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="a942d-115">stateChangeDate</span></span>   | <span data-ttu-id="a942d-116">日付</span><span class="sxs-lookup"><span data-stu-id="a942d-116">Date</span></span>    |
| <span data-ttu-id="a942d-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a942d-117">lastActivityDate</span></span>  | <span data-ttu-id="a942d-118">日付</span><span class="sxs-lookup"><span data-stu-id="a942d-118">Date</span></span>    |
| <span data-ttu-id="a942d-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="a942d-119">usedWeb</span></span>           | <span data-ttu-id="a942d-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="a942d-120">Boolean</span></span> |
| <span data-ttu-id="a942d-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="a942d-121">usedWindowsPhone</span></span>  | <span data-ttu-id="a942d-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="a942d-122">Boolean</span></span> |
| <span data-ttu-id="a942d-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="a942d-123">usedAndroidPhone</span></span>  | <span data-ttu-id="a942d-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="a942d-124">Boolean</span></span> |
| <span data-ttu-id="a942d-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="a942d-125">usediPhone</span></span>        | <span data-ttu-id="a942d-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="a942d-126">Boolean</span></span> |
| <span data-ttu-id="a942d-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="a942d-127">usediPad</span></span>          | <span data-ttu-id="a942d-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="a942d-128">Boolean</span></span> |
| <span data-ttu-id="a942d-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="a942d-129">usedOthers</span></span>        | <span data-ttu-id="a942d-130">ブール型</span><span class="sxs-lookup"><span data-stu-id="a942d-130">Boolean</span></span> |
| <span data-ttu-id="a942d-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a942d-131">reportPeriod</span></span>      | <span data-ttu-id="a942d-132">String</span><span class="sxs-lookup"><span data-stu-id="a942d-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a942d-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a942d-133">JSON representation</span></span>

<span data-ttu-id="a942d-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a942d-134">The following is a JSON representation of the resource.</span></span>

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
