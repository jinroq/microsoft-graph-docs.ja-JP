---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3872b7c09c8934e95725565b83cc195d9b9d8da5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785294"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="ca4e6-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="ca4e6-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="ca4e6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca4e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca4e6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca4e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca4e6-106">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="ca4e6-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="ca4e6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ca4e6-107">Members</span></span>
|<span data-ttu-id="ca4e6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ca4e6-108">Member</span></span>|<span data-ttu-id="ca4e6-109">値</span><span class="sxs-lookup"><span data-stu-id="ca4e6-109">Value</span></span>|<span data-ttu-id="ca4e6-110">説明</span><span class="sxs-lookup"><span data-stu-id="ca4e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca4e6-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="ca4e6-111">userDefined</span></span>|<span data-ttu-id="ca4e6-112">.0</span><span class="sxs-lookup"><span data-stu-id="ca4e6-112">0</span></span>|<span data-ttu-id="ca4e6-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ca4e6-113">Allow the user to set.</span></span>|
|<span data-ttu-id="ca4e6-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="ca4e6-114">httpOnly</span></span>|<span data-ttu-id="ca4e6-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ca4e6-115">1</span></span>|<span data-ttu-id="ca4e6-116">HTTP のみ、ピアリングなし</span><span class="sxs-lookup"><span data-stu-id="ca4e6-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="ca4e6-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="ca4e6-117">httpWithPeeringNat</span></span>|<span data-ttu-id="ca4e6-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ca4e6-118">2</span></span>|<span data-ttu-id="ca4e6-119">OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの</span><span class="sxs-lookup"><span data-stu-id="ca4e6-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="ca4e6-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="ca4e6-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="ca4e6-121">1/3</span><span class="sxs-lookup"><span data-stu-id="ca4e6-121">3</span></span>|<span data-ttu-id="ca4e6-122">プライベートグループ間でのピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="ca4e6-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="ca4e6-123">httpwithinternetpeering リング</span><span class="sxs-lookup"><span data-stu-id="ca4e6-123">httpWithInternetPeering</span></span>|<span data-ttu-id="ca4e6-124">2/4</span><span class="sxs-lookup"><span data-stu-id="ca4e6-124">4</span></span>|<span data-ttu-id="ca4e6-125">インターネットピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="ca4e6-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="ca4e6-126">simpledownload</span><span class="sxs-lookup"><span data-stu-id="ca4e6-126">simpleDownload</span></span>|<span data-ttu-id="ca4e6-127">99</span><span class="sxs-lookup"><span data-stu-id="ca4e6-127">99</span></span>|<span data-ttu-id="ca4e6-128">ピアリングのない簡易ダウンロードモード</span><span class="sxs-lookup"><span data-stu-id="ca4e6-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="ca4e6-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="ca4e6-129">bypassMode</span></span>|<span data-ttu-id="ca4e6-130">100</span><span class="sxs-lookup"><span data-stu-id="ca4e6-130">100</span></span>|<span data-ttu-id="ca4e6-131">バイパスモード。</span><span class="sxs-lookup"><span data-stu-id="ca4e6-131">Bypass mode.</span></span> <span data-ttu-id="ca4e6-132">配信の最適化を使用せず、代わりにビットを使用する</span><span class="sxs-lookup"><span data-stu-id="ca4e6-132">Do not use Delivery Optimization and use BITS instead</span></span>|





