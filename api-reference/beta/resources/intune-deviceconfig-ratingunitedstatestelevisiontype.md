---
title: ratingUnitedStatesTelevisionType 列挙型
description: 米国でのテレビコンテンツ評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e280ad851e9d53b8c1dc2d000419d8aaa2d9c6c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771363"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="0b29e-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0b29e-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="0b29e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b29e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b29e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b29e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b29e-106">米国でのテレビコンテンツ評価のラベル</span><span class="sxs-lookup"><span data-stu-id="0b29e-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="0b29e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b29e-107">Members</span></span>
|<span data-ttu-id="0b29e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b29e-108">Member</span></span>|<span data-ttu-id="0b29e-109">値</span><span class="sxs-lookup"><span data-stu-id="0b29e-109">Value</span></span>|<span data-ttu-id="0b29e-110">説明</span><span class="sxs-lookup"><span data-stu-id="0b29e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b29e-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="0b29e-111">allAllowed</span></span>|<span data-ttu-id="0b29e-112">.0</span><span class="sxs-lookup"><span data-stu-id="0b29e-112">0</span></span>|<span data-ttu-id="0b29e-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="0b29e-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="0b29e-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="0b29e-114">allBlocked</span></span>|<span data-ttu-id="0b29e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0b29e-115">1</span></span>|<span data-ttu-id="0b29e-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="0b29e-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="0b29e-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="0b29e-117">childrenAll</span></span>|<span data-ttu-id="0b29e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0b29e-118">2</span></span>|<span data-ttu-id="0b29e-119">テレビ-Y、すべての子</span><span class="sxs-lookup"><span data-stu-id="0b29e-119">TV-Y, all children</span></span>|
|<span data-ttu-id="0b29e-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="0b29e-120">childrenAbove7</span></span>|<span data-ttu-id="0b29e-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0b29e-121">3</span></span>|<span data-ttu-id="0b29e-122">テレビ-Y7、子供の7歳以上</span><span class="sxs-lookup"><span data-stu-id="0b29e-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="0b29e-123">元帳</span><span class="sxs-lookup"><span data-stu-id="0b29e-123">general</span></span>|<span data-ttu-id="0b29e-124">2/4</span><span class="sxs-lookup"><span data-stu-id="0b29e-124">4</span></span>|<span data-ttu-id="0b29e-125">テレビ-G (すべての年齢に適している)</span><span class="sxs-lookup"><span data-stu-id="0b29e-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="0b29e-126">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="0b29e-126">parentalGuidance</span></span>|<span data-ttu-id="0b29e-127">5</span><span class="sxs-lookup"><span data-stu-id="0b29e-127">5</span></span>|<span data-ttu-id="0b29e-128">テレビ-PG、保護者によるガイダンス</span><span class="sxs-lookup"><span data-stu-id="0b29e-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="0b29e-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="0b29e-129">childrenAbove14</span></span>|<span data-ttu-id="0b29e-130">シックス</span><span class="sxs-lookup"><span data-stu-id="0b29e-130">6</span></span>|<span data-ttu-id="0b29e-131">TV-14 歳以上の子供</span><span class="sxs-lookup"><span data-stu-id="0b29e-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="0b29e-132">保護者</span><span class="sxs-lookup"><span data-stu-id="0b29e-132">adults</span></span>|<span data-ttu-id="0b29e-133">7</span><span class="sxs-lookup"><span data-stu-id="0b29e-133">7</span></span>|<span data-ttu-id="0b29e-134">テレビ-MA、大人のみ</span><span class="sxs-lookup"><span data-stu-id="0b29e-134">TV-MA, adults only</span></span>|





