---
title: ratingCanadaTelevisionType 列挙型
description: カナダのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14e6ac55f0b69f00e53015153aecd511ba0086f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951489"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="f0b76-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f0b76-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="f0b76-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0b76-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0b76-105">カナダのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="f0b76-105">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="f0b76-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0b76-106">Members</span></span>
|<span data-ttu-id="f0b76-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0b76-107">Member</span></span>|<span data-ttu-id="f0b76-108">値</span><span class="sxs-lookup"><span data-stu-id="f0b76-108">Value</span></span>|<span data-ttu-id="f0b76-109">説明</span><span class="sxs-lookup"><span data-stu-id="f0b76-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0b76-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f0b76-110">allAllowed</span></span>|<span data-ttu-id="f0b76-111">0</span><span class="sxs-lookup"><span data-stu-id="f0b76-111">0</span></span>|<span data-ttu-id="f0b76-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="f0b76-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="f0b76-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f0b76-113">allBlocked</span></span>|<span data-ttu-id="f0b76-114">1</span><span class="sxs-lookup"><span data-stu-id="f0b76-114">1</span></span>|<span data-ttu-id="f0b76-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="f0b76-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="f0b76-116">children</span><span class="sxs-lookup"><span data-stu-id="f0b76-116">children</span></span>|<span data-ttu-id="f0b76-117">2</span><span class="sxs-lookup"><span data-stu-id="f0b76-117">2</span></span>|<span data-ttu-id="f0b76-118">C のクラス分けが 2 ~ 7 年間の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="f0b76-118">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="f0b76-119">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="f0b76-119">childrenAbove8</span></span>|<span data-ttu-id="f0b76-120">3</span><span class="sxs-lookup"><span data-stu-id="f0b76-120">3</span></span>|<span data-ttu-id="f0b76-121">C8 のクラス分けは、子供に適して古く 8 +</span><span class="sxs-lookup"><span data-stu-id="f0b76-121">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="f0b76-122">全般</span><span class="sxs-lookup"><span data-stu-id="f0b76-122">general</span></span>|<span data-ttu-id="f0b76-123">4</span><span class="sxs-lookup"><span data-stu-id="f0b76-123">4</span></span>|<span data-ttu-id="f0b76-124">G 分類が一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="f0b76-124">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="f0b76-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="f0b76-125">parentalGuidance</span></span>|<span data-ttu-id="f0b76-126">5</span><span class="sxs-lookup"><span data-stu-id="f0b76-126">5</span></span>|<span data-ttu-id="f0b76-127">PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="f0b76-127">PG, Parental Guidance</span></span>|
|<span data-ttu-id="f0b76-128">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="f0b76-128">agesAbove14</span></span>|<span data-ttu-id="f0b76-129">6</span><span class="sxs-lookup"><span data-stu-id="f0b76-129">6</span></span>|<span data-ttu-id="f0b76-130">14 と古い視聴者の年齢 14 + のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="f0b76-130">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="f0b76-131">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="f0b76-131">agesAbove18</span></span>|<span data-ttu-id="f0b76-132">7</span><span class="sxs-lookup"><span data-stu-id="f0b76-132">7</span></span>|<span data-ttu-id="f0b76-133">18 + のクラス分けは、視聴者の年齢 18</span><span class="sxs-lookup"><span data-stu-id="f0b76-133">The 18+ classification is intended for viewers ages 18 and older</span></span>|



