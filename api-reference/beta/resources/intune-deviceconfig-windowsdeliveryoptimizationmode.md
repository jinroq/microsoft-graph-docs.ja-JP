---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e020b4f32cc9075acab6c783b4e9df3eb19a438b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944125"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="bea40-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="bea40-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="bea40-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bea40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bea40-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bea40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bea40-106">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="bea40-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="bea40-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bea40-107">Members</span></span>
|<span data-ttu-id="bea40-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bea40-108">Member</span></span>|<span data-ttu-id="bea40-109">値</span><span class="sxs-lookup"><span data-stu-id="bea40-109">Value</span></span>|<span data-ttu-id="bea40-110">説明</span><span class="sxs-lookup"><span data-stu-id="bea40-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bea40-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="bea40-111">userDefined</span></span>|<span data-ttu-id="bea40-112">.0</span><span class="sxs-lookup"><span data-stu-id="bea40-112">0</span></span>|<span data-ttu-id="bea40-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="bea40-113">Allow the user to set.</span></span>|
|<span data-ttu-id="bea40-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="bea40-114">httpOnly</span></span>|<span data-ttu-id="bea40-115">1-d</span><span class="sxs-lookup"><span data-stu-id="bea40-115">1</span></span>|<span data-ttu-id="bea40-116">HTTP のみ、ピアリングなし</span><span class="sxs-lookup"><span data-stu-id="bea40-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="bea40-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="bea40-117">httpWithPeeringNat</span></span>|<span data-ttu-id="bea40-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="bea40-118">2</span></span>|<span data-ttu-id="bea40-119">OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの</span><span class="sxs-lookup"><span data-stu-id="bea40-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="bea40-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="bea40-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="bea40-121">1/3</span><span class="sxs-lookup"><span data-stu-id="bea40-121">3</span></span>|<span data-ttu-id="bea40-122">プライベートグループ間でのピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="bea40-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="bea40-123">httpWithInternetPeering リング</span><span class="sxs-lookup"><span data-stu-id="bea40-123">httpWithInternetPeering</span></span>|<span data-ttu-id="bea40-124">2/4</span><span class="sxs-lookup"><span data-stu-id="bea40-124">4</span></span>|<span data-ttu-id="bea40-125">インターネットピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="bea40-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="bea40-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="bea40-126">simpleDownload</span></span>|<span data-ttu-id="bea40-127">99</span><span class="sxs-lookup"><span data-stu-id="bea40-127">99</span></span>|<span data-ttu-id="bea40-128">ピアリングのない簡易ダウンロードモード</span><span class="sxs-lookup"><span data-stu-id="bea40-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="bea40-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="bea40-129">bypassMode</span></span>|<span data-ttu-id="bea40-130">100</span><span class="sxs-lookup"><span data-stu-id="bea40-130">100</span></span>|<span data-ttu-id="bea40-131">バイパスモード。</span><span class="sxs-lookup"><span data-stu-id="bea40-131">Bypass mode.</span></span> <span data-ttu-id="bea40-132">配信の最適化を使用せず、代わりにビットを使用する</span><span class="sxs-lookup"><span data-stu-id="bea40-132">Do not use Delivery Optimization and use BITS instead</span></span>|




