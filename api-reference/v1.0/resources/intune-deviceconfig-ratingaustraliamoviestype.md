---
title: ratingAustraliaMoviesType 列挙型
description: 映画のオーストラリアのラベルの評価
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0f7df26bc12a92c2571967c68fcd82619a69cb64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911715"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="0d6f4-103">ratingAustraliaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0d6f4-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="0d6f4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d6f4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d6f4-105">映画のオーストラリアのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="0d6f4-105">Movies rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="0d6f4-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0d6f4-106">Members</span></span>
|<span data-ttu-id="0d6f4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0d6f4-107">Member</span></span>|<span data-ttu-id="0d6f4-108">値</span><span class="sxs-lookup"><span data-stu-id="0d6f4-108">Value</span></span>|<span data-ttu-id="0d6f4-109">説明</span><span class="sxs-lookup"><span data-stu-id="0d6f4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d6f4-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="0d6f4-110">allAllowed</span></span>|<span data-ttu-id="0d6f4-111">0</span><span class="sxs-lookup"><span data-stu-id="0d6f4-111">0</span></span>|<span data-ttu-id="0d6f4-112">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="0d6f4-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="0d6f4-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="0d6f4-113">allBlocked</span></span>|<span data-ttu-id="0d6f4-114">1</span><span class="sxs-lookup"><span data-stu-id="0d6f4-114">1</span></span>|<span data-ttu-id="0d6f4-115">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="0d6f4-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="0d6f4-116">全般</span><span class="sxs-lookup"><span data-stu-id="0d6f4-116">general</span></span>|<span data-ttu-id="0d6f4-117">2</span><span class="sxs-lookup"><span data-stu-id="0d6f4-117">2</span></span>|<span data-ttu-id="0d6f4-118">G のクラス分けは、すべてのユーザーに対して適切です</span><span class="sxs-lookup"><span data-stu-id="0d6f4-118">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="0d6f4-119">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="0d6f4-119">parentalGuidance</span></span>|<span data-ttu-id="0d6f4-120">3</span><span class="sxs-lookup"><span data-stu-id="0d6f4-120">3</span></span>|<span data-ttu-id="0d6f4-121">PG が視聴者の親または保護者からのガイドに目をお勧め</span><span class="sxs-lookup"><span data-stu-id="0d6f4-121">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="0d6f4-122">成熟</span><span class="sxs-lookup"><span data-stu-id="0d6f4-122">mature</span></span>|<span data-ttu-id="0d6f4-123">4</span><span class="sxs-lookup"><span data-stu-id="0d6f4-123">4</span></span>|<span data-ttu-id="0d6f4-124">ビューアーで 15 M のクラス分けは推奨されません。</span><span class="sxs-lookup"><span data-stu-id="0d6f4-124">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="0d6f4-125">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="0d6f4-125">agesAbove15</span></span>|<span data-ttu-id="0d6f4-126">5</span><span class="sxs-lookup"><span data-stu-id="0d6f4-126">5</span></span>|<span data-ttu-id="0d6f4-127">MA15 + 分類には適していません 15 未満の閲覧者です。</span><span class="sxs-lookup"><span data-stu-id="0d6f4-127">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="0d6f4-128">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="0d6f4-128">agesAbove18</span></span>|<span data-ttu-id="0d6f4-129">6</span><span class="sxs-lookup"><span data-stu-id="0d6f4-129">6</span></span>|<span data-ttu-id="0d6f4-130">R18 + の分類は 18 才未満の閲覧者には適していません。</span><span class="sxs-lookup"><span data-stu-id="0d6f4-130">The R18+ classification is not suitable for viewers under 18</span></span>|



