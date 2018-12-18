---
title: userActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: dkershaw10
ms.openlocfilehash: 396f6182d000df6d701e8c0cbad3dd02a258c4c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322919"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="b11b0-103">userActivationCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b11b0-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b11b0-104">Properties</span><span class="sxs-lookup"><span data-stu-id="b11b0-104">Properties</span></span>

| <span data-ttu-id="b11b0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b11b0-105">Property</span></span>          | <span data-ttu-id="b11b0-106">種類</span><span class="sxs-lookup"><span data-stu-id="b11b0-106">Type</span></span>   | <span data-ttu-id="b11b0-107">説明</span><span class="sxs-lookup"><span data-stu-id="b11b0-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="b11b0-108">productType</span><span class="sxs-lookup"><span data-stu-id="b11b0-108">productType</span></span>       | <span data-ttu-id="b11b0-109">String</span><span class="sxs-lookup"><span data-stu-id="b11b0-109">String</span></span> | <span data-ttu-id="b11b0-110">「Office 365 用リソース"、「プロジェクト クライアント」など、製品の種類または"Office 365"の Visio Pro です。</span><span class="sxs-lookup"><span data-stu-id="b11b0-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="b11b0-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="b11b0-111">lastActivatedDate</span></span> | <span data-ttu-id="b11b0-112">日付</span><span class="sxs-lookup"><span data-stu-id="b11b0-112">Date</span></span>   | <span data-ttu-id="b11b0-113">最新のアクティブ化の日付です。</span><span class="sxs-lookup"><span data-stu-id="b11b0-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="b11b0-114">windows</span><span class="sxs-lookup"><span data-stu-id="b11b0-114">windows</span></span>           | <span data-ttu-id="b11b0-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b11b0-115">Int64</span></span>  | <span data-ttu-id="b11b0-116">[Windows のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="b11b0-116">The activation count on Windows.</span></span> <span data-ttu-id="b11b0-117">この数値には、任意の Windows コンピューターですべてのアクティブ化が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b11b0-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="b11b0-118">Mac</span><span class="sxs-lookup"><span data-stu-id="b11b0-118">mac</span></span>               | <span data-ttu-id="b11b0-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b11b0-119">Int64</span></span>  | <span data-ttu-id="b11b0-120">Mac OS のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="b11b0-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="b11b0-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="b11b0-121">windows10Mobile</span></span>   | <span data-ttu-id="b11b0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b11b0-122">Int64</span></span>  | <span data-ttu-id="b11b0-123">ライセンス認証カウント 10 の Windows のモバイルです。</span><span class="sxs-lookup"><span data-stu-id="b11b0-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="b11b0-124">ios</span><span class="sxs-lookup"><span data-stu-id="b11b0-124">ios</span></span>               | <span data-ttu-id="b11b0-125">Int64</span><span class="sxs-lookup"><span data-stu-id="b11b0-125">Int64</span></span>  | <span data-ttu-id="b11b0-126">IOS のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="b11b0-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="b11b0-127">android</span><span class="sxs-lookup"><span data-stu-id="b11b0-127">android</span></span>           | <span data-ttu-id="b11b0-128">Int64</span><span class="sxs-lookup"><span data-stu-id="b11b0-128">Int64</span></span>  | <span data-ttu-id="b11b0-129">Android デバイス上のアクティブ化の数。</span><span class="sxs-lookup"><span data-stu-id="b11b0-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="b11b0-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="b11b0-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="b11b0-131">ブール型</span><span class="sxs-lookup"><span data-stu-id="b11b0-131">Boolean</span></span> | <span data-ttu-id="b11b0-132">ユーザーが共有する前にコンピューターに製品を使用する場合は true にします。</span><span class="sxs-lookup"><span data-stu-id="b11b0-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b11b0-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b11b0-133">JSON representation</span></span>

<span data-ttu-id="b11b0-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b11b0-134">The following is a JSON representation of the resource.</span></span>

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
