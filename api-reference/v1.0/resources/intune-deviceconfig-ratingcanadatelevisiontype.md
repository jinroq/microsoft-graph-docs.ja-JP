---
title: ratingCanadaTelevisionType 列挙型
description: カナダのテレビのコンテンツの規制ラベル
ms.openlocfilehash: 636a59e9bbb4c6ce09a9118b912cdd9c6be8440b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020540"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="bc3ec-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="bc3ec-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="bc3ec-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bc3ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc3ec-105">カナダのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="bc3ec-105">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="bc3ec-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="bc3ec-106">Members</span></span>
|<span data-ttu-id="bc3ec-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bc3ec-107">Member</span></span>|<span data-ttu-id="bc3ec-108">値</span><span class="sxs-lookup"><span data-stu-id="bc3ec-108">Value</span></span>|<span data-ttu-id="bc3ec-109">説明</span><span class="sxs-lookup"><span data-stu-id="bc3ec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc3ec-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="bc3ec-110">allAllowed</span></span>|<span data-ttu-id="bc3ec-111">0</span><span class="sxs-lookup"><span data-stu-id="bc3ec-111">0</span></span>|<span data-ttu-id="bc3ec-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="bc3ec-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="bc3ec-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="bc3ec-113">allBlocked</span></span>|<span data-ttu-id="bc3ec-114">1</span><span class="sxs-lookup"><span data-stu-id="bc3ec-114">1</span></span>|<span data-ttu-id="bc3ec-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="bc3ec-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="bc3ec-116">children</span><span class="sxs-lookup"><span data-stu-id="bc3ec-116">children</span></span>|<span data-ttu-id="bc3ec-117">2</span><span class="sxs-lookup"><span data-stu-id="bc3ec-117">2</span></span>|<span data-ttu-id="bc3ec-118">C のクラス分けが 2 ~ 7 年間の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="bc3ec-118">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="bc3ec-119">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="bc3ec-119">childrenAbove8</span></span>|<span data-ttu-id="bc3ec-120">3</span><span class="sxs-lookup"><span data-stu-id="bc3ec-120">3</span></span>|<span data-ttu-id="bc3ec-121">C8 のクラス分けは、子供に適して古く 8 +</span><span class="sxs-lookup"><span data-stu-id="bc3ec-121">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="bc3ec-122">全般</span><span class="sxs-lookup"><span data-stu-id="bc3ec-122">general</span></span>|<span data-ttu-id="bc3ec-123">4</span><span class="sxs-lookup"><span data-stu-id="bc3ec-123">4</span></span>|<span data-ttu-id="bc3ec-124">G 分類が一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="bc3ec-124">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="bc3ec-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="bc3ec-125">parentalGuidance</span></span>|<span data-ttu-id="bc3ec-126">5</span><span class="sxs-lookup"><span data-stu-id="bc3ec-126">5</span></span>|<span data-ttu-id="bc3ec-127">PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="bc3ec-127">PG, Parental Guidance</span></span>|
|<span data-ttu-id="bc3ec-128">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="bc3ec-128">agesAbove14</span></span>|<span data-ttu-id="bc3ec-129">6</span><span class="sxs-lookup"><span data-stu-id="bc3ec-129">6</span></span>|<span data-ttu-id="bc3ec-130">14 と古い視聴者の年齢 14 + のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="bc3ec-130">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="bc3ec-131">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="bc3ec-131">agesAbove18</span></span>|<span data-ttu-id="bc3ec-132">7</span><span class="sxs-lookup"><span data-stu-id="bc3ec-132">7</span></span>|<span data-ttu-id="bc3ec-133">18 + のクラス分けは、視聴者の年齢 18</span><span class="sxs-lookup"><span data-stu-id="bc3ec-133">The 18+ classification is intended for viewers ages 18 and older</span></span>|



