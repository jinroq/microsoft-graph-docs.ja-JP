---
title: ratingUnitedStatesTelevisionType 列挙型
description: 米国でのテレビコンテンツ評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86ee28f600ae9f1e55f09d3d7db794fd55c79281
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534753"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="56113-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="56113-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="56113-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="56113-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56113-105">米国でのテレビコンテンツ評価のラベル</span><span class="sxs-lookup"><span data-stu-id="56113-105">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="56113-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="56113-106">Members</span></span>
|<span data-ttu-id="56113-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="56113-107">Member</span></span>|<span data-ttu-id="56113-108">値</span><span class="sxs-lookup"><span data-stu-id="56113-108">Value</span></span>|<span data-ttu-id="56113-109">説明</span><span class="sxs-lookup"><span data-stu-id="56113-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56113-110">allallowed</span><span class="sxs-lookup"><span data-stu-id="56113-110">allAllowed</span></span>|<span data-ttu-id="56113-111">.0</span><span class="sxs-lookup"><span data-stu-id="56113-111">0</span></span>|<span data-ttu-id="56113-112">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="56113-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="56113-113">allblocked</span><span class="sxs-lookup"><span data-stu-id="56113-113">allBlocked</span></span>|<span data-ttu-id="56113-114">1 </span><span class="sxs-lookup"><span data-stu-id="56113-114">1</span></span>|<span data-ttu-id="56113-115">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="56113-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="56113-116">childrenAll</span><span class="sxs-lookup"><span data-stu-id="56113-116">childrenAll</span></span>|<span data-ttu-id="56113-117">2 </span><span class="sxs-lookup"><span data-stu-id="56113-117">2</span></span>|<span data-ttu-id="56113-118">テレビ-Y、すべての子</span><span class="sxs-lookup"><span data-stu-id="56113-118">TV-Y, all children</span></span>|
|<span data-ttu-id="56113-119">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="56113-119">childrenAbove7</span></span>|<span data-ttu-id="56113-120">3 </span><span class="sxs-lookup"><span data-stu-id="56113-120">3</span></span>|<span data-ttu-id="56113-121">テレビ-Y7、子供の7歳以上</span><span class="sxs-lookup"><span data-stu-id="56113-121">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="56113-122">元帳</span><span class="sxs-lookup"><span data-stu-id="56113-122">general</span></span>|<span data-ttu-id="56113-123">4 </span><span class="sxs-lookup"><span data-stu-id="56113-123">4</span></span>|<span data-ttu-id="56113-124">テレビ-G (すべての年齢に適している)</span><span class="sxs-lookup"><span data-stu-id="56113-124">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="56113-125">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="56113-125">parentalGuidance</span></span>|<span data-ttu-id="56113-126">5 </span><span class="sxs-lookup"><span data-stu-id="56113-126">5</span></span>|<span data-ttu-id="56113-127">テレビ-PG、保護者によるガイダンス</span><span class="sxs-lookup"><span data-stu-id="56113-127">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="56113-128">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="56113-128">childrenAbove14</span></span>|<span data-ttu-id="56113-129">6 </span><span class="sxs-lookup"><span data-stu-id="56113-129">6</span></span>|<span data-ttu-id="56113-130">TV-14 歳以上の子供</span><span class="sxs-lookup"><span data-stu-id="56113-130">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="56113-131">保護者</span><span class="sxs-lookup"><span data-stu-id="56113-131">adults</span></span>|<span data-ttu-id="56113-132">7 </span><span class="sxs-lookup"><span data-stu-id="56113-132">7</span></span>|<span data-ttu-id="56113-133">テレビ-MA、大人のみ</span><span class="sxs-lookup"><span data-stu-id="56113-133">TV-MA, adults only</span></span>|



