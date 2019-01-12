---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 004bb3d3984d8d304f89dc339899035d218546a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972657"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="a4361-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="a4361-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="a4361-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4361-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4361-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4361-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4361-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4361-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4361-107">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="a4361-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="a4361-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a4361-108">Members</span></span>
|<span data-ttu-id="a4361-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a4361-109">Member</span></span>|<span data-ttu-id="a4361-110">値</span><span class="sxs-lookup"><span data-stu-id="a4361-110">Value</span></span>|<span data-ttu-id="a4361-111">説明</span><span class="sxs-lookup"><span data-stu-id="a4361-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4361-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="a4361-112">userDefined</span></span>|<span data-ttu-id="a4361-113">0</span><span class="sxs-lookup"><span data-stu-id="a4361-113">0</span></span>|<span data-ttu-id="a4361-114">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="a4361-114">Allow the user to set.</span></span>|
|<span data-ttu-id="a4361-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="a4361-115">httpOnly</span></span>|<span data-ttu-id="a4361-116">1</span><span class="sxs-lookup"><span data-stu-id="a4361-116">1</span></span>|<span data-ttu-id="a4361-117">ないピアリングのみ、HTTP</span><span class="sxs-lookup"><span data-stu-id="a4361-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="a4361-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="a4361-118">httpWithPeeringNat</span></span>|<span data-ttu-id="a4361-119">2</span><span class="sxs-lookup"><span data-stu-id="a4361-119">2</span></span>|<span data-ttu-id="a4361-120">OS の既定値は – Http が同じネットワーク アドレス変換器の背後にあるピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="a4361-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="a4361-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="a4361-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="a4361-122">3</span><span class="sxs-lookup"><span data-stu-id="a4361-122">3</span></span>|<span data-ttu-id="a4361-123">HTTP は、プライベート グループ全体でピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="a4361-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="a4361-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="a4361-124">httpWithInternetPeering</span></span>|<span data-ttu-id="a4361-125">4</span><span class="sxs-lookup"><span data-stu-id="a4361-125">4</span></span>|<span data-ttu-id="a4361-126">HTTP はインターネットのピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="a4361-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="a4361-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="a4361-127">simpleDownload</span></span>|<span data-ttu-id="a4361-128">99</span><span class="sxs-lookup"><span data-stu-id="a4361-128">99</span></span>|<span data-ttu-id="a4361-129">ピアリングのない単純なダウンロード モード</span><span class="sxs-lookup"><span data-stu-id="a4361-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="a4361-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="a4361-130">bypassMode</span></span>|<span data-ttu-id="a4361-131">100</span><span class="sxs-lookup"><span data-stu-id="a4361-131">100</span></span>|<span data-ttu-id="a4361-132">バイパス モードにします。</span><span class="sxs-lookup"><span data-stu-id="a4361-132">Bypass mode.</span></span> <span data-ttu-id="a4361-133">配信の最適化を使用せず、代わりにビットを使用</span><span class="sxs-lookup"><span data-stu-id="a4361-133">Do not use Delivery Optimization and use BITS instead</span></span>|





