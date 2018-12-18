---
title: ratingCanadaMoviesType 列挙型
description: 映画がカナダでのラベルの評価
author: tfitzmac
ms.openlocfilehash: fdedbd1b52c8ac8527119fb4957a26becd5c0a1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336933"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="b2dc8-103">ratingCanadaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b2dc8-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="b2dc8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2dc8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2dc8-105">映画がカナダでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="b2dc8-105">Movies rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="b2dc8-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="b2dc8-106">Members</span></span>
|<span data-ttu-id="b2dc8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b2dc8-107">Member</span></span>|<span data-ttu-id="b2dc8-108">値</span><span class="sxs-lookup"><span data-stu-id="b2dc8-108">Value</span></span>|<span data-ttu-id="b2dc8-109">説明</span><span class="sxs-lookup"><span data-stu-id="b2dc8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2dc8-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="b2dc8-110">allAllowed</span></span>|<span data-ttu-id="b2dc8-111">0</span><span class="sxs-lookup"><span data-stu-id="b2dc8-111">0</span></span>|<span data-ttu-id="b2dc8-112">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="b2dc8-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="b2dc8-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="b2dc8-113">allBlocked</span></span>|<span data-ttu-id="b2dc8-114">1</span><span class="sxs-lookup"><span data-stu-id="b2dc8-114">1</span></span>|<span data-ttu-id="b2dc8-115">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="b2dc8-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="b2dc8-116">全般</span><span class="sxs-lookup"><span data-stu-id="b2dc8-116">general</span></span>|<span data-ttu-id="b2dc8-117">2</span><span class="sxs-lookup"><span data-stu-id="b2dc8-117">2</span></span>|<span data-ttu-id="b2dc8-118">G のクラス分けがすべての年代に適しています。</span><span class="sxs-lookup"><span data-stu-id="b2dc8-118">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="b2dc8-119">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="b2dc8-119">parentalGuidance</span></span>|<span data-ttu-id="b2dc8-120">3</span><span class="sxs-lookup"><span data-stu-id="b2dc8-120">3</span></span>|<span data-ttu-id="b2dc8-121">PG の分類には、保護者による制限が示されます</span><span class="sxs-lookup"><span data-stu-id="b2dc8-121">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="b2dc8-122">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="b2dc8-122">agesAbove14</span></span>|<span data-ttu-id="b2dc8-123">4</span><span class="sxs-lookup"><span data-stu-id="b2dc8-123">4</span></span>|<span data-ttu-id="b2dc8-124">14A 分類が 14 またはそれ以前の上のあるユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="b2dc8-124">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="b2dc8-125">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="b2dc8-125">agesAbove18</span></span>|<span data-ttu-id="b2dc8-126">5</span><span class="sxs-lookup"><span data-stu-id="b2dc8-126">5</span></span>|<span data-ttu-id="b2dc8-127">18A 分類が 18 またはそれ以前の上のあるユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="b2dc8-127">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="b2dc8-128">制限</span><span class="sxs-lookup"><span data-stu-id="b2dc8-128">restricted</span></span>|<span data-ttu-id="b2dc8-129">6</span><span class="sxs-lookup"><span data-stu-id="b2dc8-129">6</span></span>|<span data-ttu-id="b2dc8-130">R のクラス分けは、18 年間に限定され、古い</span><span class="sxs-lookup"><span data-stu-id="b2dc8-130">The R classification is restricted to 18 years and older</span></span>|



