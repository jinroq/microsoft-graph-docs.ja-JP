---
title: ratingIrelandTelevisionType 列挙型
description: アイルランドのテレビのコンテンツの規制ラベル
ms.openlocfilehash: b81a48a5f9ea74861eb0b6ed71c7cee52c3df5be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073345"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="8434e-103">ratingIrelandTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8434e-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="8434e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8434e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8434e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8434e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8434e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8434e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8434e-107">アイルランドのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="8434e-107">TV content rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="8434e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8434e-108">Members</span></span>
|<span data-ttu-id="8434e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8434e-109">Member</span></span>|<span data-ttu-id="8434e-110">値</span><span class="sxs-lookup"><span data-stu-id="8434e-110">Value</span></span>|<span data-ttu-id="8434e-111">説明</span><span class="sxs-lookup"><span data-stu-id="8434e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8434e-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="8434e-112">allAllowed</span></span>|<span data-ttu-id="8434e-113">0</span><span class="sxs-lookup"><span data-stu-id="8434e-113">0</span></span>|<span data-ttu-id="8434e-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="8434e-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="8434e-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="8434e-115">allBlocked</span></span>|<span data-ttu-id="8434e-116">1</span><span class="sxs-lookup"><span data-stu-id="8434e-116">1</span></span>|<span data-ttu-id="8434e-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="8434e-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="8434e-118">全般</span><span class="sxs-lookup"><span data-stu-id="8434e-118">general</span></span>|<span data-ttu-id="8434e-119">2</span><span class="sxs-lookup"><span data-stu-id="8434e-119">2</span></span>|<span data-ttu-id="8434e-120">GA クラス分けがすべての対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="8434e-120">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="8434e-121">children</span><span class="sxs-lookup"><span data-stu-id="8434e-121">children</span></span>|<span data-ttu-id="8434e-122">3</span><span class="sxs-lookup"><span data-stu-id="8434e-122">3</span></span>|<span data-ttu-id="8434e-123">CH クラス分けが子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="8434e-123">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="8434e-124">youngAdults</span><span class="sxs-lookup"><span data-stu-id="8434e-124">youngAdults</span></span>|<span data-ttu-id="8434e-125">4</span><span class="sxs-lookup"><span data-stu-id="8434e-125">4</span></span>|<span data-ttu-id="8434e-126">YA クラス分けが 10 代向けに適しています。</span><span class="sxs-lookup"><span data-stu-id="8434e-126">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="8434e-127">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="8434e-127">parentalSupervision</span></span>|<span data-ttu-id="8434e-128">5</span><span class="sxs-lookup"><span data-stu-id="8434e-128">5</span></span>|<span data-ttu-id="8434e-129">PS 分類制限子供のアクセスを考慮するには、親と保護者へを招待します。</span><span class="sxs-lookup"><span data-stu-id="8434e-129">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="8434e-130">成熟</span><span class="sxs-lookup"><span data-stu-id="8434e-130">mature</span></span>|<span data-ttu-id="8434e-131">6</span><span class="sxs-lookup"><span data-stu-id="8434e-131">6</span></span>|<span data-ttu-id="8434e-132">MA クラス分けが大人に適しています。</span><span class="sxs-lookup"><span data-stu-id="8434e-132">The MA classification is suitable for adults</span></span>|





