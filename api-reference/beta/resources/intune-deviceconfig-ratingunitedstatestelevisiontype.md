---
title: ratingUnitedStatesTelevisionType 列挙型
description: 米国でのテレビコンテンツ評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d016565ba9fdbb62ea24d39d52f0e2931bab3117
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166837"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="81196-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="81196-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="81196-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81196-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81196-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81196-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81196-106">米国でのテレビコンテンツ評価のラベル</span><span class="sxs-lookup"><span data-stu-id="81196-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="81196-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="81196-107">Members</span></span>
|<span data-ttu-id="81196-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="81196-108">Member</span></span>|<span data-ttu-id="81196-109">値</span><span class="sxs-lookup"><span data-stu-id="81196-109">Value</span></span>|<span data-ttu-id="81196-110">説明</span><span class="sxs-lookup"><span data-stu-id="81196-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81196-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="81196-111">allAllowed</span></span>|<span data-ttu-id="81196-112">.0</span><span class="sxs-lookup"><span data-stu-id="81196-112">0</span></span>|<span data-ttu-id="81196-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="81196-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="81196-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="81196-114">allBlocked</span></span>|<span data-ttu-id="81196-115">1-d</span><span class="sxs-lookup"><span data-stu-id="81196-115">1</span></span>|<span data-ttu-id="81196-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="81196-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="81196-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="81196-117">childrenAll</span></span>|<span data-ttu-id="81196-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="81196-118">2</span></span>|<span data-ttu-id="81196-119">テレビ-Y、すべての子</span><span class="sxs-lookup"><span data-stu-id="81196-119">TV-Y, all children</span></span>|
|<span data-ttu-id="81196-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="81196-120">childrenAbove7</span></span>|<span data-ttu-id="81196-121">1/3</span><span class="sxs-lookup"><span data-stu-id="81196-121">3</span></span>|<span data-ttu-id="81196-122">テレビ-Y7、子供の7歳以上</span><span class="sxs-lookup"><span data-stu-id="81196-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="81196-123">元帳</span><span class="sxs-lookup"><span data-stu-id="81196-123">general</span></span>|<span data-ttu-id="81196-124">2/4</span><span class="sxs-lookup"><span data-stu-id="81196-124">4</span></span>|<span data-ttu-id="81196-125">テレビ-G (すべての年齢に適している)</span><span class="sxs-lookup"><span data-stu-id="81196-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="81196-126">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="81196-126">parentalGuidance</span></span>|<span data-ttu-id="81196-127">5</span><span class="sxs-lookup"><span data-stu-id="81196-127">5</span></span>|<span data-ttu-id="81196-128">テレビ-PG、保護者によるガイダンス</span><span class="sxs-lookup"><span data-stu-id="81196-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="81196-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="81196-129">childrenAbove14</span></span>|<span data-ttu-id="81196-130">シックス</span><span class="sxs-lookup"><span data-stu-id="81196-130">6</span></span>|<span data-ttu-id="81196-131">TV-14 歳以上の子供</span><span class="sxs-lookup"><span data-stu-id="81196-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="81196-132">保護者</span><span class="sxs-lookup"><span data-stu-id="81196-132">adults</span></span>|<span data-ttu-id="81196-133">7</span><span class="sxs-lookup"><span data-stu-id="81196-133">7</span></span>|<span data-ttu-id="81196-134">テレビ-MA、大人のみ</span><span class="sxs-lookup"><span data-stu-id="81196-134">TV-MA, adults only</span></span>|




