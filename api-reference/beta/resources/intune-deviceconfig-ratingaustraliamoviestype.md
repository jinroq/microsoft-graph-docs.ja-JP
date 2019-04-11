---
title: ratingAustraliaMoviesType 列挙型
description: オーストラリアでの映画の定格ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 438b255970d42bfb0ef63018e87fcbcdfe62b163
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797852"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="81ac2-103">ratingAustraliaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="81ac2-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="81ac2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81ac2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81ac2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81ac2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81ac2-106">オーストラリアでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="81ac2-106">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="81ac2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="81ac2-107">Members</span></span>
|<span data-ttu-id="81ac2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="81ac2-108">Member</span></span>|<span data-ttu-id="81ac2-109">値</span><span class="sxs-lookup"><span data-stu-id="81ac2-109">Value</span></span>|<span data-ttu-id="81ac2-110">説明</span><span class="sxs-lookup"><span data-stu-id="81ac2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ac2-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="81ac2-111">allAllowed</span></span>|<span data-ttu-id="81ac2-112">.0</span><span class="sxs-lookup"><span data-stu-id="81ac2-112">0</span></span>|<span data-ttu-id="81ac2-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="81ac2-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="81ac2-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="81ac2-114">allBlocked</span></span>|<span data-ttu-id="81ac2-115">1-d</span><span class="sxs-lookup"><span data-stu-id="81ac2-115">1</span></span>|<span data-ttu-id="81ac2-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="81ac2-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="81ac2-117">元帳</span><span class="sxs-lookup"><span data-stu-id="81ac2-117">general</span></span>|<span data-ttu-id="81ac2-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="81ac2-118">2</span></span>|<span data-ttu-id="81ac2-119">G 分類は、すべてのユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="81ac2-119">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="81ac2-120">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="81ac2-120">parentalGuidance</span></span>|<span data-ttu-id="81ac2-121">1/3</span><span class="sxs-lookup"><span data-stu-id="81ac2-121">3</span></span>|<span data-ttu-id="81ac2-122">この PG は、親またはガーディアンからのガイダンスを含む15未満のビューアーを推奨します。</span><span class="sxs-lookup"><span data-stu-id="81ac2-122">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="81ac2-123">度</span><span class="sxs-lookup"><span data-stu-id="81ac2-123">mature</span></span>|<span data-ttu-id="81ac2-124">2/4</span><span class="sxs-lookup"><span data-stu-id="81ac2-124">4</span></span>|<span data-ttu-id="81ac2-125">M 分類は15以下の閲覧者には推奨されません</span><span class="sxs-lookup"><span data-stu-id="81ac2-125">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="81ac2-126">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="81ac2-126">agesAbove15</span></span>|<span data-ttu-id="81ac2-127">5</span><span class="sxs-lookup"><span data-stu-id="81ac2-127">5</span></span>|<span data-ttu-id="81ac2-128">MA15 + 分類は15以下の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="81ac2-128">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="81ac2-129">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="81ac2-129">agesAbove18</span></span>|<span data-ttu-id="81ac2-130">シックス</span><span class="sxs-lookup"><span data-stu-id="81ac2-130">6</span></span>|<span data-ttu-id="81ac2-131">R18 + 分類が18の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="81ac2-131">The R18+ classification is not suitable for viewers under 18</span></span>|





