---
title: ratingGermanyTelevisionType 列挙型
description: ドイツでのテレビコンテンツの評価のラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cc91bd7988dbc8f1c1f36d4aaf28e10d2609710
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566669"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="6fc21-103">ratingGermanyTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6fc21-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="6fc21-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fc21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fc21-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6fc21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fc21-106">ドイツでのテレビコンテンツの評価のラベル</span><span class="sxs-lookup"><span data-stu-id="6fc21-106">TV content rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="6fc21-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6fc21-107">Members</span></span>
|<span data-ttu-id="6fc21-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6fc21-108">Member</span></span>|<span data-ttu-id="6fc21-109">値</span><span class="sxs-lookup"><span data-stu-id="6fc21-109">Value</span></span>|<span data-ttu-id="6fc21-110">説明</span><span class="sxs-lookup"><span data-stu-id="6fc21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc21-111">allallowed</span><span class="sxs-lookup"><span data-stu-id="6fc21-111">allAllowed</span></span>|<span data-ttu-id="6fc21-112">.0</span><span class="sxs-lookup"><span data-stu-id="6fc21-112">0</span></span>|<span data-ttu-id="6fc21-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="6fc21-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="6fc21-114">allblocked</span><span class="sxs-lookup"><span data-stu-id="6fc21-114">allBlocked</span></span>|<span data-ttu-id="6fc21-115">1 </span><span class="sxs-lookup"><span data-stu-id="6fc21-115">1</span></span>|<span data-ttu-id="6fc21-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="6fc21-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="6fc21-117">元帳</span><span class="sxs-lookup"><span data-stu-id="6fc21-117">general</span></span>|<span data-ttu-id="6fc21-118">2 </span><span class="sxs-lookup"><span data-stu-id="6fc21-118">2</span></span>|<span data-ttu-id="6fc21-119">Ab 0 Jahren、年齢制限なし</span><span class="sxs-lookup"><span data-stu-id="6fc21-119">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="6fc21-120">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="6fc21-120">agesAbove6</span></span>|<span data-ttu-id="6fc21-121">3 </span><span class="sxs-lookup"><span data-stu-id="6fc21-121">3</span></span>|<span data-ttu-id="6fc21-122">Ab 6 Jahren、才を過ぎた</span><span class="sxs-lookup"><span data-stu-id="6fc21-122">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="6fc21-123">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="6fc21-123">agesAbove12</span></span>|<span data-ttu-id="6fc21-124">4 </span><span class="sxs-lookup"><span data-stu-id="6fc21-124">4</span></span>|<span data-ttu-id="6fc21-125">Ab 12 Jahren、12才以上</span><span class="sxs-lookup"><span data-stu-id="6fc21-125">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="6fc21-126">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="6fc21-126">agesAbove16</span></span>|<span data-ttu-id="6fc21-127">5 </span><span class="sxs-lookup"><span data-stu-id="6fc21-127">5</span></span>|<span data-ttu-id="6fc21-128">Ab 16 Jahren、16才以上</span><span class="sxs-lookup"><span data-stu-id="6fc21-128">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="6fc21-129">保護者</span><span class="sxs-lookup"><span data-stu-id="6fc21-129">adults</span></span>|<span data-ttu-id="6fc21-130">6 </span><span class="sxs-lookup"><span data-stu-id="6fc21-130">6</span></span>|<span data-ttu-id="6fc21-131">Ab 18 Jahren、大人のみ</span><span class="sxs-lookup"><span data-stu-id="6fc21-131">Ab 18 Jahren, adults only</span></span>|





