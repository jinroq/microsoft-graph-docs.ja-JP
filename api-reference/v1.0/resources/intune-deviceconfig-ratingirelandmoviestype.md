---
title: ratingIrelandMoviesType 列挙型
description: アイルランドのラベルを規制ムービー
author: tfitzmac
ms.openlocfilehash: bf36790325edfa665f504f161c1de59ebe7c5bbb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349197"
---
# <a name="ratingirelandmoviestype-enum-type"></a><span data-ttu-id="1157c-103">ratingIrelandMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1157c-103">ratingIrelandMoviesType enum type</span></span>

> <span data-ttu-id="1157c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1157c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1157c-105">アイルランドのラベルを規制ムービー</span><span class="sxs-lookup"><span data-stu-id="1157c-105">Movies rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="1157c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1157c-106">Members</span></span>
|<span data-ttu-id="1157c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1157c-107">Member</span></span>|<span data-ttu-id="1157c-108">値</span><span class="sxs-lookup"><span data-stu-id="1157c-108">Value</span></span>|<span data-ttu-id="1157c-109">説明</span><span class="sxs-lookup"><span data-stu-id="1157c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1157c-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="1157c-110">allAllowed</span></span>|<span data-ttu-id="1157c-111">0</span><span class="sxs-lookup"><span data-stu-id="1157c-111">0</span></span>|<span data-ttu-id="1157c-112">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="1157c-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="1157c-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="1157c-113">allBlocked</span></span>|<span data-ttu-id="1157c-114">1</span><span class="sxs-lookup"><span data-stu-id="1157c-114">1</span></span>|<span data-ttu-id="1157c-115">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="1157c-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="1157c-116">全般</span><span class="sxs-lookup"><span data-stu-id="1157c-116">general</span></span>|<span data-ttu-id="1157c-117">2</span><span class="sxs-lookup"><span data-stu-id="1157c-117">2</span></span>|<span data-ttu-id="1157c-118">時代のこと、学校の子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="1157c-118">Suitable for children of school going age</span></span>|
|<span data-ttu-id="1157c-119">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="1157c-119">parentalGuidance</span></span>|<span data-ttu-id="1157c-120">3</span><span class="sxs-lookup"><span data-stu-id="1157c-120">3</span></span>|<span data-ttu-id="1157c-121">PG の分類には、保護者による制限が示されます</span><span class="sxs-lookup"><span data-stu-id="1157c-121">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="1157c-122">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="1157c-122">agesAbove12</span></span>|<span data-ttu-id="1157c-123">4</span><span class="sxs-lookup"><span data-stu-id="1157c-123">4</span></span>|<span data-ttu-id="1157c-124">12 a のクラス分けは、12 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="1157c-124">The 12A classification is suitable for viewers of 12 or older</span></span>|
|<span data-ttu-id="1157c-125">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="1157c-125">agesAbove15</span></span>|<span data-ttu-id="1157c-126">5</span><span class="sxs-lookup"><span data-stu-id="1157c-126">5</span></span>|<span data-ttu-id="1157c-127">15 a のクラス分けは、15 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="1157c-127">The 15A classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="1157c-128">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="1157c-128">agesAbove16</span></span>|<span data-ttu-id="1157c-129">6</span><span class="sxs-lookup"><span data-stu-id="1157c-129">6</span></span>|<span data-ttu-id="1157c-130">16 のクラス分けは、16 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="1157c-130">The 16 classification is suitable for viewers of 16 or older</span></span>|
|<span data-ttu-id="1157c-131">大人</span><span class="sxs-lookup"><span data-stu-id="1157c-131">adults</span></span>|<span data-ttu-id="1157c-132">7</span><span class="sxs-lookup"><span data-stu-id="1157c-132">7</span></span>|<span data-ttu-id="1157c-133">大人にのみ適しての 18 の分類</span><span class="sxs-lookup"><span data-stu-id="1157c-133">The 18 classification, suitable only for adults</span></span>|



