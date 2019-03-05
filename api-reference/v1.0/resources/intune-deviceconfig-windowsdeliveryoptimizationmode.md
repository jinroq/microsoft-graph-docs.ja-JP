---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251504"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="0b27e-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="0b27e-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="0b27e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b27e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b27e-105">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="0b27e-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="0b27e-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b27e-106">Members</span></span>
|<span data-ttu-id="0b27e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b27e-107">Member</span></span>|<span data-ttu-id="0b27e-108">値</span><span class="sxs-lookup"><span data-stu-id="0b27e-108">Value</span></span>|<span data-ttu-id="0b27e-109">説明</span><span class="sxs-lookup"><span data-stu-id="0b27e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b27e-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="0b27e-110">userDefined</span></span>|<span data-ttu-id="0b27e-111">.0</span><span class="sxs-lookup"><span data-stu-id="0b27e-111">0</span></span>|<span data-ttu-id="0b27e-112">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0b27e-112">Allow the user to set.</span></span>|
|<span data-ttu-id="0b27e-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="0b27e-113">httpOnly</span></span>|<span data-ttu-id="0b27e-114">1-d</span><span class="sxs-lookup"><span data-stu-id="0b27e-114">1</span></span>|<span data-ttu-id="0b27e-115">HTTP のみ、ピアリングなし</span><span class="sxs-lookup"><span data-stu-id="0b27e-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="0b27e-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="0b27e-116">httpWithPeeringNat</span></span>|<span data-ttu-id="0b27e-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0b27e-117">2</span></span>|<span data-ttu-id="0b27e-118">OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの</span><span class="sxs-lookup"><span data-stu-id="0b27e-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="0b27e-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="0b27e-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="0b27e-120">1/3</span><span class="sxs-lookup"><span data-stu-id="0b27e-120">3</span></span>|<span data-ttu-id="0b27e-121">プライベートグループ間でのピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="0b27e-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="0b27e-122">httpwithinternetpeering リング</span><span class="sxs-lookup"><span data-stu-id="0b27e-122">httpWithInternetPeering</span></span>|<span data-ttu-id="0b27e-123">2/4</span><span class="sxs-lookup"><span data-stu-id="0b27e-123">4</span></span>|<span data-ttu-id="0b27e-124">インターネットピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="0b27e-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="0b27e-125">simpledownload</span><span class="sxs-lookup"><span data-stu-id="0b27e-125">simpleDownload</span></span>|<span data-ttu-id="0b27e-126">99</span><span class="sxs-lookup"><span data-stu-id="0b27e-126">99</span></span>|<span data-ttu-id="0b27e-127">ピアリングのない簡易ダウンロードモード</span><span class="sxs-lookup"><span data-stu-id="0b27e-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="0b27e-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="0b27e-128">bypassMode</span></span>|<span data-ttu-id="0b27e-129">100</span><span class="sxs-lookup"><span data-stu-id="0b27e-129">100</span></span>|<span data-ttu-id="0b27e-130">バイパスモード。</span><span class="sxs-lookup"><span data-stu-id="0b27e-130">Bypass mode.</span></span> <span data-ttu-id="0b27e-131">配信の最適化を使用せず、代わりにビットを使用する</span><span class="sxs-lookup"><span data-stu-id="0b27e-131">Do not use Delivery Optimization and use BITS instead</span></span>|



