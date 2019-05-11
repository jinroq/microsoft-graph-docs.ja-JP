---
title: ratingJapanMoviesType 列挙型
description: 日本の映画の視聴制限ラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1fa023e6f875c14618483185d90e6e793a2441e9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950873"
---
# <a name="ratingjapanmoviestype-enum-type"></a><span data-ttu-id="68426-103">ratingJapanMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="68426-103">ratingJapanMoviesType enum type</span></span>

> <span data-ttu-id="68426-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68426-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68426-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68426-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68426-106">日本の映画の視聴制限ラベル</span><span class="sxs-lookup"><span data-stu-id="68426-106">Movies rating labels in Japan</span></span>

## <a name="members"></a><span data-ttu-id="68426-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="68426-107">Members</span></span>
|<span data-ttu-id="68426-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="68426-108">Member</span></span>|<span data-ttu-id="68426-109">値</span><span class="sxs-lookup"><span data-stu-id="68426-109">Value</span></span>|<span data-ttu-id="68426-110">説明</span><span class="sxs-lookup"><span data-stu-id="68426-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68426-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="68426-111">allAllowed</span></span>|<span data-ttu-id="68426-112">.0</span><span class="sxs-lookup"><span data-stu-id="68426-112">0</span></span>|<span data-ttu-id="68426-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="68426-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="68426-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="68426-114">allBlocked</span></span>|<span data-ttu-id="68426-115">1-d</span><span class="sxs-lookup"><span data-stu-id="68426-115">1</span></span>|<span data-ttu-id="68426-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="68426-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="68426-117">元帳</span><span class="sxs-lookup"><span data-stu-id="68426-117">general</span></span>|<span data-ttu-id="68426-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="68426-118">2</span></span>|<span data-ttu-id="68426-119">すべての年齢に適している</span><span class="sxs-lookup"><span data-stu-id="68426-119">Suitable for all ages</span></span>|
|<span data-ttu-id="68426-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="68426-120">parentalGuidance</span></span>|<span data-ttu-id="68426-121">1/3</span><span class="sxs-lookup"><span data-stu-id="68426-121">3</span></span>|<span data-ttu-id="68426-122">PG-12 の分類では、12の下のユーザーについての上位のガイダンスが要求されます。</span><span class="sxs-lookup"><span data-stu-id="68426-122">The PG-12 classification requests parental guidance for young people under 12</span></span>|
|<span data-ttu-id="68426-123">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="68426-123">agesAbove15</span></span>|<span data-ttu-id="68426-124">2/4</span><span class="sxs-lookup"><span data-stu-id="68426-124">4</span></span>|<span data-ttu-id="68426-125">R15 + 分類は、15才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="68426-125">The R15+ classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="68426-126">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="68426-126">agesAbove18</span></span>|<span data-ttu-id="68426-127">5</span><span class="sxs-lookup"><span data-stu-id="68426-127">5</span></span>|<span data-ttu-id="68426-128">R18 + 分類は、18才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="68426-128">The R18+ classification is suitable for viewers of 18 or older</span></span>|




