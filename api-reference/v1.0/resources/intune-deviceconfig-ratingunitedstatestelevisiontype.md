---
title: ratingUnitedStatesTelevisionType 列挙型
description: アメリカ合衆国内のテレビ コンテンツの規制ラベル
ms.openlocfilehash: bb0a977294d8236205b6d6bdf6311db75e377951
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024163"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="ae83f-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ae83f-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="ae83f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae83f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae83f-105">アメリカ合衆国内のテレビ コンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="ae83f-105">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="ae83f-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae83f-106">Members</span></span>
|<span data-ttu-id="ae83f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae83f-107">Member</span></span>|<span data-ttu-id="ae83f-108">値</span><span class="sxs-lookup"><span data-stu-id="ae83f-108">Value</span></span>|<span data-ttu-id="ae83f-109">説明</span><span class="sxs-lookup"><span data-stu-id="ae83f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae83f-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="ae83f-110">allAllowed</span></span>|<span data-ttu-id="ae83f-111">0</span><span class="sxs-lookup"><span data-stu-id="ae83f-111">0</span></span>|<span data-ttu-id="ae83f-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="ae83f-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="ae83f-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="ae83f-113">allBlocked</span></span>|<span data-ttu-id="ae83f-114">1</span><span class="sxs-lookup"><span data-stu-id="ae83f-114">1</span></span>|<span data-ttu-id="ae83f-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="ae83f-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="ae83f-116">childrenAll</span><span class="sxs-lookup"><span data-stu-id="ae83f-116">childrenAll</span></span>|<span data-ttu-id="ae83f-117">2</span><span class="sxs-lookup"><span data-stu-id="ae83f-117">2</span></span>|<span data-ttu-id="ae83f-118">テレビ Y のすべての子</span><span class="sxs-lookup"><span data-stu-id="ae83f-118">TV-Y, all children</span></span>|
|<span data-ttu-id="ae83f-119">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="ae83f-119">childrenAbove7</span></span>|<span data-ttu-id="ae83f-120">3</span><span class="sxs-lookup"><span data-stu-id="ae83f-120">3</span></span>|<span data-ttu-id="ae83f-121">テレビ ・ Y7、子供の年齢 7 およびそれ以上</span><span class="sxs-lookup"><span data-stu-id="ae83f-121">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="ae83f-122">全般</span><span class="sxs-lookup"><span data-stu-id="ae83f-122">general</span></span>|<span data-ttu-id="ae83f-123">4</span><span class="sxs-lookup"><span data-stu-id="ae83f-123">4</span></span>|<span data-ttu-id="ae83f-124">テレビ G、一般ユーザー向け</span><span class="sxs-lookup"><span data-stu-id="ae83f-124">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="ae83f-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="ae83f-125">parentalGuidance</span></span>|<span data-ttu-id="ae83f-126">5</span><span class="sxs-lookup"><span data-stu-id="ae83f-126">5</span></span>|<span data-ttu-id="ae83f-127">テレビ PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="ae83f-127">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="ae83f-128">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="ae83f-128">childrenAbove14</span></span>|<span data-ttu-id="ae83f-129">6</span><span class="sxs-lookup"><span data-stu-id="ae83f-129">6</span></span>|<span data-ttu-id="ae83f-130">テレビ-14、子供時代の 14 以上の文字</span><span class="sxs-lookup"><span data-stu-id="ae83f-130">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="ae83f-131">大人</span><span class="sxs-lookup"><span data-stu-id="ae83f-131">adults</span></span>|<span data-ttu-id="ae83f-132">7</span><span class="sxs-lookup"><span data-stu-id="ae83f-132">7</span></span>|<span data-ttu-id="ae83f-133">テレビ MA、成人のみ</span><span class="sxs-lookup"><span data-stu-id="ae83f-133">TV-MA, adults only</span></span>|



