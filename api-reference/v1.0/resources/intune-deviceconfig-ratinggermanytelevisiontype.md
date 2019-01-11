---
title: ratingGermanyTelevisionType 列挙型
description: ドイツのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8a1f0e16d43fe9a97f18b2bc02f2cacc8d54c7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841357"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="9ffe0-103">ratingGermanyTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9ffe0-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="9ffe0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ffe0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ffe0-105">ドイツのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="9ffe0-105">TV content rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="9ffe0-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="9ffe0-106">Members</span></span>
|<span data-ttu-id="9ffe0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9ffe0-107">Member</span></span>|<span data-ttu-id="9ffe0-108">値</span><span class="sxs-lookup"><span data-stu-id="9ffe0-108">Value</span></span>|<span data-ttu-id="9ffe0-109">説明</span><span class="sxs-lookup"><span data-stu-id="9ffe0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ffe0-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="9ffe0-110">allAllowed</span></span>|<span data-ttu-id="9ffe0-111">0</span><span class="sxs-lookup"><span data-stu-id="9ffe0-111">0</span></span>|<span data-ttu-id="9ffe0-112">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="9ffe0-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="9ffe0-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="9ffe0-113">allBlocked</span></span>|<span data-ttu-id="9ffe0-114">1</span><span class="sxs-lookup"><span data-stu-id="9ffe0-114">1</span></span>|<span data-ttu-id="9ffe0-115">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="9ffe0-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="9ffe0-116">全般</span><span class="sxs-lookup"><span data-stu-id="9ffe0-116">general</span></span>|<span data-ttu-id="9ffe0-117">2</span><span class="sxs-lookup"><span data-stu-id="9ffe0-117">2</span></span>|<span data-ttu-id="9ffe0-118">Ab 0 Jahren、年齢制限はありません。</span><span class="sxs-lookup"><span data-stu-id="9ffe0-118">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="9ffe0-119">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="9ffe0-119">agesAbove6</span></span>|<span data-ttu-id="9ffe0-120">3</span><span class="sxs-lookup"><span data-stu-id="9ffe0-120">3</span></span>|<span data-ttu-id="9ffe0-121">Ab 6 Jahren では、6 と以前のエージングします。</span><span class="sxs-lookup"><span data-stu-id="9ffe0-121">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="9ffe0-122">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="9ffe0-122">agesAbove12</span></span>|<span data-ttu-id="9ffe0-123">4</span><span class="sxs-lookup"><span data-stu-id="9ffe0-123">4</span></span>|<span data-ttu-id="9ffe0-124">Ab 12 Jahren、12 と古いのエージングします。</span><span class="sxs-lookup"><span data-stu-id="9ffe0-124">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="9ffe0-125">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="9ffe0-125">agesAbove16</span></span>|<span data-ttu-id="9ffe0-126">5</span><span class="sxs-lookup"><span data-stu-id="9ffe0-126">5</span></span>|<span data-ttu-id="9ffe0-127">Ab 16 Jahren、16 のエージングします。</span><span class="sxs-lookup"><span data-stu-id="9ffe0-127">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="9ffe0-128">大人</span><span class="sxs-lookup"><span data-stu-id="9ffe0-128">adults</span></span>|<span data-ttu-id="9ffe0-129">6</span><span class="sxs-lookup"><span data-stu-id="9ffe0-129">6</span></span>|<span data-ttu-id="9ffe0-130">Ab 18 Jahren、成人のみ</span><span class="sxs-lookup"><span data-stu-id="9ffe0-130">Ab 18 Jahren, adults only</span></span>|



