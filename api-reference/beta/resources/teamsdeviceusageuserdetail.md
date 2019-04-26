---
title: teamsdeviceの使い方 userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553604"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="a3bb8-103">teamsdeviceの使い方 userdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3bb8-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a3bb8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3bb8-104">Properties</span></span>

| <span data-ttu-id="a3bb8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3bb8-105">Property</span></span>          | <span data-ttu-id="a3bb8-106">型</span><span class="sxs-lookup"><span data-stu-id="a3bb8-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="a3bb8-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="a3bb8-107">reportRefreshDate</span></span> | <span data-ttu-id="a3bb8-108">Date</span><span class="sxs-lookup"><span data-stu-id="a3bb8-108">Date</span></span>    |
| <span data-ttu-id="a3bb8-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3bb8-109">userPrincipalName</span></span> | <span data-ttu-id="a3bb8-110">String</span><span class="sxs-lookup"><span data-stu-id="a3bb8-110">String</span></span>  |
| <span data-ttu-id="a3bb8-111">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="a3bb8-111">lastActivityDate</span></span>  | <span data-ttu-id="a3bb8-112">Date</span><span class="sxs-lookup"><span data-stu-id="a3bb8-112">Date</span></span>    |
| <span data-ttu-id="a3bb8-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a3bb8-113">isDeleted</span></span>         | <span data-ttu-id="a3bb8-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="a3bb8-114">Boolean</span></span> |
| <span data-ttu-id="a3bb8-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a3bb8-115">deletedDate</span></span>       | <span data-ttu-id="a3bb8-116">Date</span><span class="sxs-lookup"><span data-stu-id="a3bb8-116">Date</span></span>    |
| <span data-ttu-id="a3bb8-117">used web</span><span class="sxs-lookup"><span data-stu-id="a3bb8-117">usedWeb</span></span>           | <span data-ttu-id="a3bb8-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="a3bb8-118">Boolean</span></span> |
| <span data-ttu-id="a3bb8-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="a3bb8-119">usedWindowsPhone</span></span>  | <span data-ttu-id="a3bb8-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="a3bb8-120">Boolean</span></span> |
| <span data-ttu-id="a3bb8-121">usedios</span><span class="sxs-lookup"><span data-stu-id="a3bb8-121">usediOS</span></span>           | <span data-ttu-id="a3bb8-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="a3bb8-122">Boolean</span></span> |
| <span data-ttu-id="a3bb8-123">used mac</span><span class="sxs-lookup"><span data-stu-id="a3bb8-123">usedMac</span></span>           | <span data-ttu-id="a3bb8-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="a3bb8-124">Boolean</span></span> |
| <span data-ttu-id="a3bb8-125">used androidphone</span><span class="sxs-lookup"><span data-stu-id="a3bb8-125">usedAndroidPhone</span></span>  | <span data-ttu-id="a3bb8-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="a3bb8-126">Boolean</span></span> |
| <span data-ttu-id="a3bb8-127">未使用のウィンドウ</span><span class="sxs-lookup"><span data-stu-id="a3bb8-127">usedWindows</span></span>       | <span data-ttu-id="a3bb8-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="a3bb8-128">Boolean</span></span> |
| <span data-ttu-id="a3bb8-129">reportperiod</span><span class="sxs-lookup"><span data-stu-id="a3bb8-129">reportPeriod</span></span>      | <span data-ttu-id="a3bb8-130">String</span><span class="sxs-lookup"><span data-stu-id="a3bb8-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a3bb8-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3bb8-131">JSON representation</span></span>

<span data-ttu-id="a3bb8-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3bb8-132">The following is a JSON representation of the resource.</span></span>

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
