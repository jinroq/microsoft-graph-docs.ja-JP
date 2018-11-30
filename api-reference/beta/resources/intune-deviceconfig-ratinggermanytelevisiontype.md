---
title: ratingGermanyTelevisionType 列挙型
description: ドイツのテレビのコンテンツの規制ラベル
ms.openlocfilehash: 615ccc0fbd0d155a4db9c1dc25e6478d916448a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066949"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="5d2b9-103">ratingGermanyTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5d2b9-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="5d2b9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d2b9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d2b9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d2b9-107">ドイツのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="5d2b9-107">TV content rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="5d2b9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5d2b9-108">Members</span></span>
|<span data-ttu-id="5d2b9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5d2b9-109">Member</span></span>|<span data-ttu-id="5d2b9-110">値</span><span class="sxs-lookup"><span data-stu-id="5d2b9-110">Value</span></span>|<span data-ttu-id="5d2b9-111">説明</span><span class="sxs-lookup"><span data-stu-id="5d2b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d2b9-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="5d2b9-112">allAllowed</span></span>|<span data-ttu-id="5d2b9-113">0</span><span class="sxs-lookup"><span data-stu-id="5d2b9-113">0</span></span>|<span data-ttu-id="5d2b9-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="5d2b9-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="5d2b9-115">allBlocked</span></span>|<span data-ttu-id="5d2b9-116">1</span><span class="sxs-lookup"><span data-stu-id="5d2b9-116">1</span></span>|<span data-ttu-id="5d2b9-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="5d2b9-118">全般</span><span class="sxs-lookup"><span data-stu-id="5d2b9-118">general</span></span>|<span data-ttu-id="5d2b9-119">2</span><span class="sxs-lookup"><span data-stu-id="5d2b9-119">2</span></span>|<span data-ttu-id="5d2b9-120">Ab 0 Jahren、年齢制限はありません。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="5d2b9-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="5d2b9-121">agesAbove6</span></span>|<span data-ttu-id="5d2b9-122">3</span><span class="sxs-lookup"><span data-stu-id="5d2b9-122">3</span></span>|<span data-ttu-id="5d2b9-123">Ab 6 Jahren では、6 と以前のエージングします。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="5d2b9-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="5d2b9-124">agesAbove12</span></span>|<span data-ttu-id="5d2b9-125">4</span><span class="sxs-lookup"><span data-stu-id="5d2b9-125">4</span></span>|<span data-ttu-id="5d2b9-126">Ab 12 Jahren、12 と古いのエージングします。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="5d2b9-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="5d2b9-127">agesAbove16</span></span>|<span data-ttu-id="5d2b9-128">5</span><span class="sxs-lookup"><span data-stu-id="5d2b9-128">5</span></span>|<span data-ttu-id="5d2b9-129">Ab 16 Jahren、16 のエージングします。</span><span class="sxs-lookup"><span data-stu-id="5d2b9-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="5d2b9-130">大人</span><span class="sxs-lookup"><span data-stu-id="5d2b9-130">adults</span></span>|<span data-ttu-id="5d2b9-131">6</span><span class="sxs-lookup"><span data-stu-id="5d2b9-131">6</span></span>|<span data-ttu-id="5d2b9-132">Ab 18 Jahren、成人のみ</span><span class="sxs-lookup"><span data-stu-id="5d2b9-132">Ab 18 Jahren, adults only</span></span>|





