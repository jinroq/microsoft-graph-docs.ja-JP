---
title: Skypeforbusinessdevice使い方 Userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b84cf9c7654354446fb7c6a5005befe3d17a0fa4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964915"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="de6fe-103">Skypeforbusinessdevice使い方 Userdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de6fe-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="de6fe-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de6fe-104">Properties</span></span>

| <span data-ttu-id="de6fe-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de6fe-105">Property</span></span>          | <span data-ttu-id="de6fe-106">型</span><span class="sxs-lookup"><span data-stu-id="de6fe-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="de6fe-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="de6fe-107">reportRefreshDate</span></span> | <span data-ttu-id="de6fe-108">日付</span><span class="sxs-lookup"><span data-stu-id="de6fe-108">Date</span></span>    |
| <span data-ttu-id="de6fe-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="de6fe-109">userPrincipalName</span></span> | <span data-ttu-id="de6fe-110">String</span><span class="sxs-lookup"><span data-stu-id="de6fe-110">String</span></span>  |
| <span data-ttu-id="de6fe-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="de6fe-111">lastActivityDate</span></span>  | <span data-ttu-id="de6fe-112">日付</span><span class="sxs-lookup"><span data-stu-id="de6fe-112">Date</span></span>    |
| <span data-ttu-id="de6fe-113">未使用のウィンドウ</span><span class="sxs-lookup"><span data-stu-id="de6fe-113">usedWindows</span></span>       | <span data-ttu-id="de6fe-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="de6fe-114">Boolean</span></span> |
| <span data-ttu-id="de6fe-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="de6fe-115">usedWindowsPhone</span></span>  | <span data-ttu-id="de6fe-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="de6fe-116">Boolean</span></span> |
| <span data-ttu-id="de6fe-117">Used Androidphone</span><span class="sxs-lookup"><span data-stu-id="de6fe-117">usedAndroidPhone</span></span>  | <span data-ttu-id="de6fe-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="de6fe-118">Boolean</span></span> |
| <span data-ttu-id="de6fe-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="de6fe-119">usediPhone</span></span>        | <span data-ttu-id="de6fe-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="de6fe-120">Boolean</span></span> |
| <span data-ttu-id="de6fe-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="de6fe-121">usediPad</span></span>          | <span data-ttu-id="de6fe-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="de6fe-122">Boolean</span></span> |
| <span data-ttu-id="de6fe-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="de6fe-123">reportPeriod</span></span>      | <span data-ttu-id="de6fe-124">String</span><span class="sxs-lookup"><span data-stu-id="de6fe-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="de6fe-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de6fe-125">JSON representation</span></span>

<span data-ttu-id="de6fe-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de6fe-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
