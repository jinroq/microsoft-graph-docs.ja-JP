---
title: ratingUnitedStatesTelevisionType 列挙型
description: アメリカ合衆国内のテレビ コンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9f4492fac5bc003fdaba15a39b0f58892872ea87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964803"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="d3ba0-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d3ba0-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="d3ba0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d3ba0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3ba0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3ba0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3ba0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3ba0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3ba0-107">アメリカ合衆国内のテレビ コンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="d3ba0-107">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="d3ba0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3ba0-108">Members</span></span>
|<span data-ttu-id="d3ba0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3ba0-109">Member</span></span>|<span data-ttu-id="d3ba0-110">値</span><span class="sxs-lookup"><span data-stu-id="d3ba0-110">Value</span></span>|<span data-ttu-id="d3ba0-111">説明</span><span class="sxs-lookup"><span data-stu-id="d3ba0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3ba0-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="d3ba0-112">allAllowed</span></span>|<span data-ttu-id="d3ba0-113">0</span><span class="sxs-lookup"><span data-stu-id="d3ba0-113">0</span></span>|<span data-ttu-id="d3ba0-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="d3ba0-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="d3ba0-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="d3ba0-115">allBlocked</span></span>|<span data-ttu-id="d3ba0-116">1</span><span class="sxs-lookup"><span data-stu-id="d3ba0-116">1</span></span>|<span data-ttu-id="d3ba0-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="d3ba0-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="d3ba0-118">childrenAll</span><span class="sxs-lookup"><span data-stu-id="d3ba0-118">childrenAll</span></span>|<span data-ttu-id="d3ba0-119">2</span><span class="sxs-lookup"><span data-stu-id="d3ba0-119">2</span></span>|<span data-ttu-id="d3ba0-120">テレビ Y のすべての子</span><span class="sxs-lookup"><span data-stu-id="d3ba0-120">TV-Y, all children</span></span>|
|<span data-ttu-id="d3ba0-121">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="d3ba0-121">childrenAbove7</span></span>|<span data-ttu-id="d3ba0-122">3</span><span class="sxs-lookup"><span data-stu-id="d3ba0-122">3</span></span>|<span data-ttu-id="d3ba0-123">テレビ ・ Y7、子供の年齢 7 およびそれ以上</span><span class="sxs-lookup"><span data-stu-id="d3ba0-123">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="d3ba0-124">全般</span><span class="sxs-lookup"><span data-stu-id="d3ba0-124">general</span></span>|<span data-ttu-id="d3ba0-125">4</span><span class="sxs-lookup"><span data-stu-id="d3ba0-125">4</span></span>|<span data-ttu-id="d3ba0-126">テレビ G、一般ユーザー向け</span><span class="sxs-lookup"><span data-stu-id="d3ba0-126">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="d3ba0-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="d3ba0-127">parentalGuidance</span></span>|<span data-ttu-id="d3ba0-128">5</span><span class="sxs-lookup"><span data-stu-id="d3ba0-128">5</span></span>|<span data-ttu-id="d3ba0-129">テレビ PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="d3ba0-129">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="d3ba0-130">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="d3ba0-130">childrenAbove14</span></span>|<span data-ttu-id="d3ba0-131">6</span><span class="sxs-lookup"><span data-stu-id="d3ba0-131">6</span></span>|<span data-ttu-id="d3ba0-132">テレビ-14、子供時代の 14 以上の文字</span><span class="sxs-lookup"><span data-stu-id="d3ba0-132">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="d3ba0-133">大人</span><span class="sxs-lookup"><span data-stu-id="d3ba0-133">adults</span></span>|<span data-ttu-id="d3ba0-134">7</span><span class="sxs-lookup"><span data-stu-id="d3ba0-134">7</span></span>|<span data-ttu-id="d3ba0-135">テレビ MA、成人のみ</span><span class="sxs-lookup"><span data-stu-id="d3ba0-135">TV-MA, adults only</span></span>|





