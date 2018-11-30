---
title: ratingUnitedStatesTelevisionType 列挙型
description: アメリカ合衆国内のテレビ コンテンツの規制ラベル
ms.openlocfilehash: 7e962716e70c2cf88d70011843094ce9bebeb8b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072870"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="0adb7-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0adb7-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="0adb7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0adb7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0adb7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0adb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0adb7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0adb7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0adb7-107">アメリカ合衆国内のテレビ コンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="0adb7-107">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="0adb7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0adb7-108">Members</span></span>
|<span data-ttu-id="0adb7-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0adb7-109">Member</span></span>|<span data-ttu-id="0adb7-110">値</span><span class="sxs-lookup"><span data-stu-id="0adb7-110">Value</span></span>|<span data-ttu-id="0adb7-111">説明</span><span class="sxs-lookup"><span data-stu-id="0adb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0adb7-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="0adb7-112">allAllowed</span></span>|<span data-ttu-id="0adb7-113">0</span><span class="sxs-lookup"><span data-stu-id="0adb7-113">0</span></span>|<span data-ttu-id="0adb7-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="0adb7-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="0adb7-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="0adb7-115">allBlocked</span></span>|<span data-ttu-id="0adb7-116">1</span><span class="sxs-lookup"><span data-stu-id="0adb7-116">1</span></span>|<span data-ttu-id="0adb7-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="0adb7-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="0adb7-118">childrenAll</span><span class="sxs-lookup"><span data-stu-id="0adb7-118">childrenAll</span></span>|<span data-ttu-id="0adb7-119">2</span><span class="sxs-lookup"><span data-stu-id="0adb7-119">2</span></span>|<span data-ttu-id="0adb7-120">テレビ Y のすべての子</span><span class="sxs-lookup"><span data-stu-id="0adb7-120">TV-Y, all children</span></span>|
|<span data-ttu-id="0adb7-121">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="0adb7-121">childrenAbove7</span></span>|<span data-ttu-id="0adb7-122">3</span><span class="sxs-lookup"><span data-stu-id="0adb7-122">3</span></span>|<span data-ttu-id="0adb7-123">テレビ ・ Y7、子供の年齢 7 およびそれ以上</span><span class="sxs-lookup"><span data-stu-id="0adb7-123">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="0adb7-124">全般</span><span class="sxs-lookup"><span data-stu-id="0adb7-124">general</span></span>|<span data-ttu-id="0adb7-125">4</span><span class="sxs-lookup"><span data-stu-id="0adb7-125">4</span></span>|<span data-ttu-id="0adb7-126">テレビ G、一般ユーザー向け</span><span class="sxs-lookup"><span data-stu-id="0adb7-126">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="0adb7-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="0adb7-127">parentalGuidance</span></span>|<span data-ttu-id="0adb7-128">5</span><span class="sxs-lookup"><span data-stu-id="0adb7-128">5</span></span>|<span data-ttu-id="0adb7-129">テレビ PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="0adb7-129">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="0adb7-130">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="0adb7-130">childrenAbove14</span></span>|<span data-ttu-id="0adb7-131">6</span><span class="sxs-lookup"><span data-stu-id="0adb7-131">6</span></span>|<span data-ttu-id="0adb7-132">テレビ-14、子供時代の 14 以上の文字</span><span class="sxs-lookup"><span data-stu-id="0adb7-132">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="0adb7-133">大人</span><span class="sxs-lookup"><span data-stu-id="0adb7-133">adults</span></span>|<span data-ttu-id="0adb7-134">7</span><span class="sxs-lookup"><span data-stu-id="0adb7-134">7</span></span>|<span data-ttu-id="0adb7-135">テレビ MA、成人のみ</span><span class="sxs-lookup"><span data-stu-id="0adb7-135">TV-MA, adults only</span></span>|





