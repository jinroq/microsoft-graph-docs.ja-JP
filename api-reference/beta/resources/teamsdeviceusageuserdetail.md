---
title: teamsDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06e2cea1154c608b61642b07adbd96aae1710903
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807106"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="6d832-103">teamsDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d832-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d832-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d832-104">Properties</span></span>

| <span data-ttu-id="6d832-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d832-105">Property</span></span>          | <span data-ttu-id="6d832-106">種類</span><span class="sxs-lookup"><span data-stu-id="6d832-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="6d832-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d832-107">reportRefreshDate</span></span> | <span data-ttu-id="6d832-108">日付</span><span class="sxs-lookup"><span data-stu-id="6d832-108">Date</span></span>    |
| <span data-ttu-id="6d832-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6d832-109">userPrincipalName</span></span> | <span data-ttu-id="6d832-110">String</span><span class="sxs-lookup"><span data-stu-id="6d832-110">String</span></span>  |
| <span data-ttu-id="6d832-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6d832-111">lastActivityDate</span></span>  | <span data-ttu-id="6d832-112">日付</span><span class="sxs-lookup"><span data-stu-id="6d832-112">Date</span></span>    |
| <span data-ttu-id="6d832-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6d832-113">isDeleted</span></span>         | <span data-ttu-id="6d832-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="6d832-114">Boolean</span></span> |
| <span data-ttu-id="6d832-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="6d832-115">deletedDate</span></span>       | <span data-ttu-id="6d832-116">日付</span><span class="sxs-lookup"><span data-stu-id="6d832-116">Date</span></span>    |
| <span data-ttu-id="6d832-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="6d832-117">usedWeb</span></span>           | <span data-ttu-id="6d832-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="6d832-118">Boolean</span></span> |
| <span data-ttu-id="6d832-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="6d832-119">usedWindowsPhone</span></span>  | <span data-ttu-id="6d832-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="6d832-120">Boolean</span></span> |
| <span data-ttu-id="6d832-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="6d832-121">usediOS</span></span>           | <span data-ttu-id="6d832-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="6d832-122">Boolean</span></span> |
| <span data-ttu-id="6d832-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="6d832-123">usedMac</span></span>           | <span data-ttu-id="6d832-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="6d832-124">Boolean</span></span> |
| <span data-ttu-id="6d832-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="6d832-125">usedAndroidPhone</span></span>  | <span data-ttu-id="6d832-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="6d832-126">Boolean</span></span> |
| <span data-ttu-id="6d832-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="6d832-127">usedWindows</span></span>       | <span data-ttu-id="6d832-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="6d832-128">Boolean</span></span> |
| <span data-ttu-id="6d832-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d832-129">reportPeriod</span></span>      | <span data-ttu-id="6d832-130">String</span><span class="sxs-lookup"><span data-stu-id="6d832-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6d832-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d832-131">JSON representation</span></span>

<span data-ttu-id="6d832-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d832-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
