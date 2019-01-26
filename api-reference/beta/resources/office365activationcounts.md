---
title: office365ActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7bc21be693a5c68ecd5c6a1e4e44d53c9261acdb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575528"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="39e0a-103">office365ActivationCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39e0a-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="39e0a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39e0a-104">Properties</span></span>

| <span data-ttu-id="39e0a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39e0a-105">Property</span></span>          | <span data-ttu-id="39e0a-106">型</span><span class="sxs-lookup"><span data-stu-id="39e0a-106">Type</span></span>   | <span data-ttu-id="39e0a-107">説明</span><span class="sxs-lookup"><span data-stu-id="39e0a-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="39e0a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="39e0a-108">reportRefreshDate</span></span> | <span data-ttu-id="39e0a-109">日付</span><span class="sxs-lookup"><span data-stu-id="39e0a-109">Date</span></span>   | <span data-ttu-id="39e0a-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="39e0a-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="39e0a-111">productType</span><span class="sxs-lookup"><span data-stu-id="39e0a-111">productType</span></span>       | <span data-ttu-id="39e0a-112">String</span><span class="sxs-lookup"><span data-stu-id="39e0a-112">String</span></span> | <span data-ttu-id="39e0a-113">「Office 365 用リソース"、「プロジェクト クライアント」など、製品の種類または"Office 365"の Visio Pro です。</span><span class="sxs-lookup"><span data-stu-id="39e0a-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="39e0a-114">windows</span><span class="sxs-lookup"><span data-stu-id="39e0a-114">windows</span></span>           | <span data-ttu-id="39e0a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="39e0a-115">Int64</span></span>  | <span data-ttu-id="39e0a-116">[Windows のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="39e0a-116">The activation count on Windows.</span></span> <span data-ttu-id="39e0a-117">この数値には、任意の Windows コンピューターですべてのアクティブ化が含まれます。</span><span class="sxs-lookup"><span data-stu-id="39e0a-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="39e0a-118">Mac</span><span class="sxs-lookup"><span data-stu-id="39e0a-118">mac</span></span>               | <span data-ttu-id="39e0a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="39e0a-119">Int64</span></span>  | <span data-ttu-id="39e0a-120">Mac OS のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="39e0a-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="39e0a-121">android</span><span class="sxs-lookup"><span data-stu-id="39e0a-121">android</span></span>           | <span data-ttu-id="39e0a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="39e0a-122">Int64</span></span>  | <span data-ttu-id="39e0a-123">Android デバイス上のアクティブ化の数。</span><span class="sxs-lookup"><span data-stu-id="39e0a-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="39e0a-124">ios</span><span class="sxs-lookup"><span data-stu-id="39e0a-124">ios</span></span>               | <span data-ttu-id="39e0a-125">Int64</span><span class="sxs-lookup"><span data-stu-id="39e0a-125">Int64</span></span>  | <span data-ttu-id="39e0a-126">IOS のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="39e0a-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="39e0a-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="39e0a-127">windows10Mobile</span></span>   | <span data-ttu-id="39e0a-128">Int64</span><span class="sxs-lookup"><span data-stu-id="39e0a-128">Int64</span></span>  | <span data-ttu-id="39e0a-129">ライセンス認証カウント 10 の Windows のモバイルです。</span><span class="sxs-lookup"><span data-stu-id="39e0a-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="39e0a-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39e0a-130">JSON representation</span></span>

<span data-ttu-id="39e0a-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39e0a-131">The following is a JSON representation of the resource.</span></span>

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
