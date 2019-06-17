---
title: ratingGermanyTelevisionType 列挙型
description: ドイツでのテレビコンテンツの評価のラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c881f729a9b0af57c53515af88afe311fe8a877
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984640"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="3b130-103">ratingGermanyTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3b130-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="3b130-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b130-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b130-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3b130-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b130-106">ドイツでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="3b130-106">TV content rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="3b130-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b130-107">Members</span></span>
|<span data-ttu-id="3b130-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b130-108">Member</span></span>|<span data-ttu-id="3b130-109">値</span><span class="sxs-lookup"><span data-stu-id="3b130-109">Value</span></span>|<span data-ttu-id="3b130-110">説明</span><span class="sxs-lookup"><span data-stu-id="3b130-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b130-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="3b130-111">allAllowed</span></span>|<span data-ttu-id="3b130-112">.0</span><span class="sxs-lookup"><span data-stu-id="3b130-112">0</span></span>|<span data-ttu-id="3b130-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="3b130-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="3b130-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="3b130-114">allBlocked</span></span>|<span data-ttu-id="3b130-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3b130-115">1</span></span>|<span data-ttu-id="3b130-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="3b130-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="3b130-117">元帳</span><span class="sxs-lookup"><span data-stu-id="3b130-117">general</span></span>|<span data-ttu-id="3b130-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3b130-118">2</span></span>|<span data-ttu-id="3b130-119">Ab 0 Jahren、年齢制限なし</span><span class="sxs-lookup"><span data-stu-id="3b130-119">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="3b130-120">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="3b130-120">agesAbove6</span></span>|<span data-ttu-id="3b130-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3b130-121">3</span></span>|<span data-ttu-id="3b130-122">Ab 6 Jahren、才を過ぎた</span><span class="sxs-lookup"><span data-stu-id="3b130-122">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="3b130-123">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="3b130-123">agesAbove12</span></span>|<span data-ttu-id="3b130-124">2/4</span><span class="sxs-lookup"><span data-stu-id="3b130-124">4</span></span>|<span data-ttu-id="3b130-125">Ab 12 Jahren、12才以上</span><span class="sxs-lookup"><span data-stu-id="3b130-125">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="3b130-126">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="3b130-126">agesAbove16</span></span>|<span data-ttu-id="3b130-127">5</span><span class="sxs-lookup"><span data-stu-id="3b130-127">5</span></span>|<span data-ttu-id="3b130-128">Ab 16 Jahren、16才以上</span><span class="sxs-lookup"><span data-stu-id="3b130-128">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="3b130-129">保護者</span><span class="sxs-lookup"><span data-stu-id="3b130-129">adults</span></span>|<span data-ttu-id="3b130-130">シックス</span><span class="sxs-lookup"><span data-stu-id="3b130-130">6</span></span>|<span data-ttu-id="3b130-131">Ab 18 Jahren、大人のみ</span><span class="sxs-lookup"><span data-stu-id="3b130-131">Ab 18 Jahren, adults only</span></span>|





