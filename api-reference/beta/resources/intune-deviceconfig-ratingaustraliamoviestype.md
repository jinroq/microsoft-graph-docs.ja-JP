---
title: ratingAustraliaMoviesType 列挙型
description: 映画のオーストラリアのラベルの評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ee94e37275d0a97729ea3de12264067ecf1e2d3d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408412"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="9329a-103">ratingAustraliaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9329a-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="9329a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9329a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9329a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9329a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9329a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9329a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9329a-107">映画のオーストラリアのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="9329a-107">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="9329a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9329a-108">Members</span></span>
|<span data-ttu-id="9329a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9329a-109">Member</span></span>|<span data-ttu-id="9329a-110">値</span><span class="sxs-lookup"><span data-stu-id="9329a-110">Value</span></span>|<span data-ttu-id="9329a-111">説明</span><span class="sxs-lookup"><span data-stu-id="9329a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9329a-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="9329a-112">allAllowed</span></span>|<span data-ttu-id="9329a-113">0</span><span class="sxs-lookup"><span data-stu-id="9329a-113">0</span></span>|<span data-ttu-id="9329a-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="9329a-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="9329a-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="9329a-115">allBlocked</span></span>|<span data-ttu-id="9329a-116">1</span><span class="sxs-lookup"><span data-stu-id="9329a-116">1</span></span>|<span data-ttu-id="9329a-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="9329a-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="9329a-118">全般</span><span class="sxs-lookup"><span data-stu-id="9329a-118">general</span></span>|<span data-ttu-id="9329a-119">2</span><span class="sxs-lookup"><span data-stu-id="9329a-119">2</span></span>|<span data-ttu-id="9329a-120">G のクラス分けは、すべてのユーザーに対して適切です</span><span class="sxs-lookup"><span data-stu-id="9329a-120">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="9329a-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="9329a-121">parentalGuidance</span></span>|<span data-ttu-id="9329a-122">3</span><span class="sxs-lookup"><span data-stu-id="9329a-122">3</span></span>|<span data-ttu-id="9329a-123">PG が視聴者の親または保護者からのガイドに目をお勧め</span><span class="sxs-lookup"><span data-stu-id="9329a-123">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="9329a-124">成熟</span><span class="sxs-lookup"><span data-stu-id="9329a-124">mature</span></span>|<span data-ttu-id="9329a-125">4</span><span class="sxs-lookup"><span data-stu-id="9329a-125">4</span></span>|<span data-ttu-id="9329a-126">ビューアーで 15 M のクラス分けは推奨されません。</span><span class="sxs-lookup"><span data-stu-id="9329a-126">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="9329a-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="9329a-127">agesAbove15</span></span>|<span data-ttu-id="9329a-128">5</span><span class="sxs-lookup"><span data-stu-id="9329a-128">5</span></span>|<span data-ttu-id="9329a-129">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="9329a-129">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="9329a-130">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="9329a-130">agesAbove18</span></span>|<span data-ttu-id="9329a-131">6</span><span class="sxs-lookup"><span data-stu-id="9329a-131">6</span></span>|<span data-ttu-id="9329a-132">R18 + の分類は 18 才未満の閲覧者には適していません。</span><span class="sxs-lookup"><span data-stu-id="9329a-132">The R18+ classification is not suitable for viewers under 18</span></span>|




