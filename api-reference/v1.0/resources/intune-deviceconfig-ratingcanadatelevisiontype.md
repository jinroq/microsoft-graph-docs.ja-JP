---
title: ratingCanadaTelevisionType 列挙型
description: カナダのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9003cb0743b534f0a36787b35043ec8b639ca0f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873137"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="15440-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="15440-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="15440-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15440-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15440-105">カナダのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="15440-105">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="15440-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="15440-106">Members</span></span>
|<span data-ttu-id="15440-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="15440-107">Member</span></span>|<span data-ttu-id="15440-108">値</span><span class="sxs-lookup"><span data-stu-id="15440-108">Value</span></span>|<span data-ttu-id="15440-109">説明</span><span class="sxs-lookup"><span data-stu-id="15440-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15440-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="15440-110">allAllowed</span></span>|<span data-ttu-id="15440-111">0</span><span class="sxs-lookup"><span data-stu-id="15440-111">0</span></span>|<span data-ttu-id="15440-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="15440-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="15440-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="15440-113">allBlocked</span></span>|<span data-ttu-id="15440-114">1</span><span class="sxs-lookup"><span data-stu-id="15440-114">1</span></span>|<span data-ttu-id="15440-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="15440-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="15440-116">children</span><span class="sxs-lookup"><span data-stu-id="15440-116">children</span></span>|<span data-ttu-id="15440-117">2</span><span class="sxs-lookup"><span data-stu-id="15440-117">2</span></span>|<span data-ttu-id="15440-118">C のクラス分けが 2 ~ 7 年間の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="15440-118">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="15440-119">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="15440-119">childrenAbove8</span></span>|<span data-ttu-id="15440-120">3</span><span class="sxs-lookup"><span data-stu-id="15440-120">3</span></span>|<span data-ttu-id="15440-121">C8 のクラス分けは、子供に適して古く 8 +</span><span class="sxs-lookup"><span data-stu-id="15440-121">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="15440-122">全般</span><span class="sxs-lookup"><span data-stu-id="15440-122">general</span></span>|<span data-ttu-id="15440-123">4</span><span class="sxs-lookup"><span data-stu-id="15440-123">4</span></span>|<span data-ttu-id="15440-124">G 分類が一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="15440-124">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="15440-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="15440-125">parentalGuidance</span></span>|<span data-ttu-id="15440-126">5</span><span class="sxs-lookup"><span data-stu-id="15440-126">5</span></span>|<span data-ttu-id="15440-127">PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="15440-127">PG, Parental Guidance</span></span>|
|<span data-ttu-id="15440-128">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="15440-128">agesAbove14</span></span>|<span data-ttu-id="15440-129">6</span><span class="sxs-lookup"><span data-stu-id="15440-129">6</span></span>|<span data-ttu-id="15440-130">14 と古い視聴者の年齢 14 + のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="15440-130">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="15440-131">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="15440-131">agesAbove18</span></span>|<span data-ttu-id="15440-132">7</span><span class="sxs-lookup"><span data-stu-id="15440-132">7</span></span>|<span data-ttu-id="15440-133">18 + のクラス分けは、視聴者の年齢 18</span><span class="sxs-lookup"><span data-stu-id="15440-133">The 18+ classification is intended for viewers ages 18 and older</span></span>|



