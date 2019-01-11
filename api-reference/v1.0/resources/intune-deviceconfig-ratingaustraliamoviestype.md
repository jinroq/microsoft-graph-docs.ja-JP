---
title: ratingAustraliaMoviesType 列挙型
description: 映画のオーストラリアのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fe95e91077514022360d273dead76e694af3169b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829541"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="e1a96-103">ratingAustraliaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e1a96-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="e1a96-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1a96-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1a96-105">映画のオーストラリアのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="e1a96-105">Movies rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="e1a96-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1a96-106">Members</span></span>
|<span data-ttu-id="e1a96-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1a96-107">Member</span></span>|<span data-ttu-id="e1a96-108">値</span><span class="sxs-lookup"><span data-stu-id="e1a96-108">Value</span></span>|<span data-ttu-id="e1a96-109">説明</span><span class="sxs-lookup"><span data-stu-id="e1a96-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a96-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="e1a96-110">allAllowed</span></span>|<span data-ttu-id="e1a96-111">0</span><span class="sxs-lookup"><span data-stu-id="e1a96-111">0</span></span>|<span data-ttu-id="e1a96-112">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="e1a96-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="e1a96-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="e1a96-113">allBlocked</span></span>|<span data-ttu-id="e1a96-114">1</span><span class="sxs-lookup"><span data-stu-id="e1a96-114">1</span></span>|<span data-ttu-id="e1a96-115">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="e1a96-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="e1a96-116">全般</span><span class="sxs-lookup"><span data-stu-id="e1a96-116">general</span></span>|<span data-ttu-id="e1a96-117">2</span><span class="sxs-lookup"><span data-stu-id="e1a96-117">2</span></span>|<span data-ttu-id="e1a96-118">G のクラス分けは、すべてのユーザーに対して適切です</span><span class="sxs-lookup"><span data-stu-id="e1a96-118">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="e1a96-119">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="e1a96-119">parentalGuidance</span></span>|<span data-ttu-id="e1a96-120">3</span><span class="sxs-lookup"><span data-stu-id="e1a96-120">3</span></span>|<span data-ttu-id="e1a96-121">PG が視聴者の親または保護者からのガイドに目をお勧め</span><span class="sxs-lookup"><span data-stu-id="e1a96-121">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="e1a96-122">成熟</span><span class="sxs-lookup"><span data-stu-id="e1a96-122">mature</span></span>|<span data-ttu-id="e1a96-123">4</span><span class="sxs-lookup"><span data-stu-id="e1a96-123">4</span></span>|<span data-ttu-id="e1a96-124">ビューアーで 15 M のクラス分けは推奨されません。</span><span class="sxs-lookup"><span data-stu-id="e1a96-124">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="e1a96-125">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="e1a96-125">agesAbove15</span></span>|<span data-ttu-id="e1a96-126">5</span><span class="sxs-lookup"><span data-stu-id="e1a96-126">5</span></span>|<span data-ttu-id="e1a96-127">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="e1a96-127">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="e1a96-128">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="e1a96-128">agesAbove18</span></span>|<span data-ttu-id="e1a96-129">6</span><span class="sxs-lookup"><span data-stu-id="e1a96-129">6</span></span>|<span data-ttu-id="e1a96-130">R18 + の分類は 18 才未満の閲覧者には適していません。</span><span class="sxs-lookup"><span data-stu-id="e1a96-130">The R18+ classification is not suitable for viewers under 18</span></span>|



