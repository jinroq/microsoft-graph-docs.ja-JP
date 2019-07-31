---
title: office365ActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d396ee84e4af6606cfde3e5fc17ef02c0a9594f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966581"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="35f97-103">office365ActivationCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35f97-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="35f97-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35f97-104">Properties</span></span>

| <span data-ttu-id="35f97-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35f97-105">Property</span></span>          | <span data-ttu-id="35f97-106">型</span><span class="sxs-lookup"><span data-stu-id="35f97-106">Type</span></span>   | <span data-ttu-id="35f97-107">説明</span><span class="sxs-lookup"><span data-stu-id="35f97-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="35f97-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="35f97-108">reportRefreshDate</span></span> | <span data-ttu-id="35f97-109">日付</span><span class="sxs-lookup"><span data-stu-id="35f97-109">Date</span></span>   | <span data-ttu-id="35f97-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="35f97-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="35f97-111">productType</span><span class="sxs-lookup"><span data-stu-id="35f97-111">productType</span></span>       | <span data-ttu-id="35f97-112">String</span><span class="sxs-lookup"><span data-stu-id="35f97-112">String</span></span> | <span data-ttu-id="35f97-113">"Office 365 ProPlus"、"Project Client"、"Visio Pro for Office 365" などの製品の種類。</span><span class="sxs-lookup"><span data-stu-id="35f97-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="35f97-114">ws</span><span class="sxs-lookup"><span data-stu-id="35f97-114">windows</span></span>           | <span data-ttu-id="35f97-115">Int64</span><span class="sxs-lookup"><span data-stu-id="35f97-115">Int64</span></span>  | <span data-ttu-id="35f97-116">Windows のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="35f97-116">The activation count on Windows.</span></span> <span data-ttu-id="35f97-117">この番号には、Windows コンピューターのすべてのライセンス認証が含まれます。</span><span class="sxs-lookup"><span data-stu-id="35f97-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="35f97-118">Mac</span><span class="sxs-lookup"><span data-stu-id="35f97-118">mac</span></span>               | <span data-ttu-id="35f97-119">Int64</span><span class="sxs-lookup"><span data-stu-id="35f97-119">Int64</span></span>  | <span data-ttu-id="35f97-120">Mac OS のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="35f97-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="35f97-121">android</span><span class="sxs-lookup"><span data-stu-id="35f97-121">android</span></span>           | <span data-ttu-id="35f97-122">Int64</span><span class="sxs-lookup"><span data-stu-id="35f97-122">Int64</span></span>  | <span data-ttu-id="35f97-123">Android デバイスのアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="35f97-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="35f97-124">ios</span><span class="sxs-lookup"><span data-stu-id="35f97-124">ios</span></span>               | <span data-ttu-id="35f97-125">Int64</span><span class="sxs-lookup"><span data-stu-id="35f97-125">Int64</span></span>  | <span data-ttu-id="35f97-126">IOS のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="35f97-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="35f97-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="35f97-127">windows10Mobile</span></span>   | <span data-ttu-id="35f97-128">Int64</span><span class="sxs-lookup"><span data-stu-id="35f97-128">Int64</span></span>  | <span data-ttu-id="35f97-129">Windows 10 mobile のライセンス認証回数。</span><span class="sxs-lookup"><span data-stu-id="35f97-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35f97-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35f97-130">JSON representation</span></span>

<span data-ttu-id="35f97-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="35f97-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
