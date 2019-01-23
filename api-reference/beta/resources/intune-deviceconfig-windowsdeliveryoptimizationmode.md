---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5565965f9ba9395d7cd07b2935e6772478e0bb50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406886"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="47a6c-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="47a6c-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="47a6c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47a6c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="47a6c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47a6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47a6c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47a6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47a6c-107">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="47a6c-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="47a6c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="47a6c-108">Members</span></span>
|<span data-ttu-id="47a6c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="47a6c-109">Member</span></span>|<span data-ttu-id="47a6c-110">値</span><span class="sxs-lookup"><span data-stu-id="47a6c-110">Value</span></span>|<span data-ttu-id="47a6c-111">説明</span><span class="sxs-lookup"><span data-stu-id="47a6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a6c-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="47a6c-112">userDefined</span></span>|<span data-ttu-id="47a6c-113">0</span><span class="sxs-lookup"><span data-stu-id="47a6c-113">0</span></span>|<span data-ttu-id="47a6c-114">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="47a6c-114">Allow the user to set.</span></span>|
|<span data-ttu-id="47a6c-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="47a6c-115">httpOnly</span></span>|<span data-ttu-id="47a6c-116">1</span><span class="sxs-lookup"><span data-stu-id="47a6c-116">1</span></span>|<span data-ttu-id="47a6c-117">ないピアリングのみ、HTTP</span><span class="sxs-lookup"><span data-stu-id="47a6c-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="47a6c-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="47a6c-118">httpWithPeeringNat</span></span>|<span data-ttu-id="47a6c-119">2</span><span class="sxs-lookup"><span data-stu-id="47a6c-119">2</span></span>|<span data-ttu-id="47a6c-120">OS の既定値は – Http が同じネットワーク アドレス変換器の背後にあるピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="47a6c-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="47a6c-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="47a6c-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="47a6c-122">3</span><span class="sxs-lookup"><span data-stu-id="47a6c-122">3</span></span>|<span data-ttu-id="47a6c-123">HTTP は、プライベート グループ全体でピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="47a6c-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="47a6c-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="47a6c-124">httpWithInternetPeering</span></span>|<span data-ttu-id="47a6c-125">4</span><span class="sxs-lookup"><span data-stu-id="47a6c-125">4</span></span>|<span data-ttu-id="47a6c-126">HTTP はインターネットのピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="47a6c-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="47a6c-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="47a6c-127">simpleDownload</span></span>|<span data-ttu-id="47a6c-128">99</span><span class="sxs-lookup"><span data-stu-id="47a6c-128">99</span></span>|<span data-ttu-id="47a6c-129">ピアリングのない単純なダウンロード モード</span><span class="sxs-lookup"><span data-stu-id="47a6c-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="47a6c-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="47a6c-130">bypassMode</span></span>|<span data-ttu-id="47a6c-131">100</span><span class="sxs-lookup"><span data-stu-id="47a6c-131">100</span></span>|<span data-ttu-id="47a6c-132">バイパス モードにします。</span><span class="sxs-lookup"><span data-stu-id="47a6c-132">Bypass mode.</span></span> <span data-ttu-id="47a6c-133">配信の最適化を使用せず、代わりにビットを使用</span><span class="sxs-lookup"><span data-stu-id="47a6c-133">Do not use Delivery Optimization and use BITS instead</span></span>|




