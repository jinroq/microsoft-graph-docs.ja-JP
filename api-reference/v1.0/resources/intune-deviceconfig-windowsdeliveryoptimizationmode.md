---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463895"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="f41f3-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="f41f3-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="f41f3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f41f3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f41f3-105">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="f41f3-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="f41f3-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f41f3-106">Members</span></span>
|<span data-ttu-id="f41f3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f41f3-107">Member</span></span>|<span data-ttu-id="f41f3-108">値</span><span class="sxs-lookup"><span data-stu-id="f41f3-108">Value</span></span>|<span data-ttu-id="f41f3-109">説明</span><span class="sxs-lookup"><span data-stu-id="f41f3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f41f3-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="f41f3-110">userDefined</span></span>|<span data-ttu-id="f41f3-111">.0</span><span class="sxs-lookup"><span data-stu-id="f41f3-111">0</span></span>|<span data-ttu-id="f41f3-112">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f41f3-112">Allow the user to set.</span></span>|
|<span data-ttu-id="f41f3-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="f41f3-113">httpOnly</span></span>|<span data-ttu-id="f41f3-114">1-d</span><span class="sxs-lookup"><span data-stu-id="f41f3-114">1</span></span>|<span data-ttu-id="f41f3-115">HTTP のみ、ピアリングなし</span><span class="sxs-lookup"><span data-stu-id="f41f3-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="f41f3-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="f41f3-116">httpWithPeeringNat</span></span>|<span data-ttu-id="f41f3-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f41f3-117">2</span></span>|<span data-ttu-id="f41f3-118">OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの</span><span class="sxs-lookup"><span data-stu-id="f41f3-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="f41f3-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="f41f3-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="f41f3-120">1/3</span><span class="sxs-lookup"><span data-stu-id="f41f3-120">3</span></span>|<span data-ttu-id="f41f3-121">プライベートグループ間でのピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="f41f3-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="f41f3-122">httpwithinternetpeering リング</span><span class="sxs-lookup"><span data-stu-id="f41f3-122">httpWithInternetPeering</span></span>|<span data-ttu-id="f41f3-123">2/4</span><span class="sxs-lookup"><span data-stu-id="f41f3-123">4</span></span>|<span data-ttu-id="f41f3-124">インターネットピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="f41f3-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="f41f3-125">simpledownload</span><span class="sxs-lookup"><span data-stu-id="f41f3-125">simpleDownload</span></span>|<span data-ttu-id="f41f3-126">99</span><span class="sxs-lookup"><span data-stu-id="f41f3-126">99</span></span>|<span data-ttu-id="f41f3-127">ピアリングのない簡易ダウンロードモード</span><span class="sxs-lookup"><span data-stu-id="f41f3-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="f41f3-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="f41f3-128">bypassMode</span></span>|<span data-ttu-id="f41f3-129">100</span><span class="sxs-lookup"><span data-stu-id="f41f3-129">100</span></span>|<span data-ttu-id="f41f3-130">バイパスモード。</span><span class="sxs-lookup"><span data-stu-id="f41f3-130">Bypass mode.</span></span> <span data-ttu-id="f41f3-131">配信の最適化を使用せず、代わりにビットを使用する</span><span class="sxs-lookup"><span data-stu-id="f41f3-131">Do not use Delivery Optimization and use BITS instead</span></span>|



