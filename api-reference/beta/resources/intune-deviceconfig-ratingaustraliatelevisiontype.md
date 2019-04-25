---
title: ratingAustraliaTelevisionType 列挙型
description: オーストラリアでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a65d8b272e99a3a8432214b3ac51916bc6e9f50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566704"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="591df-103">ratingAustraliaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="591df-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="591df-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="591df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="591df-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="591df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="591df-106">オーストラリアでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="591df-106">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="591df-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="591df-107">Members</span></span>
|<span data-ttu-id="591df-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="591df-108">Member</span></span>|<span data-ttu-id="591df-109">値</span><span class="sxs-lookup"><span data-stu-id="591df-109">Value</span></span>|<span data-ttu-id="591df-110">説明</span><span class="sxs-lookup"><span data-stu-id="591df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="591df-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="591df-111">allAllowed</span></span>|<span data-ttu-id="591df-112">.0</span><span class="sxs-lookup"><span data-stu-id="591df-112">0</span></span>|<span data-ttu-id="591df-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="591df-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="591df-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="591df-114">allBlocked</span></span>|<span data-ttu-id="591df-115">1 </span><span class="sxs-lookup"><span data-stu-id="591df-115">1</span></span>|<span data-ttu-id="591df-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="591df-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="591df-117">prespreser</span><span class="sxs-lookup"><span data-stu-id="591df-117">preschoolers</span></span>|<span data-ttu-id="591df-118">2 </span><span class="sxs-lookup"><span data-stu-id="591df-118">2</span></span>|<span data-ttu-id="591df-119">P 分類は、preschoolers に対して使用されます。</span><span class="sxs-lookup"><span data-stu-id="591df-119">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="591df-120">children</span><span class="sxs-lookup"><span data-stu-id="591df-120">children</span></span>|<span data-ttu-id="591df-121">3 </span><span class="sxs-lookup"><span data-stu-id="591df-121">3</span></span>|<span data-ttu-id="591df-122">C の分類は、14の下の子を対象としています。</span><span class="sxs-lookup"><span data-stu-id="591df-122">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="591df-123">元帳</span><span class="sxs-lookup"><span data-stu-id="591df-123">general</span></span>|<span data-ttu-id="591df-124">4 </span><span class="sxs-lookup"><span data-stu-id="591df-124">4</span></span>|<span data-ttu-id="591df-125">G 分類は、すべての年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="591df-125">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="591df-126">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="591df-126">parentalGuidance</span></span>|<span data-ttu-id="591df-127">5 </span><span class="sxs-lookup"><span data-stu-id="591df-127">5</span></span>|<span data-ttu-id="591df-128">閲覧者には PG 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="591df-128">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="591df-129">度</span><span class="sxs-lookup"><span data-stu-id="591df-129">mature</span></span>|<span data-ttu-id="591df-130">6 </span><span class="sxs-lookup"><span data-stu-id="591df-130">6</span></span>|<span data-ttu-id="591df-131">15を超える閲覧者には M 分類が推奨されています</span><span class="sxs-lookup"><span data-stu-id="591df-131">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="591df-132">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="591df-132">agesAbove15</span></span>|<span data-ttu-id="591df-133">7 </span><span class="sxs-lookup"><span data-stu-id="591df-133">7</span></span>|<span data-ttu-id="591df-134">MA15 + 分類は15以下の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="591df-134">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="591df-135">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="591df-135">agesAbove15AdultViolence</span></span>|<span data-ttu-id="591df-136">8 </span><span class="sxs-lookup"><span data-stu-id="591df-136">8</span></span>|<span data-ttu-id="591df-137">AV15 + 分類は、15の下の閲覧者には適していません。成人の暴力に固有のものです。</span><span class="sxs-lookup"><span data-stu-id="591df-137">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|





