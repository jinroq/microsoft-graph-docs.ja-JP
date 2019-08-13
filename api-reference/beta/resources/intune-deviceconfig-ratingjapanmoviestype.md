---
title: ratingJapanMoviesType 列挙型
description: 日本の映画の視聴制限ラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8511194966f2bc0bb2a1de95ff0b554be714c232
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368234"
---
# <a name="ratingjapanmoviestype-enum-type"></a><span data-ttu-id="68262-103">ratingJapanMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="68262-103">ratingJapanMoviesType enum type</span></span>

> <span data-ttu-id="68262-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68262-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68262-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68262-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68262-106">日本の映画の視聴制限ラベル</span><span class="sxs-lookup"><span data-stu-id="68262-106">Movies rating labels in Japan</span></span>

## <a name="members"></a><span data-ttu-id="68262-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="68262-107">Members</span></span>
|<span data-ttu-id="68262-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="68262-108">Member</span></span>|<span data-ttu-id="68262-109">値</span><span class="sxs-lookup"><span data-stu-id="68262-109">Value</span></span>|<span data-ttu-id="68262-110">説明</span><span class="sxs-lookup"><span data-stu-id="68262-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68262-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="68262-111">allAllowed</span></span>|<span data-ttu-id="68262-112">.0</span><span class="sxs-lookup"><span data-stu-id="68262-112">0</span></span>|<span data-ttu-id="68262-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="68262-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="68262-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="68262-114">allBlocked</span></span>|<span data-ttu-id="68262-115">1-d</span><span class="sxs-lookup"><span data-stu-id="68262-115">1</span></span>|<span data-ttu-id="68262-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="68262-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="68262-117">元帳</span><span class="sxs-lookup"><span data-stu-id="68262-117">general</span></span>|<span data-ttu-id="68262-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="68262-118">2</span></span>|<span data-ttu-id="68262-119">すべての年齢に適している</span><span class="sxs-lookup"><span data-stu-id="68262-119">Suitable for all ages</span></span>|
|<span data-ttu-id="68262-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="68262-120">parentalGuidance</span></span>|<span data-ttu-id="68262-121">1/3</span><span class="sxs-lookup"><span data-stu-id="68262-121">3</span></span>|<span data-ttu-id="68262-122">PG-12 の分類では、12の下のユーザーについての上位のガイダンスが要求されます。</span><span class="sxs-lookup"><span data-stu-id="68262-122">The PG-12 classification requests parental guidance for young people under 12</span></span>|
|<span data-ttu-id="68262-123">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="68262-123">agesAbove15</span></span>|<span data-ttu-id="68262-124">2/4</span><span class="sxs-lookup"><span data-stu-id="68262-124">4</span></span>|<span data-ttu-id="68262-125">R15 + 分類は、15才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="68262-125">The R15+ classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="68262-126">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="68262-126">agesAbove18</span></span>|<span data-ttu-id="68262-127">5</span><span class="sxs-lookup"><span data-stu-id="68262-127">5</span></span>|<span data-ttu-id="68262-128">R18 + 分類は、18才以上の閲覧者に適しています。</span><span class="sxs-lookup"><span data-stu-id="68262-128">The R18+ classification is suitable for viewers of 18 or older</span></span>|



