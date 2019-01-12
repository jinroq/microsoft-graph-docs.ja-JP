---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f80c6b5cbe7316c851954154bdb559f370f02b79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951517"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="92e2c-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="92e2c-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="92e2c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="92e2c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92e2c-105">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="92e2c-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="92e2c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="92e2c-106">Members</span></span>
|<span data-ttu-id="92e2c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="92e2c-107">Member</span></span>|<span data-ttu-id="92e2c-108">値</span><span class="sxs-lookup"><span data-stu-id="92e2c-108">Value</span></span>|<span data-ttu-id="92e2c-109">説明</span><span class="sxs-lookup"><span data-stu-id="92e2c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e2c-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="92e2c-110">userDefined</span></span>|<span data-ttu-id="92e2c-111">0</span><span class="sxs-lookup"><span data-stu-id="92e2c-111">0</span></span>|<span data-ttu-id="92e2c-112">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="92e2c-112">Allow the user to set.</span></span>|
|<span data-ttu-id="92e2c-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="92e2c-113">httpOnly</span></span>|<span data-ttu-id="92e2c-114">1</span><span class="sxs-lookup"><span data-stu-id="92e2c-114">1</span></span>|<span data-ttu-id="92e2c-115">ないピアリングのみ、HTTP</span><span class="sxs-lookup"><span data-stu-id="92e2c-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="92e2c-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="92e2c-116">httpWithPeeringNat</span></span>|<span data-ttu-id="92e2c-117">2</span><span class="sxs-lookup"><span data-stu-id="92e2c-117">2</span></span>|<span data-ttu-id="92e2c-118">OS の既定値は – Http が同じネットワーク アドレス変換器の背後にあるピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="92e2c-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="92e2c-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="92e2c-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="92e2c-120">3</span><span class="sxs-lookup"><span data-stu-id="92e2c-120">3</span></span>|<span data-ttu-id="92e2c-121">HTTP は、プライベート グループ全体でピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="92e2c-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="92e2c-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="92e2c-122">httpWithInternetPeering</span></span>|<span data-ttu-id="92e2c-123">4</span><span class="sxs-lookup"><span data-stu-id="92e2c-123">4</span></span>|<span data-ttu-id="92e2c-124">HTTP はインターネットのピアリングとブレンド</span><span class="sxs-lookup"><span data-stu-id="92e2c-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="92e2c-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="92e2c-125">simpleDownload</span></span>|<span data-ttu-id="92e2c-126">99</span><span class="sxs-lookup"><span data-stu-id="92e2c-126">99</span></span>|<span data-ttu-id="92e2c-127">ピアリングのない単純なダウンロード モード</span><span class="sxs-lookup"><span data-stu-id="92e2c-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="92e2c-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="92e2c-128">bypassMode</span></span>|<span data-ttu-id="92e2c-129">100</span><span class="sxs-lookup"><span data-stu-id="92e2c-129">100</span></span>|<span data-ttu-id="92e2c-130">バイパス モードにします。</span><span class="sxs-lookup"><span data-stu-id="92e2c-130">Bypass mode.</span></span> <span data-ttu-id="92e2c-131">配信の最適化を使用せず、代わりにビットを使用</span><span class="sxs-lookup"><span data-stu-id="92e2c-131">Do not use Delivery Optimization and use BITS instead</span></span>|



