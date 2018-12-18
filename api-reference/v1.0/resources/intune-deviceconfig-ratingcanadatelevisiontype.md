---
title: ratingCanadaTelevisionType 列挙型
description: カナダのテレビのコンテンツの規制ラベル
author: tfitzmac
ms.openlocfilehash: cf11640b65fd5f0e724c7866dc14322306c3f760
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338711"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="74d35-103">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="74d35-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="74d35-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="74d35-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74d35-105">カナダのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="74d35-105">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="74d35-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="74d35-106">Members</span></span>
|<span data-ttu-id="74d35-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="74d35-107">Member</span></span>|<span data-ttu-id="74d35-108">値</span><span class="sxs-lookup"><span data-stu-id="74d35-108">Value</span></span>|<span data-ttu-id="74d35-109">説明</span><span class="sxs-lookup"><span data-stu-id="74d35-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74d35-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="74d35-110">allAllowed</span></span>|<span data-ttu-id="74d35-111">0</span><span class="sxs-lookup"><span data-stu-id="74d35-111">0</span></span>|<span data-ttu-id="74d35-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="74d35-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="74d35-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="74d35-113">allBlocked</span></span>|<span data-ttu-id="74d35-114">1</span><span class="sxs-lookup"><span data-stu-id="74d35-114">1</span></span>|<span data-ttu-id="74d35-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="74d35-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="74d35-116">children</span><span class="sxs-lookup"><span data-stu-id="74d35-116">children</span></span>|<span data-ttu-id="74d35-117">2</span><span class="sxs-lookup"><span data-stu-id="74d35-117">2</span></span>|<span data-ttu-id="74d35-118">C のクラス分けが 2 ~ 7 年間の子供の年齢に適しています。</span><span class="sxs-lookup"><span data-stu-id="74d35-118">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="74d35-119">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="74d35-119">childrenAbove8</span></span>|<span data-ttu-id="74d35-120">3</span><span class="sxs-lookup"><span data-stu-id="74d35-120">3</span></span>|<span data-ttu-id="74d35-121">C8 のクラス分けは、子供に適して古く 8 +</span><span class="sxs-lookup"><span data-stu-id="74d35-121">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="74d35-122">全般</span><span class="sxs-lookup"><span data-stu-id="74d35-122">general</span></span>|<span data-ttu-id="74d35-123">4</span><span class="sxs-lookup"><span data-stu-id="74d35-123">4</span></span>|<span data-ttu-id="74d35-124">G 分類が一般的な対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="74d35-124">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="74d35-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="74d35-125">parentalGuidance</span></span>|<span data-ttu-id="74d35-126">5</span><span class="sxs-lookup"><span data-stu-id="74d35-126">5</span></span>|<span data-ttu-id="74d35-127">PG、保護者による制限</span><span class="sxs-lookup"><span data-stu-id="74d35-127">PG, Parental Guidance</span></span>|
|<span data-ttu-id="74d35-128">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="74d35-128">agesAbove14</span></span>|<span data-ttu-id="74d35-129">6</span><span class="sxs-lookup"><span data-stu-id="74d35-129">6</span></span>|<span data-ttu-id="74d35-130">14 と古い視聴者の年齢 14 + のクラス分けは、します。</span><span class="sxs-lookup"><span data-stu-id="74d35-130">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="74d35-131">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="74d35-131">agesAbove18</span></span>|<span data-ttu-id="74d35-132">7</span><span class="sxs-lookup"><span data-stu-id="74d35-132">7</span></span>|<span data-ttu-id="74d35-133">18 + のクラス分けは、視聴者の年齢 18</span><span class="sxs-lookup"><span data-stu-id="74d35-133">The 18+ classification is intended for viewers ages 18 and older</span></span>|



