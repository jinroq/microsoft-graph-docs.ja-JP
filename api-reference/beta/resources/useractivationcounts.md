---
title: userActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581283"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="bdb0d-103">userActivationCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bdb0d-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bdb0d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdb0d-104">Properties</span></span>

| <span data-ttu-id="bdb0d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdb0d-105">Property</span></span>          | <span data-ttu-id="bdb0d-106">型</span><span class="sxs-lookup"><span data-stu-id="bdb0d-106">Type</span></span>   | <span data-ttu-id="bdb0d-107">説明</span><span class="sxs-lookup"><span data-stu-id="bdb0d-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="bdb0d-108">productType</span><span class="sxs-lookup"><span data-stu-id="bdb0d-108">productType</span></span>       | <span data-ttu-id="bdb0d-109">String</span><span class="sxs-lookup"><span data-stu-id="bdb0d-109">String</span></span> | <span data-ttu-id="bdb0d-110">"office 365 ProPlus"、"Project Client"、"Visio Pro for Office 365" などの製品の種類。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="bdb0d-111">lastactivateddate</span><span class="sxs-lookup"><span data-stu-id="bdb0d-111">lastActivatedDate</span></span> | <span data-ttu-id="bdb0d-112">Date</span><span class="sxs-lookup"><span data-stu-id="bdb0d-112">Date</span></span>   | <span data-ttu-id="bdb0d-113">最新のライセンス認証の日付。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="bdb0d-114">ws</span><span class="sxs-lookup"><span data-stu-id="bdb0d-114">windows</span></span>           | <span data-ttu-id="bdb0d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="bdb0d-115">Int64</span></span>  | <span data-ttu-id="bdb0d-116">Windows のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-116">The activation count on Windows.</span></span> <span data-ttu-id="bdb0d-117">この番号には、Windows コンピューターのすべてのライセンス認証が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="bdb0d-118">Mac</span><span class="sxs-lookup"><span data-stu-id="bdb0d-118">mac</span></span>               | <span data-ttu-id="bdb0d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="bdb0d-119">Int64</span></span>  | <span data-ttu-id="bdb0d-120">Mac OS のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="bdb0d-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="bdb0d-121">windows10Mobile</span></span>   | <span data-ttu-id="bdb0d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="bdb0d-122">Int64</span></span>  | <span data-ttu-id="bdb0d-123">Windows 10 mobile のライセンス認証回数。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="bdb0d-124">ios</span><span class="sxs-lookup"><span data-stu-id="bdb0d-124">ios</span></span>               | <span data-ttu-id="bdb0d-125">Int64</span><span class="sxs-lookup"><span data-stu-id="bdb0d-125">Int64</span></span>  | <span data-ttu-id="bdb0d-126">iOS のアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="bdb0d-127">android</span><span class="sxs-lookup"><span data-stu-id="bdb0d-127">android</span></span>           | <span data-ttu-id="bdb0d-128">Int64</span><span class="sxs-lookup"><span data-stu-id="bdb0d-128">Int64</span></span>  | <span data-ttu-id="bdb0d-129">Android デバイスのアクティブ化回数。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="bdb0d-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="bdb0d-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="bdb0d-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdb0d-131">Boolean</span></span> | <span data-ttu-id="bdb0d-132">ユーザーが以前に共有コンピューターで製品を使用した場合は True。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bdb0d-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bdb0d-133">JSON representation</span></span>

<span data-ttu-id="bdb0d-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bdb0d-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```
