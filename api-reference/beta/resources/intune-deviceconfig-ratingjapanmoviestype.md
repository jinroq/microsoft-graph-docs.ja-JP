---
title: ratingJapanMoviesType 列挙型
description: 映画の日本でのラベルの評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bc8b5a6ba4790f749fb2da5c1e8c6ec1c000b962
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422041"
---
# <a name="ratingjapanmoviestype-enum-type"></a><span data-ttu-id="59c29-103">ratingJapanMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="59c29-103">ratingJapanMoviesType enum type</span></span>

> <span data-ttu-id="59c29-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59c29-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="59c29-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59c29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59c29-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="59c29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59c29-107">映画の日本でのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="59c29-107">Movies rating labels in Japan</span></span>

## <a name="members"></a><span data-ttu-id="59c29-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="59c29-108">Members</span></span>
|<span data-ttu-id="59c29-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="59c29-109">Member</span></span>|<span data-ttu-id="59c29-110">値</span><span class="sxs-lookup"><span data-stu-id="59c29-110">Value</span></span>|<span data-ttu-id="59c29-111">説明</span><span class="sxs-lookup"><span data-stu-id="59c29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59c29-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="59c29-112">allAllowed</span></span>|<span data-ttu-id="59c29-113">0</span><span class="sxs-lookup"><span data-stu-id="59c29-113">0</span></span>|<span data-ttu-id="59c29-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="59c29-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="59c29-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="59c29-115">allBlocked</span></span>|<span data-ttu-id="59c29-116">1</span><span class="sxs-lookup"><span data-stu-id="59c29-116">1</span></span>|<span data-ttu-id="59c29-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="59c29-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="59c29-118">全般</span><span class="sxs-lookup"><span data-stu-id="59c29-118">general</span></span>|<span data-ttu-id="59c29-119">2</span><span class="sxs-lookup"><span data-stu-id="59c29-119">2</span></span>|<span data-ttu-id="59c29-120">一般ユーザー向け</span><span class="sxs-lookup"><span data-stu-id="59c29-120">Suitable for all ages</span></span>|
|<span data-ttu-id="59c29-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="59c29-121">parentalGuidance</span></span>|<span data-ttu-id="59c29-122">3</span><span class="sxs-lookup"><span data-stu-id="59c29-122">3</span></span>|<span data-ttu-id="59c29-123">PG 12 分類若い人で 12 の保護者による制限を要求します。</span><span class="sxs-lookup"><span data-stu-id="59c29-123">The PG-12 classification requests parental guidance for young people under 12</span></span>|
|<span data-ttu-id="59c29-124">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="59c29-124">agesAbove15</span></span>|<span data-ttu-id="59c29-125">4</span><span class="sxs-lookup"><span data-stu-id="59c29-125">4</span></span>|<span data-ttu-id="59c29-126">R15 の各 + のクラス分けは、15 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="59c29-126">The R15+ classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="59c29-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="59c29-127">agesAbove18</span></span>|<span data-ttu-id="59c29-128">5</span><span class="sxs-lookup"><span data-stu-id="59c29-128">5</span></span>|<span data-ttu-id="59c29-129">R18 + の分類は、18 の閲覧者に対して適切なまたは古い</span><span class="sxs-lookup"><span data-stu-id="59c29-129">The R18+ classification is suitable for viewers of 18 or older</span></span>|




