---
title: Teamsdeviceの使い方 Userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5bd7443e775a8a9de0dbbc27cf8843331f8f8cb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007628"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="4b959-103">Teamsdeviceの使い方 Userdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b959-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4b959-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b959-104">Properties</span></span>

| <span data-ttu-id="4b959-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b959-105">Property</span></span>          | <span data-ttu-id="4b959-106">型</span><span class="sxs-lookup"><span data-stu-id="4b959-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="4b959-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4b959-107">reportRefreshDate</span></span> | <span data-ttu-id="4b959-108">日付</span><span class="sxs-lookup"><span data-stu-id="4b959-108">Date</span></span>    |
| <span data-ttu-id="4b959-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b959-109">userPrincipalName</span></span> | <span data-ttu-id="4b959-110">String</span><span class="sxs-lookup"><span data-stu-id="4b959-110">String</span></span>  |
| <span data-ttu-id="4b959-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4b959-111">lastActivityDate</span></span>  | <span data-ttu-id="4b959-112">日付</span><span class="sxs-lookup"><span data-stu-id="4b959-112">Date</span></span>    |
| <span data-ttu-id="4b959-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4b959-113">isDeleted</span></span>         | <span data-ttu-id="4b959-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b959-114">Boolean</span></span> |
| <span data-ttu-id="4b959-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="4b959-115">deletedDate</span></span>       | <span data-ttu-id="4b959-116">日付</span><span class="sxs-lookup"><span data-stu-id="4b959-116">Date</span></span>    |
| <span data-ttu-id="4b959-117">Used Web</span><span class="sxs-lookup"><span data-stu-id="4b959-117">usedWeb</span></span>           | <span data-ttu-id="4b959-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b959-118">Boolean</span></span> |
| <span data-ttu-id="4b959-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="4b959-119">usedWindowsPhone</span></span>  | <span data-ttu-id="4b959-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b959-120">Boolean</span></span> |
| <span data-ttu-id="4b959-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="4b959-121">usediOS</span></span>           | <span data-ttu-id="4b959-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b959-122">Boolean</span></span> |
| <span data-ttu-id="4b959-123">Used Mac</span><span class="sxs-lookup"><span data-stu-id="4b959-123">usedMac</span></span>           | <span data-ttu-id="4b959-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b959-124">Boolean</span></span> |
| <span data-ttu-id="4b959-125">Used Androidphone</span><span class="sxs-lookup"><span data-stu-id="4b959-125">usedAndroidPhone</span></span>  | <span data-ttu-id="4b959-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b959-126">Boolean</span></span> |
| <span data-ttu-id="4b959-127">未使用のウィンドウ</span><span class="sxs-lookup"><span data-stu-id="4b959-127">usedWindows</span></span>       | <span data-ttu-id="4b959-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b959-128">Boolean</span></span> |
| <span data-ttu-id="4b959-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4b959-129">reportPeriod</span></span>      | <span data-ttu-id="4b959-130">String</span><span class="sxs-lookup"><span data-stu-id="4b959-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="4b959-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b959-131">JSON representation</span></span>

<span data-ttu-id="4b959-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b959-132">The following is a JSON representation of the resource.</span></span>

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
