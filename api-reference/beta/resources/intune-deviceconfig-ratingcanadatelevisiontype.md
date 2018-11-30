---
title: ratingCanadaTelevisionType 列挙型
description: カナダのテレビのコンテンツの規制ラベル
ms.openlocfilehash: ca5e35f05d76a7135ef73949cdb804b088d61ebe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072685"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="b9df2-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b9df2-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="b9df2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b9df2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9df2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9df2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9df2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9df2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9df2-107">カナダのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="b9df2-107">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="b9df2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b9df2-108">Members</span></span>
|<span data-ttu-id="b9df2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b9df2-109">Member</span></span>|<span data-ttu-id="b9df2-110">値</span><span class="sxs-lookup"><span data-stu-id="b9df2-110">Value</span></span>|<span data-ttu-id="b9df2-111">説明</span><span class="sxs-lookup"><span data-stu-id="b9df2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9df2-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="b9df2-112">allAllowed</span></span>|<span data-ttu-id="b9df2-113">0</span><span class="sxs-lookup"><span data-stu-id="b9df2-113">0</span></span>|<span data-ttu-id="b9df2-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="b9df2-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="b9df2-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="b9df2-115">allBlocked</span></span>|<span data-ttu-id="b9df2-116">1</span><span class="sxs-lookup"><span data-stu-id="b9df2-116">1</span></span>|<span data-ttu-id="b9df2-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="b9df2-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="b9df2-118">children</span><span class="sxs-lookup"><span data-stu-id="b9df2-118">children</span></span>|<span data-ttu-id="b9df2-119">2</span><span class="sxs-lookup"><span data-stu-id="b9df2-119">2</span></span>|<span data-ttu-id="b9df2-120">C のクラス分けが 2 ~ 7 年間の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="b9df2-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="b9df2-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="b9df2-121">childrenAbove8</span></span>|<span data-ttu-id="b9df2-122">3</span><span class="sxs-lookup"><span data-stu-id="b9df2-122">3</span></span>|<span data-ttu-id="b9df2-123">C8 のクラス分けは、子供に適して古く 8 +</span><span class="sxs-lookup"><span data-stu-id="b9df2-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="b9df2-124">全般</span><span class="sxs-lookup"><span data-stu-id="b9df2-124">general</span></span>|<span data-ttu-id="b9df2-125">4</span><span class="sxs-lookup"><span data-stu-id="b9df2-125">4</span></span>|<span data-ttu-id="b9df2-126">G 分類が一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="b9df2-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="b9df2-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="b9df2-127">parentalGuidance</span></span>|<span data-ttu-id="b9df2-128">5</span><span class="sxs-lookup"><span data-stu-id="b9df2-128">5</span></span>|<span data-ttu-id="b9df2-129">PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="b9df2-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="b9df2-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="b9df2-130">agesAbove14</span></span>|<span data-ttu-id="b9df2-131">6</span><span class="sxs-lookup"><span data-stu-id="b9df2-131">6</span></span>|<span data-ttu-id="b9df2-132">14 と古い視聴者の年齢 14 + のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="b9df2-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="b9df2-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="b9df2-133">agesAbove18</span></span>|<span data-ttu-id="b9df2-134">7</span><span class="sxs-lookup"><span data-stu-id="b9df2-134">7</span></span>|<span data-ttu-id="b9df2-135">18 + のクラス分けは、視聴者の年齢 18</span><span class="sxs-lookup"><span data-stu-id="b9df2-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|





