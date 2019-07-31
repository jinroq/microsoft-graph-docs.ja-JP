---
title: ratingIrelandTelevisionType 列挙型
description: アイルランドのテレビコンテンツ評価のラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4e58781065d290a44e187aff8f11c746affe0474
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000663"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="eeece-103">ratingIrelandTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="eeece-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="eeece-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeece-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeece-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eeece-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeece-106">アイルランドのテレビコンテンツ評価のラベル</span><span class="sxs-lookup"><span data-stu-id="eeece-106">TV content rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="eeece-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="eeece-107">Members</span></span>
|<span data-ttu-id="eeece-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="eeece-108">Member</span></span>|<span data-ttu-id="eeece-109">値</span><span class="sxs-lookup"><span data-stu-id="eeece-109">Value</span></span>|<span data-ttu-id="eeece-110">説明</span><span class="sxs-lookup"><span data-stu-id="eeece-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeece-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="eeece-111">allAllowed</span></span>|<span data-ttu-id="eeece-112">.0</span><span class="sxs-lookup"><span data-stu-id="eeece-112">0</span></span>|<span data-ttu-id="eeece-113">既定値、すべてのテレビ番組にコンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="eeece-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="eeece-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="eeece-114">allBlocked</span></span>|<span data-ttu-id="eeece-115">1-d</span><span class="sxs-lookup"><span data-stu-id="eeece-115">1</span></span>|<span data-ttu-id="eeece-116">すべてのテレビ番組の内容を許可しない</span><span class="sxs-lookup"><span data-stu-id="eeece-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="eeece-117">元帳</span><span class="sxs-lookup"><span data-stu-id="eeece-117">general</span></span>|<span data-ttu-id="eeece-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="eeece-118">2</span></span>|<span data-ttu-id="eeece-119">GA 分類は、すべての対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="eeece-119">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="eeece-120">children</span><span class="sxs-lookup"><span data-stu-id="eeece-120">children</span></span>|<span data-ttu-id="eeece-121">1/3</span><span class="sxs-lookup"><span data-stu-id="eeece-121">3</span></span>|<span data-ttu-id="eeece-122">CH 分類は、子に適しています。</span><span class="sxs-lookup"><span data-stu-id="eeece-122">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="eeece-123">youngAdults</span><span class="sxs-lookup"><span data-stu-id="eeece-123">youngAdults</span></span>|<span data-ttu-id="eeece-124">2/4</span><span class="sxs-lookup"><span data-stu-id="eeece-124">4</span></span>|<span data-ttu-id="eeece-125">YA の分類は、teenage 対象ユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="eeece-125">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="eeece-126">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="eeece-126">parentalSupervision</span></span>|<span data-ttu-id="eeece-127">5</span><span class="sxs-lookup"><span data-stu-id="eeece-127">5</span></span>|<span data-ttu-id="eeece-128">PS 分類は親とガーディアンを招待して、子のアクセス制限を考慮します。</span><span class="sxs-lookup"><span data-stu-id="eeece-128">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="eeece-129">度</span><span class="sxs-lookup"><span data-stu-id="eeece-129">mature</span></span>|<span data-ttu-id="eeece-130">シックス</span><span class="sxs-lookup"><span data-stu-id="eeece-130">6</span></span>|<span data-ttu-id="eeece-131">MA 分類は、大人に適しています。</span><span class="sxs-lookup"><span data-stu-id="eeece-131">The MA classification is suitable for adults</span></span>|





