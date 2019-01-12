---
title: ratingCanadaTelevisionType 列挙型
description: カナダのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e62339ddac6e6666e17ee5e83aee1f53f4a45fe3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949221"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="c3475-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c3475-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="c3475-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3475-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3475-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3475-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3475-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3475-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3475-107">カナダのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="c3475-107">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="c3475-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c3475-108">Members</span></span>
|<span data-ttu-id="c3475-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c3475-109">Member</span></span>|<span data-ttu-id="c3475-110">値</span><span class="sxs-lookup"><span data-stu-id="c3475-110">Value</span></span>|<span data-ttu-id="c3475-111">説明</span><span class="sxs-lookup"><span data-stu-id="c3475-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3475-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="c3475-112">allAllowed</span></span>|<span data-ttu-id="c3475-113">0</span><span class="sxs-lookup"><span data-stu-id="c3475-113">0</span></span>|<span data-ttu-id="c3475-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="c3475-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="c3475-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="c3475-115">allBlocked</span></span>|<span data-ttu-id="c3475-116">1</span><span class="sxs-lookup"><span data-stu-id="c3475-116">1</span></span>|<span data-ttu-id="c3475-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="c3475-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="c3475-118">children</span><span class="sxs-lookup"><span data-stu-id="c3475-118">children</span></span>|<span data-ttu-id="c3475-119">2</span><span class="sxs-lookup"><span data-stu-id="c3475-119">2</span></span>|<span data-ttu-id="c3475-120">C のクラス分けが 2 ~ 7 年間の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="c3475-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="c3475-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="c3475-121">childrenAbove8</span></span>|<span data-ttu-id="c3475-122">3</span><span class="sxs-lookup"><span data-stu-id="c3475-122">3</span></span>|<span data-ttu-id="c3475-123">C8 のクラス分けは、子供に適して古く 8 +</span><span class="sxs-lookup"><span data-stu-id="c3475-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="c3475-124">全般</span><span class="sxs-lookup"><span data-stu-id="c3475-124">general</span></span>|<span data-ttu-id="c3475-125">4</span><span class="sxs-lookup"><span data-stu-id="c3475-125">4</span></span>|<span data-ttu-id="c3475-126">G 分類が一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="c3475-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="c3475-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="c3475-127">parentalGuidance</span></span>|<span data-ttu-id="c3475-128">5</span><span class="sxs-lookup"><span data-stu-id="c3475-128">5</span></span>|<span data-ttu-id="c3475-129">PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="c3475-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="c3475-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="c3475-130">agesAbove14</span></span>|<span data-ttu-id="c3475-131">6</span><span class="sxs-lookup"><span data-stu-id="c3475-131">6</span></span>|<span data-ttu-id="c3475-132">14 と古い視聴者の年齢 14 + のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="c3475-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="c3475-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="c3475-133">agesAbove18</span></span>|<span data-ttu-id="c3475-134">7</span><span class="sxs-lookup"><span data-stu-id="c3475-134">7</span></span>|<span data-ttu-id="c3475-135">18 + のクラス分けは、視聴者の年齢 18</span><span class="sxs-lookup"><span data-stu-id="c3475-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|





