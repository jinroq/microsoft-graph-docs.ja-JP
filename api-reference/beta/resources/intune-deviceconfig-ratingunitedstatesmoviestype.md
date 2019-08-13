---
title: ratingUnitedStatesMoviesType 列挙型
description: 米国での映画の定格ラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1cc9a4a929b7b563322e8e2a50855592006ca323
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368150"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="7fdbf-103">ratingUnitedStatesMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7fdbf-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="7fdbf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fdbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fdbf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7fdbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fdbf-106">米国での映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="7fdbf-106">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="7fdbf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7fdbf-107">Members</span></span>
|<span data-ttu-id="7fdbf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7fdbf-108">Member</span></span>|<span data-ttu-id="7fdbf-109">値</span><span class="sxs-lookup"><span data-stu-id="7fdbf-109">Value</span></span>|<span data-ttu-id="7fdbf-110">説明</span><span class="sxs-lookup"><span data-stu-id="7fdbf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fdbf-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="7fdbf-111">allAllowed</span></span>|<span data-ttu-id="7fdbf-112">.0</span><span class="sxs-lookup"><span data-stu-id="7fdbf-112">0</span></span>|<span data-ttu-id="7fdbf-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="7fdbf-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="7fdbf-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="7fdbf-114">allBlocked</span></span>|<span data-ttu-id="7fdbf-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7fdbf-115">1</span></span>|<span data-ttu-id="7fdbf-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="7fdbf-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="7fdbf-117">元帳</span><span class="sxs-lookup"><span data-stu-id="7fdbf-117">general</span></span>|<span data-ttu-id="7fdbf-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7fdbf-118">2</span></span>|<span data-ttu-id="7fdbf-119">G、すべての年齢が許可</span><span class="sxs-lookup"><span data-stu-id="7fdbf-119">G, all ages admitted</span></span>|
|<span data-ttu-id="7fdbf-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="7fdbf-120">parentalGuidance</span></span>|<span data-ttu-id="7fdbf-121">1/3</span><span class="sxs-lookup"><span data-stu-id="7fdbf-121">3</span></span>|<span data-ttu-id="7fdbf-122">PG では、一部の素材が子供に適さない場合があります。</span><span class="sxs-lookup"><span data-stu-id="7fdbf-122">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="7fdbf-123">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="7fdbf-123">parentalGuidance13</span></span>|<span data-ttu-id="7fdbf-124">2/4</span><span class="sxs-lookup"><span data-stu-id="7fdbf-124">4</span></span>|<span data-ttu-id="7fdbf-125">PG13 では、いくつかの素材が13の子に対して不適切な場合があります。</span><span class="sxs-lookup"><span data-stu-id="7fdbf-125">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="7fdbf-126">しか</span><span class="sxs-lookup"><span data-stu-id="7fdbf-126">restricted</span></span>|<span data-ttu-id="7fdbf-127">5</span><span class="sxs-lookup"><span data-stu-id="7fdbf-127">5</span></span>|<span data-ttu-id="7fdbf-128">R、17の下の閲覧者には、親または成人のガーディアンが必要です</span><span class="sxs-lookup"><span data-stu-id="7fdbf-128">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="7fdbf-129">保護者</span><span class="sxs-lookup"><span data-stu-id="7fdbf-129">adults</span></span>|<span data-ttu-id="7fdbf-130">シックス</span><span class="sxs-lookup"><span data-stu-id="7fdbf-130">6</span></span>|<span data-ttu-id="7fdbf-131">NC17、大人のみ</span><span class="sxs-lookup"><span data-stu-id="7fdbf-131">NC17, adults only</span></span>|



