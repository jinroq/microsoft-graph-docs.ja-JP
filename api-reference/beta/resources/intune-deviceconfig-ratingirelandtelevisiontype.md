---
title: ratingIrelandTelevisionType 列挙型
description: アイルランドのテレビのコンテンツの規制ラベル
author: tfitzmac
ms.openlocfilehash: 40bff39bc943257267a03fdc0ddf1b99fa06dd18
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360768"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="c7ba6-103">ratingIrelandTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c7ba6-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="c7ba6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7ba6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7ba6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7ba6-107">アイルランドのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="c7ba6-107">TV content rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="c7ba6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7ba6-108">Members</span></span>
|<span data-ttu-id="c7ba6-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7ba6-109">Member</span></span>|<span data-ttu-id="c7ba6-110">値</span><span class="sxs-lookup"><span data-stu-id="c7ba6-110">Value</span></span>|<span data-ttu-id="c7ba6-111">説明</span><span class="sxs-lookup"><span data-stu-id="c7ba6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ba6-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="c7ba6-112">allAllowed</span></span>|<span data-ttu-id="c7ba6-113">0</span><span class="sxs-lookup"><span data-stu-id="c7ba6-113">0</span></span>|<span data-ttu-id="c7ba6-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="c7ba6-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="c7ba6-115">allBlocked</span></span>|<span data-ttu-id="c7ba6-116">1</span><span class="sxs-lookup"><span data-stu-id="c7ba6-116">1</span></span>|<span data-ttu-id="c7ba6-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="c7ba6-118">全般</span><span class="sxs-lookup"><span data-stu-id="c7ba6-118">general</span></span>|<span data-ttu-id="c7ba6-119">2</span><span class="sxs-lookup"><span data-stu-id="c7ba6-119">2</span></span>|<span data-ttu-id="c7ba6-120">GA クラス分けがすべての対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-120">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="c7ba6-121">children</span><span class="sxs-lookup"><span data-stu-id="c7ba6-121">children</span></span>|<span data-ttu-id="c7ba6-122">3</span><span class="sxs-lookup"><span data-stu-id="c7ba6-122">3</span></span>|<span data-ttu-id="c7ba6-123">CH クラス分けが子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-123">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="c7ba6-124">youngAdults</span><span class="sxs-lookup"><span data-stu-id="c7ba6-124">youngAdults</span></span>|<span data-ttu-id="c7ba6-125">4</span><span class="sxs-lookup"><span data-stu-id="c7ba6-125">4</span></span>|<span data-ttu-id="c7ba6-126">YA クラス分けが 10 代向けに適しています。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-126">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="c7ba6-127">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="c7ba6-127">parentalSupervision</span></span>|<span data-ttu-id="c7ba6-128">5</span><span class="sxs-lookup"><span data-stu-id="c7ba6-128">5</span></span>|<span data-ttu-id="c7ba6-129">PS 分類制限子供のアクセスを考慮するには、親と保護者へを招待します。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-129">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="c7ba6-130">成熟</span><span class="sxs-lookup"><span data-stu-id="c7ba6-130">mature</span></span>|<span data-ttu-id="c7ba6-131">6</span><span class="sxs-lookup"><span data-stu-id="c7ba6-131">6</span></span>|<span data-ttu-id="c7ba6-132">MA クラス分けが大人に適しています。</span><span class="sxs-lookup"><span data-stu-id="c7ba6-132">The MA classification is suitable for adults</span></span>|





