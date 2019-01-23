---
title: ratingIrelandTelevisionType 列挙型
description: アイルランドのテレビのコンテンツの規制ラベル
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8177ea18d5a8f840daf8f13c0493288fad342285
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394636"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="86c07-103">ratingIrelandTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="86c07-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="86c07-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86c07-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86c07-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86c07-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86c07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86c07-107">アイルランドのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="86c07-107">TV content rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="86c07-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="86c07-108">Members</span></span>
|<span data-ttu-id="86c07-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="86c07-109">Member</span></span>|<span data-ttu-id="86c07-110">値</span><span class="sxs-lookup"><span data-stu-id="86c07-110">Value</span></span>|<span data-ttu-id="86c07-111">説明</span><span class="sxs-lookup"><span data-stu-id="86c07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86c07-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="86c07-112">allAllowed</span></span>|<span data-ttu-id="86c07-113">0</span><span class="sxs-lookup"><span data-stu-id="86c07-113">0</span></span>|<span data-ttu-id="86c07-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="86c07-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="86c07-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="86c07-115">allBlocked</span></span>|<span data-ttu-id="86c07-116">1</span><span class="sxs-lookup"><span data-stu-id="86c07-116">1</span></span>|<span data-ttu-id="86c07-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="86c07-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="86c07-118">全般</span><span class="sxs-lookup"><span data-stu-id="86c07-118">general</span></span>|<span data-ttu-id="86c07-119">2</span><span class="sxs-lookup"><span data-stu-id="86c07-119">2</span></span>|<span data-ttu-id="86c07-120">GA クラス分けがすべての対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="86c07-120">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="86c07-121">children</span><span class="sxs-lookup"><span data-stu-id="86c07-121">children</span></span>|<span data-ttu-id="86c07-122">3</span><span class="sxs-lookup"><span data-stu-id="86c07-122">3</span></span>|<span data-ttu-id="86c07-123">CH クラス分けが子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="86c07-123">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="86c07-124">youngAdults</span><span class="sxs-lookup"><span data-stu-id="86c07-124">youngAdults</span></span>|<span data-ttu-id="86c07-125">4</span><span class="sxs-lookup"><span data-stu-id="86c07-125">4</span></span>|<span data-ttu-id="86c07-126">YA クラス分けが 10 代向けに適しています。</span><span class="sxs-lookup"><span data-stu-id="86c07-126">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="86c07-127">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="86c07-127">parentalSupervision</span></span>|<span data-ttu-id="86c07-128">5</span><span class="sxs-lookup"><span data-stu-id="86c07-128">5</span></span>|<span data-ttu-id="86c07-129">PS 分類制限子供のアクセスを考慮するには、親と保護者へを招待します。</span><span class="sxs-lookup"><span data-stu-id="86c07-129">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="86c07-130">成熟</span><span class="sxs-lookup"><span data-stu-id="86c07-130">mature</span></span>|<span data-ttu-id="86c07-131">6</span><span class="sxs-lookup"><span data-stu-id="86c07-131">6</span></span>|<span data-ttu-id="86c07-132">MA クラス分けが大人に適しています。</span><span class="sxs-lookup"><span data-stu-id="86c07-132">The MA classification is suitable for adults</span></span>|




