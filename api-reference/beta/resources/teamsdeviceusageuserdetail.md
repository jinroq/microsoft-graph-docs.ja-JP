---
title: teamsDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953786"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="6e70d-103">teamsDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e70d-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6e70d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e70d-104">Properties</span></span>

| <span data-ttu-id="6e70d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e70d-105">Property</span></span>          | <span data-ttu-id="6e70d-106">種類</span><span class="sxs-lookup"><span data-stu-id="6e70d-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="6e70d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6e70d-107">reportRefreshDate</span></span> | <span data-ttu-id="6e70d-108">日付</span><span class="sxs-lookup"><span data-stu-id="6e70d-108">Date</span></span>    |
| <span data-ttu-id="6e70d-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6e70d-109">userPrincipalName</span></span> | <span data-ttu-id="6e70d-110">String</span><span class="sxs-lookup"><span data-stu-id="6e70d-110">String</span></span>  |
| <span data-ttu-id="6e70d-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6e70d-111">lastActivityDate</span></span>  | <span data-ttu-id="6e70d-112">日付</span><span class="sxs-lookup"><span data-stu-id="6e70d-112">Date</span></span>    |
| <span data-ttu-id="6e70d-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6e70d-113">isDeleted</span></span>         | <span data-ttu-id="6e70d-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="6e70d-114">Boolean</span></span> |
| <span data-ttu-id="6e70d-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="6e70d-115">deletedDate</span></span>       | <span data-ttu-id="6e70d-116">日付</span><span class="sxs-lookup"><span data-stu-id="6e70d-116">Date</span></span>    |
| <span data-ttu-id="6e70d-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="6e70d-117">usedWeb</span></span>           | <span data-ttu-id="6e70d-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="6e70d-118">Boolean</span></span> |
| <span data-ttu-id="6e70d-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="6e70d-119">usedWindowsPhone</span></span>  | <span data-ttu-id="6e70d-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="6e70d-120">Boolean</span></span> |
| <span data-ttu-id="6e70d-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="6e70d-121">usediOS</span></span>           | <span data-ttu-id="6e70d-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="6e70d-122">Boolean</span></span> |
| <span data-ttu-id="6e70d-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="6e70d-123">usedMac</span></span>           | <span data-ttu-id="6e70d-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="6e70d-124">Boolean</span></span> |
| <span data-ttu-id="6e70d-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="6e70d-125">usedAndroidPhone</span></span>  | <span data-ttu-id="6e70d-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="6e70d-126">Boolean</span></span> |
| <span data-ttu-id="6e70d-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="6e70d-127">usedWindows</span></span>       | <span data-ttu-id="6e70d-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="6e70d-128">Boolean</span></span> |
| <span data-ttu-id="6e70d-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6e70d-129">reportPeriod</span></span>      | <span data-ttu-id="6e70d-130">String</span><span class="sxs-lookup"><span data-stu-id="6e70d-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6e70d-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e70d-131">JSON representation</span></span>

<span data-ttu-id="6e70d-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e70d-132">The following is a JSON representation of the resource.</span></span>

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
