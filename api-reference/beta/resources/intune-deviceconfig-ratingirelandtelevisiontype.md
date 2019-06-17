---
title: ratingIrelandTelevisionType 列挙型
description: アイルランドのテレビコンテンツ評価のラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0556a00c196e3bf1f543ab034ada344dfdeb98d9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984696"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="e26d5-103">ratingIrelandTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e26d5-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="e26d5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e26d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e26d5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e26d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e26d5-106">アイルランドのテレビコンテンツ評価のラベル</span><span class="sxs-lookup"><span data-stu-id="e26d5-106">TV content rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="e26d5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e26d5-107">Members</span></span>
|<span data-ttu-id="e26d5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e26d5-108">Member</span></span>|<span data-ttu-id="e26d5-109">値</span><span class="sxs-lookup"><span data-stu-id="e26d5-109">Value</span></span>|<span data-ttu-id="e26d5-110">説明</span><span class="sxs-lookup"><span data-stu-id="e26d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e26d5-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="e26d5-111">allAllowed</span></span>|<span data-ttu-id="e26d5-112">.0</span><span class="sxs-lookup"><span data-stu-id="e26d5-112">0</span></span>|<span data-ttu-id="e26d5-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="e26d5-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="e26d5-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="e26d5-114">allBlocked</span></span>|<span data-ttu-id="e26d5-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e26d5-115">1</span></span>|<span data-ttu-id="e26d5-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="e26d5-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="e26d5-117">元帳</span><span class="sxs-lookup"><span data-stu-id="e26d5-117">general</span></span>|<span data-ttu-id="e26d5-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e26d5-118">2</span></span>|<span data-ttu-id="e26d5-119">GA 分類は、すべての対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="e26d5-119">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="e26d5-120">children</span><span class="sxs-lookup"><span data-stu-id="e26d5-120">children</span></span>|<span data-ttu-id="e26d5-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e26d5-121">3</span></span>|<span data-ttu-id="e26d5-122">CH 分類は、子に適しています。</span><span class="sxs-lookup"><span data-stu-id="e26d5-122">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="e26d5-123">youngAdults</span><span class="sxs-lookup"><span data-stu-id="e26d5-123">youngAdults</span></span>|<span data-ttu-id="e26d5-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e26d5-124">4</span></span>|<span data-ttu-id="e26d5-125">YA の分類は、teenage 対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="e26d5-125">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="e26d5-126">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="e26d5-126">parentalSupervision</span></span>|<span data-ttu-id="e26d5-127">5</span><span class="sxs-lookup"><span data-stu-id="e26d5-127">5</span></span>|<span data-ttu-id="e26d5-128">PS 分類は親とガーディアンを招待して、子のアクセス制限を考慮します。</span><span class="sxs-lookup"><span data-stu-id="e26d5-128">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="e26d5-129">度</span><span class="sxs-lookup"><span data-stu-id="e26d5-129">mature</span></span>|<span data-ttu-id="e26d5-130">シックス</span><span class="sxs-lookup"><span data-stu-id="e26d5-130">6</span></span>|<span data-ttu-id="e26d5-131">MA 分類は、大人に適しています。</span><span class="sxs-lookup"><span data-stu-id="e26d5-131">The MA classification is suitable for adults</span></span>|





