---
title: ratingGermanyMoviesType 列挙型
description: ドイツでの映画の定格ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d5072b95d54b0640115f350d9e8de26e8ec23112
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807820"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="d9ad3-103">ratingGermanyMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d9ad3-103">ratingGermanyMoviesType enum type</span></span>

> <span data-ttu-id="d9ad3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9ad3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9ad3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9ad3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9ad3-106">ドイツでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="d9ad3-106">Movies rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="d9ad3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9ad3-107">Members</span></span>
|<span data-ttu-id="d9ad3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9ad3-108">Member</span></span>|<span data-ttu-id="d9ad3-109">値</span><span class="sxs-lookup"><span data-stu-id="d9ad3-109">Value</span></span>|<span data-ttu-id="d9ad3-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9ad3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ad3-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="d9ad3-111">allAllowed</span></span>|<span data-ttu-id="d9ad3-112">.0</span><span class="sxs-lookup"><span data-stu-id="d9ad3-112">0</span></span>|<span data-ttu-id="d9ad3-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="d9ad3-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="d9ad3-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="d9ad3-114">allBlocked</span></span>|<span data-ttu-id="d9ad3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d9ad3-115">1</span></span>|<span data-ttu-id="d9ad3-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="d9ad3-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="d9ad3-117">元帳</span><span class="sxs-lookup"><span data-stu-id="d9ad3-117">general</span></span>|<span data-ttu-id="d9ad3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d9ad3-118">2</span></span>|<span data-ttu-id="d9ad3-119">Ab 0 Jahren、年齢制限なし</span><span class="sxs-lookup"><span data-stu-id="d9ad3-119">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="d9ad3-120">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="d9ad3-120">agesAbove6</span></span>|<span data-ttu-id="d9ad3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d9ad3-121">3</span></span>|<span data-ttu-id="d9ad3-122">Ab 6 Jahren、才を過ぎた</span><span class="sxs-lookup"><span data-stu-id="d9ad3-122">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="d9ad3-123">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="d9ad3-123">agesAbove12</span></span>|<span data-ttu-id="d9ad3-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d9ad3-124">4</span></span>|<span data-ttu-id="d9ad3-125">Ab 12 Jahren、12才以上</span><span class="sxs-lookup"><span data-stu-id="d9ad3-125">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="d9ad3-126">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="d9ad3-126">agesAbove16</span></span>|<span data-ttu-id="d9ad3-127">5</span><span class="sxs-lookup"><span data-stu-id="d9ad3-127">5</span></span>|<span data-ttu-id="d9ad3-128">Ab 16 Jahren、16才以上</span><span class="sxs-lookup"><span data-stu-id="d9ad3-128">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="d9ad3-129">保護者</span><span class="sxs-lookup"><span data-stu-id="d9ad3-129">adults</span></span>|<span data-ttu-id="d9ad3-130">シックス</span><span class="sxs-lookup"><span data-stu-id="d9ad3-130">6</span></span>|<span data-ttu-id="d9ad3-131">Ab 18 Jahren、大人のみ</span><span class="sxs-lookup"><span data-stu-id="d9ad3-131">Ab 18 Jahren, adults only</span></span>|





