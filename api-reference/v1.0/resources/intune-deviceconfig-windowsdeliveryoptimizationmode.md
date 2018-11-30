---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
ms.openlocfilehash: 2d393a82f855f3e3a0226c8ccb450fa2dae1a95c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021599"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="80855-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="80855-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="80855-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80855-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80855-105">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="80855-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="80855-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="80855-106">Members</span></span>
|<span data-ttu-id="80855-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="80855-107">Member</span></span>|<span data-ttu-id="80855-108">値</span><span class="sxs-lookup"><span data-stu-id="80855-108">Value</span></span>|<span data-ttu-id="80855-109">説明</span><span class="sxs-lookup"><span data-stu-id="80855-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80855-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="80855-110">userDefined</span></span>|<span data-ttu-id="80855-111">0</span><span class="sxs-lookup"><span data-stu-id="80855-111">0</span></span>|<span data-ttu-id="80855-112">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="80855-112">Allow the user to set.</span></span>|
|<span data-ttu-id="80855-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="80855-113">httpOnly</span></span>|<span data-ttu-id="80855-114">1</span><span class="sxs-lookup"><span data-stu-id="80855-114">1</span></span>|<span data-ttu-id="80855-115">ないピアリングのみ、HTTP</span><span class="sxs-lookup"><span data-stu-id="80855-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="80855-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="80855-116">httpWithPeeringNat</span></span>|<span data-ttu-id="80855-117">2</span><span class="sxs-lookup"><span data-stu-id="80855-117">2</span></span>|<span data-ttu-id="80855-118">OS の既定値は – Http が同じネットワーク アドレス変換器の背後にあるピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="80855-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="80855-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="80855-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="80855-120">3</span><span class="sxs-lookup"><span data-stu-id="80855-120">3</span></span>|<span data-ttu-id="80855-121">HTTP は、プライベート グループ全体でピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="80855-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="80855-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="80855-122">httpWithInternetPeering</span></span>|<span data-ttu-id="80855-123">4</span><span class="sxs-lookup"><span data-stu-id="80855-123">4</span></span>|<span data-ttu-id="80855-124">HTTP はインターネットのピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="80855-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="80855-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="80855-125">simpleDownload</span></span>|<span data-ttu-id="80855-126">99</span><span class="sxs-lookup"><span data-stu-id="80855-126">99</span></span>|<span data-ttu-id="80855-127">ピアリングのない単純なダウンロード モード</span><span class="sxs-lookup"><span data-stu-id="80855-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="80855-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="80855-128">bypassMode</span></span>|<span data-ttu-id="80855-129">100</span><span class="sxs-lookup"><span data-stu-id="80855-129">100</span></span>|<span data-ttu-id="80855-130">バイパス モードにします。</span><span class="sxs-lookup"><span data-stu-id="80855-130">Bypass mode.</span></span> <span data-ttu-id="80855-131">配信の最適化を使用せず、代わりにビットを使用</span><span class="sxs-lookup"><span data-stu-id="80855-131">Do not use Delivery Optimization and use BITS instead</span></span>|



