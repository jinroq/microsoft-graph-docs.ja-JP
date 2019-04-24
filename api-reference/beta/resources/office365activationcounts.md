---
title: office365ActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7bc21be693a5c68ecd5c6a1e4e44d53c9261acdb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505467"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="1477d-103">office365ActivationCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1477d-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1477d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1477d-104">Properties</span></span>

| <span data-ttu-id="1477d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1477d-105">Property</span></span>          | <span data-ttu-id="1477d-106">型</span><span class="sxs-lookup"><span data-stu-id="1477d-106">Type</span></span>   | <span data-ttu-id="1477d-107">説明</span><span class="sxs-lookup"><span data-stu-id="1477d-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="1477d-108">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="1477d-108">reportRefreshDate</span></span> | <span data-ttu-id="1477d-109">Date</span><span class="sxs-lookup"><span data-stu-id="1477d-109">Date</span></span>   | <span data-ttu-id="1477d-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="1477d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="1477d-111">productType</span><span class="sxs-lookup"><span data-stu-id="1477d-111">productType</span></span>       | <span data-ttu-id="1477d-112">String</span><span class="sxs-lookup"><span data-stu-id="1477d-112">String</span></span> | <span data-ttu-id="1477d-113">"office 365 ProPlus"、"Project Client"、"Visio Pro for Office 365" などの製品の種類。</span><span class="sxs-lookup"><span data-stu-id="1477d-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="1477d-114">ws</span><span class="sxs-lookup"><span data-stu-id="1477d-114">windows</span></span>           | <span data-ttu-id="1477d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="1477d-115">Int64</span></span>  | <span data-ttu-id="1477d-116">Windows のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="1477d-116">The activation count on Windows.</span></span> <span data-ttu-id="1477d-117">この番号には、Windows コンピューターのすべてのライセンス認証が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1477d-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="1477d-118">Mac</span><span class="sxs-lookup"><span data-stu-id="1477d-118">mac</span></span>               | <span data-ttu-id="1477d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="1477d-119">Int64</span></span>  | <span data-ttu-id="1477d-120">Mac OS のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="1477d-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="1477d-121">android</span><span class="sxs-lookup"><span data-stu-id="1477d-121">android</span></span>           | <span data-ttu-id="1477d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1477d-122">Int64</span></span>  | <span data-ttu-id="1477d-123">Android デバイスのアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="1477d-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="1477d-124">ios</span><span class="sxs-lookup"><span data-stu-id="1477d-124">ios</span></span>               | <span data-ttu-id="1477d-125">Int64</span><span class="sxs-lookup"><span data-stu-id="1477d-125">Int64</span></span>  | <span data-ttu-id="1477d-126">iOS のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="1477d-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="1477d-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="1477d-127">windows10Mobile</span></span>   | <span data-ttu-id="1477d-128">Int64</span><span class="sxs-lookup"><span data-stu-id="1477d-128">Int64</span></span>  | <span data-ttu-id="1477d-129">Windows 10 mobile のライセンス認証回数。</span><span class="sxs-lookup"><span data-stu-id="1477d-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1477d-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1477d-130">JSON representation</span></span>

<span data-ttu-id="1477d-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1477d-131">The following is a JSON representation of the resource.</span></span>

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
