---
title: ratingUnitedStatesTelevisionType 列挙型
description: アメリカ合衆国内のテレビ コンテンツの規制ラベル
author: tfitzmac
ms.openlocfilehash: 2b03a053851248bcd1238b2464c2a4f8879a5580
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328386"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="a0f4e-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a0f4e-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="a0f4e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a0f4e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0f4e-105">アメリカ合衆国内のテレビ コンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="a0f4e-105">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="a0f4e-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a0f4e-106">Members</span></span>
|<span data-ttu-id="a0f4e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a0f4e-107">Member</span></span>|<span data-ttu-id="a0f4e-108">値</span><span class="sxs-lookup"><span data-stu-id="a0f4e-108">Value</span></span>|<span data-ttu-id="a0f4e-109">説明</span><span class="sxs-lookup"><span data-stu-id="a0f4e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0f4e-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="a0f4e-110">allAllowed</span></span>|<span data-ttu-id="a0f4e-111">0</span><span class="sxs-lookup"><span data-stu-id="a0f4e-111">0</span></span>|<span data-ttu-id="a0f4e-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="a0f4e-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="a0f4e-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="a0f4e-113">allBlocked</span></span>|<span data-ttu-id="a0f4e-114">1</span><span class="sxs-lookup"><span data-stu-id="a0f4e-114">1</span></span>|<span data-ttu-id="a0f4e-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="a0f4e-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="a0f4e-116">childrenAll</span><span class="sxs-lookup"><span data-stu-id="a0f4e-116">childrenAll</span></span>|<span data-ttu-id="a0f4e-117">2</span><span class="sxs-lookup"><span data-stu-id="a0f4e-117">2</span></span>|<span data-ttu-id="a0f4e-118">テレビ Y のすべての子</span><span class="sxs-lookup"><span data-stu-id="a0f4e-118">TV-Y, all children</span></span>|
|<span data-ttu-id="a0f4e-119">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="a0f4e-119">childrenAbove7</span></span>|<span data-ttu-id="a0f4e-120">3</span><span class="sxs-lookup"><span data-stu-id="a0f4e-120">3</span></span>|<span data-ttu-id="a0f4e-121">テレビ ・ Y7、子供の年齢 7 およびそれ以上</span><span class="sxs-lookup"><span data-stu-id="a0f4e-121">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="a0f4e-122">全般</span><span class="sxs-lookup"><span data-stu-id="a0f4e-122">general</span></span>|<span data-ttu-id="a0f4e-123">4</span><span class="sxs-lookup"><span data-stu-id="a0f4e-123">4</span></span>|<span data-ttu-id="a0f4e-124">テレビ G、一般ユーザー向け</span><span class="sxs-lookup"><span data-stu-id="a0f4e-124">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="a0f4e-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="a0f4e-125">parentalGuidance</span></span>|<span data-ttu-id="a0f4e-126">5</span><span class="sxs-lookup"><span data-stu-id="a0f4e-126">5</span></span>|<span data-ttu-id="a0f4e-127">テレビ PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="a0f4e-127">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="a0f4e-128">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="a0f4e-128">childrenAbove14</span></span>|<span data-ttu-id="a0f4e-129">6</span><span class="sxs-lookup"><span data-stu-id="a0f4e-129">6</span></span>|<span data-ttu-id="a0f4e-130">テレビ-14、子供時代の 14 以上の文字</span><span class="sxs-lookup"><span data-stu-id="a0f4e-130">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="a0f4e-131">大人</span><span class="sxs-lookup"><span data-stu-id="a0f4e-131">adults</span></span>|<span data-ttu-id="a0f4e-132">7</span><span class="sxs-lookup"><span data-stu-id="a0f4e-132">7</span></span>|<span data-ttu-id="a0f4e-133">テレビ MA、成人のみ</span><span class="sxs-lookup"><span data-stu-id="a0f4e-133">TV-MA, adults only</span></span>|



