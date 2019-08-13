---
title: ratingUnitedStatesTelevisionType 列挙型
description: 米国でのテレビコンテンツ評価のラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 142552da06e0c07fca3d8a59e23ebe536c709495
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368122"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="c533f-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c533f-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="c533f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c533f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c533f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c533f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c533f-106">米国でのテレビコンテンツ評価のラベル</span><span class="sxs-lookup"><span data-stu-id="c533f-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="c533f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c533f-107">Members</span></span>
|<span data-ttu-id="c533f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c533f-108">Member</span></span>|<span data-ttu-id="c533f-109">値</span><span class="sxs-lookup"><span data-stu-id="c533f-109">Value</span></span>|<span data-ttu-id="c533f-110">説明</span><span class="sxs-lookup"><span data-stu-id="c533f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c533f-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="c533f-111">allAllowed</span></span>|<span data-ttu-id="c533f-112">.0</span><span class="sxs-lookup"><span data-stu-id="c533f-112">0</span></span>|<span data-ttu-id="c533f-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="c533f-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="c533f-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="c533f-114">allBlocked</span></span>|<span data-ttu-id="c533f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c533f-115">1</span></span>|<span data-ttu-id="c533f-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="c533f-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="c533f-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="c533f-117">childrenAll</span></span>|<span data-ttu-id="c533f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c533f-118">2</span></span>|<span data-ttu-id="c533f-119">テレビ-Y、すべての子</span><span class="sxs-lookup"><span data-stu-id="c533f-119">TV-Y, all children</span></span>|
|<span data-ttu-id="c533f-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="c533f-120">childrenAbove7</span></span>|<span data-ttu-id="c533f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="c533f-121">3</span></span>|<span data-ttu-id="c533f-122">テレビ-Y7、子供の7歳以上</span><span class="sxs-lookup"><span data-stu-id="c533f-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="c533f-123">元帳</span><span class="sxs-lookup"><span data-stu-id="c533f-123">general</span></span>|<span data-ttu-id="c533f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="c533f-124">4</span></span>|<span data-ttu-id="c533f-125">テレビ-G (すべての年齢に適している)</span><span class="sxs-lookup"><span data-stu-id="c533f-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="c533f-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="c533f-126">parentalGuidance</span></span>|<span data-ttu-id="c533f-127">5</span><span class="sxs-lookup"><span data-stu-id="c533f-127">5</span></span>|<span data-ttu-id="c533f-128">テレビ-PG、保護者によるガイダンス</span><span class="sxs-lookup"><span data-stu-id="c533f-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="c533f-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="c533f-129">childrenAbove14</span></span>|<span data-ttu-id="c533f-130">シックス</span><span class="sxs-lookup"><span data-stu-id="c533f-130">6</span></span>|<span data-ttu-id="c533f-131">TV-14 歳以上の子供</span><span class="sxs-lookup"><span data-stu-id="c533f-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="c533f-132">保護者</span><span class="sxs-lookup"><span data-stu-id="c533f-132">adults</span></span>|<span data-ttu-id="c533f-133">7</span><span class="sxs-lookup"><span data-stu-id="c533f-133">7</span></span>|<span data-ttu-id="c533f-134">テレビ-MA、大人のみ</span><span class="sxs-lookup"><span data-stu-id="c533f-134">TV-MA, adults only</span></span>|



