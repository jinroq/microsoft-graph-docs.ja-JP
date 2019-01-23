---
title: ratingUnitedStatesTelevisionType 列挙型
description: アメリカ合衆国内のテレビ コンテンツの規制ラベル
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 405aad7e63d1c323503dde0b0bd8829702a7dcaf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403358"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="4d130-103">ratingUnitedStatesTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4d130-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="4d130-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4d130-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4d130-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d130-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d130-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d130-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d130-107">アメリカ合衆国内のテレビ コンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="4d130-107">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="4d130-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4d130-108">Members</span></span>
|<span data-ttu-id="4d130-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4d130-109">Member</span></span>|<span data-ttu-id="4d130-110">値</span><span class="sxs-lookup"><span data-stu-id="4d130-110">Value</span></span>|<span data-ttu-id="4d130-111">説明</span><span class="sxs-lookup"><span data-stu-id="4d130-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d130-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="4d130-112">allAllowed</span></span>|<span data-ttu-id="4d130-113">0</span><span class="sxs-lookup"><span data-stu-id="4d130-113">0</span></span>|<span data-ttu-id="4d130-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="4d130-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="4d130-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="4d130-115">allBlocked</span></span>|<span data-ttu-id="4d130-116">1</span><span class="sxs-lookup"><span data-stu-id="4d130-116">1</span></span>|<span data-ttu-id="4d130-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="4d130-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="4d130-118">childrenAll</span><span class="sxs-lookup"><span data-stu-id="4d130-118">childrenAll</span></span>|<span data-ttu-id="4d130-119">2</span><span class="sxs-lookup"><span data-stu-id="4d130-119">2</span></span>|<span data-ttu-id="4d130-120">テレビ Y のすべての子</span><span class="sxs-lookup"><span data-stu-id="4d130-120">TV-Y, all children</span></span>|
|<span data-ttu-id="4d130-121">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="4d130-121">childrenAbove7</span></span>|<span data-ttu-id="4d130-122">3</span><span class="sxs-lookup"><span data-stu-id="4d130-122">3</span></span>|<span data-ttu-id="4d130-123">テレビ ・ Y7、子供の年齢 7 およびそれ以上</span><span class="sxs-lookup"><span data-stu-id="4d130-123">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="4d130-124">全般</span><span class="sxs-lookup"><span data-stu-id="4d130-124">general</span></span>|<span data-ttu-id="4d130-125">4</span><span class="sxs-lookup"><span data-stu-id="4d130-125">4</span></span>|<span data-ttu-id="4d130-126">テレビ G、一般ユーザー向け</span><span class="sxs-lookup"><span data-stu-id="4d130-126">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="4d130-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="4d130-127">parentalGuidance</span></span>|<span data-ttu-id="4d130-128">5</span><span class="sxs-lookup"><span data-stu-id="4d130-128">5</span></span>|<span data-ttu-id="4d130-129">テレビ PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="4d130-129">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="4d130-130">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="4d130-130">childrenAbove14</span></span>|<span data-ttu-id="4d130-131">6</span><span class="sxs-lookup"><span data-stu-id="4d130-131">6</span></span>|<span data-ttu-id="4d130-132">テレビ-14、子供時代の 14 以上の文字</span><span class="sxs-lookup"><span data-stu-id="4d130-132">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="4d130-133">大人</span><span class="sxs-lookup"><span data-stu-id="4d130-133">adults</span></span>|<span data-ttu-id="4d130-134">7</span><span class="sxs-lookup"><span data-stu-id="4d130-134">7</span></span>|<span data-ttu-id="4d130-135">テレビ MA、成人のみ</span><span class="sxs-lookup"><span data-stu-id="4d130-135">TV-MA, adults only</span></span>|




