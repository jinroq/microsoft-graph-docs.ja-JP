---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1c146b42eab11dab4d90de9b3b134fdd29327323
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969073"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="d3e87-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="d3e87-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="d3e87-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3e87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3e87-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3e87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3e87-106">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="d3e87-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="d3e87-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3e87-107">Members</span></span>
|<span data-ttu-id="d3e87-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3e87-108">Member</span></span>|<span data-ttu-id="d3e87-109">値</span><span class="sxs-lookup"><span data-stu-id="d3e87-109">Value</span></span>|<span data-ttu-id="d3e87-110">説明</span><span class="sxs-lookup"><span data-stu-id="d3e87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3e87-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="d3e87-111">userDefined</span></span>|<span data-ttu-id="d3e87-112">.0</span><span class="sxs-lookup"><span data-stu-id="d3e87-112">0</span></span>|<span data-ttu-id="d3e87-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d3e87-113">Allow the user to set.</span></span>|
|<span data-ttu-id="d3e87-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="d3e87-114">httpOnly</span></span>|<span data-ttu-id="d3e87-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d3e87-115">1</span></span>|<span data-ttu-id="d3e87-116">HTTP のみ、ピアリングなし</span><span class="sxs-lookup"><span data-stu-id="d3e87-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="d3e87-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="d3e87-117">httpWithPeeringNat</span></span>|<span data-ttu-id="d3e87-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d3e87-118">2</span></span>|<span data-ttu-id="d3e87-119">OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの</span><span class="sxs-lookup"><span data-stu-id="d3e87-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="d3e87-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="d3e87-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="d3e87-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d3e87-121">3</span></span>|<span data-ttu-id="d3e87-122">プライベートグループ間でのピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="d3e87-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="d3e87-123">httpWithInternetPeering リング</span><span class="sxs-lookup"><span data-stu-id="d3e87-123">httpWithInternetPeering</span></span>|<span data-ttu-id="d3e87-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d3e87-124">4</span></span>|<span data-ttu-id="d3e87-125">インターネットピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="d3e87-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="d3e87-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="d3e87-126">simpleDownload</span></span>|<span data-ttu-id="d3e87-127">99</span><span class="sxs-lookup"><span data-stu-id="d3e87-127">99</span></span>|<span data-ttu-id="d3e87-128">ピアリングのない簡易ダウンロードモード</span><span class="sxs-lookup"><span data-stu-id="d3e87-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="d3e87-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="d3e87-129">bypassMode</span></span>|<span data-ttu-id="d3e87-130">100</span><span class="sxs-lookup"><span data-stu-id="d3e87-130">100</span></span>|<span data-ttu-id="d3e87-131">バイパスモード。</span><span class="sxs-lookup"><span data-stu-id="d3e87-131">Bypass mode.</span></span> <span data-ttu-id="d3e87-132">配信の最適化を使用せず、代わりにビットを使用する</span><span class="sxs-lookup"><span data-stu-id="d3e87-132">Do not use Delivery Optimization and use BITS instead</span></span>|





