---
title: ratingIrelandTelevisionType 列挙型
description: アイルランドのテレビコンテンツ評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9f5360f625a9e53513752133ca619d297a1dd82
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785399"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="baea2-103">ratingIrelandTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="baea2-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="baea2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baea2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baea2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="baea2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baea2-106">アイルランドのテレビコンテンツ評価のラベル</span><span class="sxs-lookup"><span data-stu-id="baea2-106">TV content rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="baea2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="baea2-107">Members</span></span>
|<span data-ttu-id="baea2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="baea2-108">Member</span></span>|<span data-ttu-id="baea2-109">値</span><span class="sxs-lookup"><span data-stu-id="baea2-109">Value</span></span>|<span data-ttu-id="baea2-110">説明</span><span class="sxs-lookup"><span data-stu-id="baea2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baea2-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="baea2-111">allAllowed</span></span>|<span data-ttu-id="baea2-112">.0</span><span class="sxs-lookup"><span data-stu-id="baea2-112">0</span></span>|<span data-ttu-id="baea2-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="baea2-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="baea2-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="baea2-114">allBlocked</span></span>|<span data-ttu-id="baea2-115">1-d</span><span class="sxs-lookup"><span data-stu-id="baea2-115">1</span></span>|<span data-ttu-id="baea2-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="baea2-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="baea2-117">元帳</span><span class="sxs-lookup"><span data-stu-id="baea2-117">general</span></span>|<span data-ttu-id="baea2-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="baea2-118">2</span></span>|<span data-ttu-id="baea2-119">GA 分類は、すべての対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="baea2-119">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="baea2-120">children</span><span class="sxs-lookup"><span data-stu-id="baea2-120">children</span></span>|<span data-ttu-id="baea2-121">1/3</span><span class="sxs-lookup"><span data-stu-id="baea2-121">3</span></span>|<span data-ttu-id="baea2-122">CH 分類は、子に適しています。</span><span class="sxs-lookup"><span data-stu-id="baea2-122">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="baea2-123">youngAdults</span><span class="sxs-lookup"><span data-stu-id="baea2-123">youngAdults</span></span>|<span data-ttu-id="baea2-124">2/4</span><span class="sxs-lookup"><span data-stu-id="baea2-124">4</span></span>|<span data-ttu-id="baea2-125">YA の分類は、teenage 対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="baea2-125">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="baea2-126">parentalsupervision</span><span class="sxs-lookup"><span data-stu-id="baea2-126">parentalSupervision</span></span>|<span data-ttu-id="baea2-127">5</span><span class="sxs-lookup"><span data-stu-id="baea2-127">5</span></span>|<span data-ttu-id="baea2-128">PS 分類は親とガーディアンを招待して、子のアクセス制限を考慮します。</span><span class="sxs-lookup"><span data-stu-id="baea2-128">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="baea2-129">度</span><span class="sxs-lookup"><span data-stu-id="baea2-129">mature</span></span>|<span data-ttu-id="baea2-130">シックス</span><span class="sxs-lookup"><span data-stu-id="baea2-130">6</span></span>|<span data-ttu-id="baea2-131">MA 分類は、大人に適しています。</span><span class="sxs-lookup"><span data-stu-id="baea2-131">The MA classification is suitable for adults</span></span>|





