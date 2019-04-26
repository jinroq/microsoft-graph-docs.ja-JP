---
title: ratingUnitedStatesMoviesType 列挙型
description: 米国での映画の定格ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 804110ee07c85a1ca68f259e8b4ae9a206f5f29b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555228"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="49b17-103">ratingUnitedStatesMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="49b17-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="49b17-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49b17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49b17-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49b17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49b17-106">米国での映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="49b17-106">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="49b17-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="49b17-107">Members</span></span>
|<span data-ttu-id="49b17-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="49b17-108">Member</span></span>|<span data-ttu-id="49b17-109">値</span><span class="sxs-lookup"><span data-stu-id="49b17-109">Value</span></span>|<span data-ttu-id="49b17-110">説明</span><span class="sxs-lookup"><span data-stu-id="49b17-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49b17-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="49b17-111">allAllowed</span></span>|<span data-ttu-id="49b17-112">.0</span><span class="sxs-lookup"><span data-stu-id="49b17-112">0</span></span>|<span data-ttu-id="49b17-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="49b17-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="49b17-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="49b17-114">allBlocked</span></span>|<span data-ttu-id="49b17-115">1 </span><span class="sxs-lookup"><span data-stu-id="49b17-115">1</span></span>|<span data-ttu-id="49b17-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="49b17-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="49b17-117">元帳</span><span class="sxs-lookup"><span data-stu-id="49b17-117">general</span></span>|<span data-ttu-id="49b17-118">2 </span><span class="sxs-lookup"><span data-stu-id="49b17-118">2</span></span>|<span data-ttu-id="49b17-119">G、すべての年齢が許可</span><span class="sxs-lookup"><span data-stu-id="49b17-119">G, all ages admitted</span></span>|
|<span data-ttu-id="49b17-120">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="49b17-120">parentalGuidance</span></span>|<span data-ttu-id="49b17-121">3 </span><span class="sxs-lookup"><span data-stu-id="49b17-121">3</span></span>|<span data-ttu-id="49b17-122">PG では、一部の素材が子供に適さない場合があります。</span><span class="sxs-lookup"><span data-stu-id="49b17-122">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="49b17-123">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="49b17-123">parentalGuidance13</span></span>|<span data-ttu-id="49b17-124">4 </span><span class="sxs-lookup"><span data-stu-id="49b17-124">4</span></span>|<span data-ttu-id="49b17-125">PG13 では、いくつかの素材が13の子に対して不適切な場合があります。</span><span class="sxs-lookup"><span data-stu-id="49b17-125">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="49b17-126">しか</span><span class="sxs-lookup"><span data-stu-id="49b17-126">restricted</span></span>|<span data-ttu-id="49b17-127">5 </span><span class="sxs-lookup"><span data-stu-id="49b17-127">5</span></span>|<span data-ttu-id="49b17-128">R、17の下の閲覧者には、親または成人のガーディアンが必要です</span><span class="sxs-lookup"><span data-stu-id="49b17-128">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="49b17-129">保護者</span><span class="sxs-lookup"><span data-stu-id="49b17-129">adults</span></span>|<span data-ttu-id="49b17-130">6 </span><span class="sxs-lookup"><span data-stu-id="49b17-130">6</span></span>|<span data-ttu-id="49b17-131">NC17、大人のみ</span><span class="sxs-lookup"><span data-stu-id="49b17-131">NC17, adults only</span></span>|





