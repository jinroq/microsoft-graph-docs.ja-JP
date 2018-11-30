---
title: userActivationCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 022b73310a54877889efebabbb6e8fc4ab71fb65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069473"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="e444c-103">userActivationCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e444c-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e444c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e444c-104">Properties</span></span>

| <span data-ttu-id="e444c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e444c-105">Property</span></span>          | <span data-ttu-id="e444c-106">型</span><span class="sxs-lookup"><span data-stu-id="e444c-106">Type</span></span>   | <span data-ttu-id="e444c-107">説明</span><span class="sxs-lookup"><span data-stu-id="e444c-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="e444c-108">productType</span><span class="sxs-lookup"><span data-stu-id="e444c-108">productType</span></span>       | <span data-ttu-id="e444c-109">String</span><span class="sxs-lookup"><span data-stu-id="e444c-109">String</span></span> | <span data-ttu-id="e444c-110">「Office 365 用リソース"、「プロジェクト クライアント」など、製品の種類または"Office 365"の Visio Pro です。</span><span class="sxs-lookup"><span data-stu-id="e444c-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="e444c-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="e444c-111">lastActivatedDate</span></span> | <span data-ttu-id="e444c-112">Date</span><span class="sxs-lookup"><span data-stu-id="e444c-112">Date</span></span>   | <span data-ttu-id="e444c-113">最新のアクティブ化の日付です。</span><span class="sxs-lookup"><span data-stu-id="e444c-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="e444c-114">windows</span><span class="sxs-lookup"><span data-stu-id="e444c-114">windows</span></span>           | <span data-ttu-id="e444c-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e444c-115">Int64</span></span>  | <span data-ttu-id="e444c-116">[Windows のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="e444c-116">The activation count on Windows.</span></span> <span data-ttu-id="e444c-117">この数値には、任意の Windows コンピューターですべてのアクティブ化が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e444c-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="e444c-118">Mac</span><span class="sxs-lookup"><span data-stu-id="e444c-118">mac</span></span>               | <span data-ttu-id="e444c-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e444c-119">Int64</span></span>  | <span data-ttu-id="e444c-120">Mac OS のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="e444c-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="e444c-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="e444c-121">windows10Mobile</span></span>   | <span data-ttu-id="e444c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e444c-122">Int64</span></span>  | <span data-ttu-id="e444c-123">ライセンス認証カウント 10 の Windows のモバイルです。</span><span class="sxs-lookup"><span data-stu-id="e444c-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="e444c-124">ios</span><span class="sxs-lookup"><span data-stu-id="e444c-124">ios</span></span>               | <span data-ttu-id="e444c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="e444c-125">Int64</span></span>  | <span data-ttu-id="e444c-126">IOS のライセンス認証の数です。</span><span class="sxs-lookup"><span data-stu-id="e444c-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="e444c-127">android</span><span class="sxs-lookup"><span data-stu-id="e444c-127">android</span></span>           | <span data-ttu-id="e444c-128">Int64</span><span class="sxs-lookup"><span data-stu-id="e444c-128">Int64</span></span>  | <span data-ttu-id="e444c-129">Android デバイス上のアクティブ化の数。</span><span class="sxs-lookup"><span data-stu-id="e444c-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="e444c-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="e444c-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="e444c-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="e444c-131">Boolean</span></span> | <span data-ttu-id="e444c-132">ユーザーが共有する前にコンピューターに製品を使用する場合は true にします。</span><span class="sxs-lookup"><span data-stu-id="e444c-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e444c-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e444c-133">JSON representation</span></span>

<span data-ttu-id="e444c-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e444c-134">The following is a JSON representation of the resource.</span></span>

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
