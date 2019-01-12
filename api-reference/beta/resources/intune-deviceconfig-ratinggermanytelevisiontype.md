---
title: ratingGermanyTelevisionType 列挙型
description: ドイツのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1f5f2a27a86151244dd7b2db3d160e8e570a61f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947667"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="23f27-103">ratingGermanyTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="23f27-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="23f27-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23f27-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23f27-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23f27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23f27-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="23f27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23f27-107">ドイツのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="23f27-107">TV content rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="23f27-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="23f27-108">Members</span></span>
|<span data-ttu-id="23f27-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="23f27-109">Member</span></span>|<span data-ttu-id="23f27-110">値</span><span class="sxs-lookup"><span data-stu-id="23f27-110">Value</span></span>|<span data-ttu-id="23f27-111">説明</span><span class="sxs-lookup"><span data-stu-id="23f27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23f27-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="23f27-112">allAllowed</span></span>|<span data-ttu-id="23f27-113">0</span><span class="sxs-lookup"><span data-stu-id="23f27-113">0</span></span>|<span data-ttu-id="23f27-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="23f27-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="23f27-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="23f27-115">allBlocked</span></span>|<span data-ttu-id="23f27-116">1</span><span class="sxs-lookup"><span data-stu-id="23f27-116">1</span></span>|<span data-ttu-id="23f27-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="23f27-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="23f27-118">全般</span><span class="sxs-lookup"><span data-stu-id="23f27-118">general</span></span>|<span data-ttu-id="23f27-119">2</span><span class="sxs-lookup"><span data-stu-id="23f27-119">2</span></span>|<span data-ttu-id="23f27-120">Ab 0 Jahren、年齢制限はありません。</span><span class="sxs-lookup"><span data-stu-id="23f27-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="23f27-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="23f27-121">agesAbove6</span></span>|<span data-ttu-id="23f27-122">3</span><span class="sxs-lookup"><span data-stu-id="23f27-122">3</span></span>|<span data-ttu-id="23f27-123">Ab 6 Jahren では、6 と以前のエージングします。</span><span class="sxs-lookup"><span data-stu-id="23f27-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="23f27-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="23f27-124">agesAbove12</span></span>|<span data-ttu-id="23f27-125">4</span><span class="sxs-lookup"><span data-stu-id="23f27-125">4</span></span>|<span data-ttu-id="23f27-126">Ab 12 Jahren、12 と古いのエージングします。</span><span class="sxs-lookup"><span data-stu-id="23f27-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="23f27-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="23f27-127">agesAbove16</span></span>|<span data-ttu-id="23f27-128">5</span><span class="sxs-lookup"><span data-stu-id="23f27-128">5</span></span>|<span data-ttu-id="23f27-129">Ab 16 Jahren、16 のエージングします。</span><span class="sxs-lookup"><span data-stu-id="23f27-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="23f27-130">大人</span><span class="sxs-lookup"><span data-stu-id="23f27-130">adults</span></span>|<span data-ttu-id="23f27-131">6</span><span class="sxs-lookup"><span data-stu-id="23f27-131">6</span></span>|<span data-ttu-id="23f27-132">Ab 18 Jahren、成人のみ</span><span class="sxs-lookup"><span data-stu-id="23f27-132">Ab 18 Jahren, adults only</span></span>|





