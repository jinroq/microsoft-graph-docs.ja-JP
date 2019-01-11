---
title: ratingIrelandMoviesType 列挙型
description: アイルランドのラベルを規制ムービー
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f8c88b14f704b0904d2b8e961ebfb99ef1f55cfa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814344"
---
# <a name="ratingirelandmoviestype-enum-type"></a><span data-ttu-id="bef92-103">ratingIrelandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="bef92-103">ratingIrelandMoviesType enum type</span></span>

> <span data-ttu-id="bef92-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bef92-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bef92-105">アイルランドのラベルを規制ムービー</span><span class="sxs-lookup"><span data-stu-id="bef92-105">Movies rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="bef92-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="bef92-106">Members</span></span>
|<span data-ttu-id="bef92-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bef92-107">Member</span></span>|<span data-ttu-id="bef92-108">値</span><span class="sxs-lookup"><span data-stu-id="bef92-108">Value</span></span>|<span data-ttu-id="bef92-109">説明</span><span class="sxs-lookup"><span data-stu-id="bef92-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bef92-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="bef92-110">allAllowed</span></span>|<span data-ttu-id="bef92-111">0</span><span class="sxs-lookup"><span data-stu-id="bef92-111">0</span></span>|<span data-ttu-id="bef92-112">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="bef92-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="bef92-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="bef92-113">allBlocked</span></span>|<span data-ttu-id="bef92-114">1</span><span class="sxs-lookup"><span data-stu-id="bef92-114">1</span></span>|<span data-ttu-id="bef92-115">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="bef92-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="bef92-116">全般</span><span class="sxs-lookup"><span data-stu-id="bef92-116">general</span></span>|<span data-ttu-id="bef92-117">2</span><span class="sxs-lookup"><span data-stu-id="bef92-117">2</span></span>|<span data-ttu-id="bef92-118">時代のこと、学校の子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="bef92-118">Suitable for children of school going age</span></span>|
|<span data-ttu-id="bef92-119">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="bef92-119">parentalGuidance</span></span>|<span data-ttu-id="bef92-120">3</span><span class="sxs-lookup"><span data-stu-id="bef92-120">3</span></span>|<span data-ttu-id="bef92-121">PG の分類には、保護者による制限が示されます</span><span class="sxs-lookup"><span data-stu-id="bef92-121">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="bef92-122">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="bef92-122">agesAbove12</span></span>|<span data-ttu-id="bef92-123">4</span><span class="sxs-lookup"><span data-stu-id="bef92-123">4</span></span>|<span data-ttu-id="bef92-124">12 a のクラス分けは、12 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="bef92-124">The 12A classification is suitable for viewers of 12 or older</span></span>|
|<span data-ttu-id="bef92-125">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="bef92-125">agesAbove15</span></span>|<span data-ttu-id="bef92-126">5</span><span class="sxs-lookup"><span data-stu-id="bef92-126">5</span></span>|<span data-ttu-id="bef92-127">15 a のクラス分けは、15 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="bef92-127">The 15A classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="bef92-128">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="bef92-128">agesAbove16</span></span>|<span data-ttu-id="bef92-129">6</span><span class="sxs-lookup"><span data-stu-id="bef92-129">6</span></span>|<span data-ttu-id="bef92-130">16 のクラス分けは、16 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="bef92-130">The 16 classification is suitable for viewers of 16 or older</span></span>|
|<span data-ttu-id="bef92-131">大人</span><span class="sxs-lookup"><span data-stu-id="bef92-131">adults</span></span>|<span data-ttu-id="bef92-132">7</span><span class="sxs-lookup"><span data-stu-id="bef92-132">7</span></span>|<span data-ttu-id="bef92-133">大人にのみ適しての 18 の分類</span><span class="sxs-lookup"><span data-stu-id="bef92-133">The 18 classification, suitable only for adults</span></span>|



