---
title: office365ActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 30386b3833b8140d4c602e27cb3a78f3a68670dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824991"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="06101-103">office365ActivationCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06101-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="06101-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06101-104">Properties</span></span>

| <span data-ttu-id="06101-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06101-105">Property</span></span>          | <span data-ttu-id="06101-106">種類</span><span class="sxs-lookup"><span data-stu-id="06101-106">Type</span></span>   | <span data-ttu-id="06101-107">説明</span><span class="sxs-lookup"><span data-stu-id="06101-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="06101-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="06101-108">reportRefreshDate</span></span> | <span data-ttu-id="06101-109">日付</span><span class="sxs-lookup"><span data-stu-id="06101-109">Date</span></span>   | <span data-ttu-id="06101-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="06101-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="06101-111">productType</span><span class="sxs-lookup"><span data-stu-id="06101-111">productType</span></span>       | <span data-ttu-id="06101-112">String</span><span class="sxs-lookup"><span data-stu-id="06101-112">String</span></span> | <span data-ttu-id="06101-113">「Office 365 用リソース"、「プロジェクト クライアント」など、製品の種類または"Office 365"の Visio Pro です。</span><span class="sxs-lookup"><span data-stu-id="06101-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="06101-114">windows</span><span class="sxs-lookup"><span data-stu-id="06101-114">windows</span></span>           | <span data-ttu-id="06101-115">Int64</span><span class="sxs-lookup"><span data-stu-id="06101-115">Int64</span></span>  | <span data-ttu-id="06101-116">[Windows のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="06101-116">The activation count on Windows.</span></span> <span data-ttu-id="06101-117">この数値には、任意の Windows コンピューターですべてのアクティブ化が含まれます。</span><span class="sxs-lookup"><span data-stu-id="06101-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="06101-118">Mac</span><span class="sxs-lookup"><span data-stu-id="06101-118">mac</span></span>               | <span data-ttu-id="06101-119">Int64</span><span class="sxs-lookup"><span data-stu-id="06101-119">Int64</span></span>  | <span data-ttu-id="06101-120">Mac OS のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="06101-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="06101-121">android</span><span class="sxs-lookup"><span data-stu-id="06101-121">android</span></span>           | <span data-ttu-id="06101-122">Int64</span><span class="sxs-lookup"><span data-stu-id="06101-122">Int64</span></span>  | <span data-ttu-id="06101-123">Android デバイス上のアクティブ化の数。</span><span class="sxs-lookup"><span data-stu-id="06101-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="06101-124">ios</span><span class="sxs-lookup"><span data-stu-id="06101-124">ios</span></span>               | <span data-ttu-id="06101-125">Int64</span><span class="sxs-lookup"><span data-stu-id="06101-125">Int64</span></span>  | <span data-ttu-id="06101-126">IOS のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="06101-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="06101-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="06101-127">windows10Mobile</span></span>   | <span data-ttu-id="06101-128">Int64</span><span class="sxs-lookup"><span data-stu-id="06101-128">Int64</span></span>  | <span data-ttu-id="06101-129">ライセンス認証カウント 10 の Windows のモバイルです。</span><span class="sxs-lookup"><span data-stu-id="06101-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="06101-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06101-130">JSON representation</span></span>

<span data-ttu-id="06101-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06101-131">The following is a JSON representation of the resource.</span></span>

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
