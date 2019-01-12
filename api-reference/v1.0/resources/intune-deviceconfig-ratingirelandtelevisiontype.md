---
title: ratingIrelandTelevisionType 列挙型
description: アイルランドのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb03562a32fa9a8d41ea0d68cf7cd5cf5416ac0e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967309"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="a7a2a-103">ratingIrelandTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a7a2a-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="a7a2a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7a2a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7a2a-105">アイルランドのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="a7a2a-105">TV content rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="a7a2a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a7a2a-106">Members</span></span>
|<span data-ttu-id="a7a2a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a7a2a-107">Member</span></span>|<span data-ttu-id="a7a2a-108">値</span><span class="sxs-lookup"><span data-stu-id="a7a2a-108">Value</span></span>|<span data-ttu-id="a7a2a-109">説明</span><span class="sxs-lookup"><span data-stu-id="a7a2a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7a2a-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="a7a2a-110">allAllowed</span></span>|<span data-ttu-id="a7a2a-111">0</span><span class="sxs-lookup"><span data-stu-id="a7a2a-111">0</span></span>|<span data-ttu-id="a7a2a-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="a7a2a-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="a7a2a-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="a7a2a-113">allBlocked</span></span>|<span data-ttu-id="a7a2a-114">1</span><span class="sxs-lookup"><span data-stu-id="a7a2a-114">1</span></span>|<span data-ttu-id="a7a2a-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="a7a2a-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="a7a2a-116">全般</span><span class="sxs-lookup"><span data-stu-id="a7a2a-116">general</span></span>|<span data-ttu-id="a7a2a-117">2</span><span class="sxs-lookup"><span data-stu-id="a7a2a-117">2</span></span>|<span data-ttu-id="a7a2a-118">GA クラス分けがすべての対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="a7a2a-118">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="a7a2a-119">children</span><span class="sxs-lookup"><span data-stu-id="a7a2a-119">children</span></span>|<span data-ttu-id="a7a2a-120">3</span><span class="sxs-lookup"><span data-stu-id="a7a2a-120">3</span></span>|<span data-ttu-id="a7a2a-121">CH クラス分けが子供に適しています。</span><span class="sxs-lookup"><span data-stu-id="a7a2a-121">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="a7a2a-122">youngAdults</span><span class="sxs-lookup"><span data-stu-id="a7a2a-122">youngAdults</span></span>|<span data-ttu-id="a7a2a-123">4</span><span class="sxs-lookup"><span data-stu-id="a7a2a-123">4</span></span>|<span data-ttu-id="a7a2a-124">YA クラス分けが 10 代向けに適しています。</span><span class="sxs-lookup"><span data-stu-id="a7a2a-124">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="a7a2a-125">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="a7a2a-125">parentalSupervision</span></span>|<span data-ttu-id="a7a2a-126">5</span><span class="sxs-lookup"><span data-stu-id="a7a2a-126">5</span></span>|<span data-ttu-id="a7a2a-127">PS 分類制限子供のアクセスを考慮するには、親と保護者へを招待します。</span><span class="sxs-lookup"><span data-stu-id="a7a2a-127">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="a7a2a-128">成熟</span><span class="sxs-lookup"><span data-stu-id="a7a2a-128">mature</span></span>|<span data-ttu-id="a7a2a-129">6</span><span class="sxs-lookup"><span data-stu-id="a7a2a-129">6</span></span>|<span data-ttu-id="a7a2a-130">MA クラス分けが大人に適しています。</span><span class="sxs-lookup"><span data-stu-id="a7a2a-130">The MA classification is suitable for adults</span></span>|



