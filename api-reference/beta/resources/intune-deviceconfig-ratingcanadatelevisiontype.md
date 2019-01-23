---
title: ratingCanadaTelevisionType 列挙型
description: カナダのテレビのコンテンツの規制ラベル
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 174a6d893220f21bafaafdc03880801947c2cd25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415643"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="8142d-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8142d-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="8142d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8142d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8142d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8142d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8142d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8142d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8142d-107">カナダのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="8142d-107">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="8142d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8142d-108">Members</span></span>
|<span data-ttu-id="8142d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8142d-109">Member</span></span>|<span data-ttu-id="8142d-110">値</span><span class="sxs-lookup"><span data-stu-id="8142d-110">Value</span></span>|<span data-ttu-id="8142d-111">説明</span><span class="sxs-lookup"><span data-stu-id="8142d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8142d-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="8142d-112">allAllowed</span></span>|<span data-ttu-id="8142d-113">0</span><span class="sxs-lookup"><span data-stu-id="8142d-113">0</span></span>|<span data-ttu-id="8142d-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="8142d-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="8142d-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="8142d-115">allBlocked</span></span>|<span data-ttu-id="8142d-116">1</span><span class="sxs-lookup"><span data-stu-id="8142d-116">1</span></span>|<span data-ttu-id="8142d-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="8142d-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="8142d-118">children</span><span class="sxs-lookup"><span data-stu-id="8142d-118">children</span></span>|<span data-ttu-id="8142d-119">2</span><span class="sxs-lookup"><span data-stu-id="8142d-119">2</span></span>|<span data-ttu-id="8142d-120">C のクラス分けが 2 ~ 7 年間の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="8142d-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="8142d-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="8142d-121">childrenAbove8</span></span>|<span data-ttu-id="8142d-122">3</span><span class="sxs-lookup"><span data-stu-id="8142d-122">3</span></span>|<span data-ttu-id="8142d-123">C8 のクラス分けは、子供に適して古く 8 +</span><span class="sxs-lookup"><span data-stu-id="8142d-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="8142d-124">全般</span><span class="sxs-lookup"><span data-stu-id="8142d-124">general</span></span>|<span data-ttu-id="8142d-125">4</span><span class="sxs-lookup"><span data-stu-id="8142d-125">4</span></span>|<span data-ttu-id="8142d-126">G 分類が一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="8142d-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="8142d-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="8142d-127">parentalGuidance</span></span>|<span data-ttu-id="8142d-128">5</span><span class="sxs-lookup"><span data-stu-id="8142d-128">5</span></span>|<span data-ttu-id="8142d-129">PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="8142d-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="8142d-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="8142d-130">agesAbove14</span></span>|<span data-ttu-id="8142d-131">6</span><span class="sxs-lookup"><span data-stu-id="8142d-131">6</span></span>|<span data-ttu-id="8142d-132">14 と古い視聴者の年齢 14 + のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="8142d-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="8142d-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="8142d-133">agesAbove18</span></span>|<span data-ttu-id="8142d-134">7</span><span class="sxs-lookup"><span data-stu-id="8142d-134">7</span></span>|<span data-ttu-id="8142d-135">18 + のクラス分けは、視聴者の年齢 18</span><span class="sxs-lookup"><span data-stu-id="8142d-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|




