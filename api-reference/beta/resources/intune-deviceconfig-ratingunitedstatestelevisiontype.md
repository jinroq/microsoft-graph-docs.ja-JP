---
title: ratingUnitedStatesTelevisionType 列挙型
description: 米国でのテレビコンテンツ評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e280ad851e9d53b8c1dc2d000419d8aaa2d9c6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555221"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="741d9-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="741d9-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="741d9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="741d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="741d9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="741d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="741d9-106">米国でのテレビコンテンツ評価のラベル</span><span class="sxs-lookup"><span data-stu-id="741d9-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="741d9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="741d9-107">Members</span></span>
|<span data-ttu-id="741d9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="741d9-108">Member</span></span>|<span data-ttu-id="741d9-109">値</span><span class="sxs-lookup"><span data-stu-id="741d9-109">Value</span></span>|<span data-ttu-id="741d9-110">説明</span><span class="sxs-lookup"><span data-stu-id="741d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="741d9-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="741d9-111">allAllowed</span></span>|<span data-ttu-id="741d9-112">.0</span><span class="sxs-lookup"><span data-stu-id="741d9-112">0</span></span>|<span data-ttu-id="741d9-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="741d9-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="741d9-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="741d9-114">allBlocked</span></span>|<span data-ttu-id="741d9-115">1 </span><span class="sxs-lookup"><span data-stu-id="741d9-115">1</span></span>|<span data-ttu-id="741d9-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="741d9-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="741d9-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="741d9-117">childrenAll</span></span>|<span data-ttu-id="741d9-118">2 </span><span class="sxs-lookup"><span data-stu-id="741d9-118">2</span></span>|<span data-ttu-id="741d9-119">テレビ-Y、すべての子</span><span class="sxs-lookup"><span data-stu-id="741d9-119">TV-Y, all children</span></span>|
|<span data-ttu-id="741d9-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="741d9-120">childrenAbove7</span></span>|<span data-ttu-id="741d9-121">3 </span><span class="sxs-lookup"><span data-stu-id="741d9-121">3</span></span>|<span data-ttu-id="741d9-122">テレビ-Y7、子供の7歳以上</span><span class="sxs-lookup"><span data-stu-id="741d9-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="741d9-123">元帳</span><span class="sxs-lookup"><span data-stu-id="741d9-123">general</span></span>|<span data-ttu-id="741d9-124">4 </span><span class="sxs-lookup"><span data-stu-id="741d9-124">4</span></span>|<span data-ttu-id="741d9-125">テレビ-G (すべての年齢に適している)</span><span class="sxs-lookup"><span data-stu-id="741d9-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="741d9-126">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="741d9-126">parentalGuidance</span></span>|<span data-ttu-id="741d9-127">5 </span><span class="sxs-lookup"><span data-stu-id="741d9-127">5</span></span>|<span data-ttu-id="741d9-128">テレビ-PG、保護者によるガイダンス</span><span class="sxs-lookup"><span data-stu-id="741d9-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="741d9-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="741d9-129">childrenAbove14</span></span>|<span data-ttu-id="741d9-130">6 </span><span class="sxs-lookup"><span data-stu-id="741d9-130">6</span></span>|<span data-ttu-id="741d9-131">TV-14 歳以上の子供</span><span class="sxs-lookup"><span data-stu-id="741d9-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="741d9-132">保護者</span><span class="sxs-lookup"><span data-stu-id="741d9-132">adults</span></span>|<span data-ttu-id="741d9-133">7 </span><span class="sxs-lookup"><span data-stu-id="741d9-133">7</span></span>|<span data-ttu-id="741d9-134">テレビ-MA、大人のみ</span><span class="sxs-lookup"><span data-stu-id="741d9-134">TV-MA, adults only</span></span>|





