---
title: ratingJapanMoviesType 列挙型
description: 日本の映画の視聴制限ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bc6d1f12d9a7eec2a2f88d483670d34cabe1349
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556922"
---
# <a name="ratingjapanmoviestype-enum-type"></a><span data-ttu-id="af2bf-103">ratingJapanMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="af2bf-103">ratingJapanMoviesType enum type</span></span>

> <span data-ttu-id="af2bf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af2bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af2bf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af2bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af2bf-106">日本の映画の視聴制限ラベル</span><span class="sxs-lookup"><span data-stu-id="af2bf-106">Movies rating labels in Japan</span></span>

## <a name="members"></a><span data-ttu-id="af2bf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="af2bf-107">Members</span></span>
|<span data-ttu-id="af2bf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="af2bf-108">Member</span></span>|<span data-ttu-id="af2bf-109">値</span><span class="sxs-lookup"><span data-stu-id="af2bf-109">Value</span></span>|<span data-ttu-id="af2bf-110">説明</span><span class="sxs-lookup"><span data-stu-id="af2bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2bf-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="af2bf-111">allAllowed</span></span>|<span data-ttu-id="af2bf-112">.0</span><span class="sxs-lookup"><span data-stu-id="af2bf-112">0</span></span>|<span data-ttu-id="af2bf-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="af2bf-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="af2bf-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="af2bf-114">allBlocked</span></span>|<span data-ttu-id="af2bf-115">1 </span><span class="sxs-lookup"><span data-stu-id="af2bf-115">1</span></span>|<span data-ttu-id="af2bf-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="af2bf-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="af2bf-117">元帳</span><span class="sxs-lookup"><span data-stu-id="af2bf-117">general</span></span>|<span data-ttu-id="af2bf-118">2 </span><span class="sxs-lookup"><span data-stu-id="af2bf-118">2</span></span>|<span data-ttu-id="af2bf-119">すべての年齢に適している</span><span class="sxs-lookup"><span data-stu-id="af2bf-119">Suitable for all ages</span></span>|
|<span data-ttu-id="af2bf-120">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="af2bf-120">parentalGuidance</span></span>|<span data-ttu-id="af2bf-121">3 </span><span class="sxs-lookup"><span data-stu-id="af2bf-121">3</span></span>|<span data-ttu-id="af2bf-122">PG-12 の分類では、12の下のユーザーについての上位のガイダンスが要求されます。</span><span class="sxs-lookup"><span data-stu-id="af2bf-122">The PG-12 classification requests parental guidance for young people under 12</span></span>|
|<span data-ttu-id="af2bf-123">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="af2bf-123">agesAbove15</span></span>|<span data-ttu-id="af2bf-124">4 </span><span class="sxs-lookup"><span data-stu-id="af2bf-124">4</span></span>|<span data-ttu-id="af2bf-125">R15 + 分類は、15才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="af2bf-125">The R15+ classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="af2bf-126">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="af2bf-126">agesAbove18</span></span>|<span data-ttu-id="af2bf-127">5 </span><span class="sxs-lookup"><span data-stu-id="af2bf-127">5</span></span>|<span data-ttu-id="af2bf-128">R18 + 分類は、18才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="af2bf-128">The R18+ classification is suitable for viewers of 18 or older</span></span>|





