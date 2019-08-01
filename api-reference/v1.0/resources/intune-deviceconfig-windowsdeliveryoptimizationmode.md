---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9154a78af87dbef125e5d211aba284d7a0023e84
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027651"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="45883-103">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="45883-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="45883-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45883-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45883-105">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="45883-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="45883-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="45883-106">Members</span></span>
|<span data-ttu-id="45883-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="45883-107">Member</span></span>|<span data-ttu-id="45883-108">値</span><span class="sxs-lookup"><span data-stu-id="45883-108">Value</span></span>|<span data-ttu-id="45883-109">説明</span><span class="sxs-lookup"><span data-stu-id="45883-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45883-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="45883-110">userDefined</span></span>|<span data-ttu-id="45883-111">.0</span><span class="sxs-lookup"><span data-stu-id="45883-111">0</span></span>|<span data-ttu-id="45883-112">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="45883-112">Allow the user to set.</span></span>|
|<span data-ttu-id="45883-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="45883-113">httpOnly</span></span>|<span data-ttu-id="45883-114">1-d</span><span class="sxs-lookup"><span data-stu-id="45883-114">1</span></span>|<span data-ttu-id="45883-115">HTTP のみ、ピアリングなし</span><span class="sxs-lookup"><span data-stu-id="45883-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="45883-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="45883-116">httpWithPeeringNat</span></span>|<span data-ttu-id="45883-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="45883-117">2</span></span>|<span data-ttu-id="45883-118">OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの</span><span class="sxs-lookup"><span data-stu-id="45883-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="45883-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="45883-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="45883-120">1/3</span><span class="sxs-lookup"><span data-stu-id="45883-120">3</span></span>|<span data-ttu-id="45883-121">プライベートグループ間でのピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="45883-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="45883-122">httpWithInternetPeering リング</span><span class="sxs-lookup"><span data-stu-id="45883-122">httpWithInternetPeering</span></span>|<span data-ttu-id="45883-123">2/4</span><span class="sxs-lookup"><span data-stu-id="45883-123">4</span></span>|<span data-ttu-id="45883-124">インターネットピアリングとの HTTP ブレンディング</span><span class="sxs-lookup"><span data-stu-id="45883-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="45883-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="45883-125">simpleDownload</span></span>|<span data-ttu-id="45883-126">99</span><span class="sxs-lookup"><span data-stu-id="45883-126">99</span></span>|<span data-ttu-id="45883-127">ピアリングのない簡易ダウンロードモード</span><span class="sxs-lookup"><span data-stu-id="45883-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="45883-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="45883-128">bypassMode</span></span>|<span data-ttu-id="45883-129">100</span><span class="sxs-lookup"><span data-stu-id="45883-129">100</span></span>|<span data-ttu-id="45883-130">バイパスモード。</span><span class="sxs-lookup"><span data-stu-id="45883-130">Bypass mode.</span></span> <span data-ttu-id="45883-131">配信の最適化を使用せず、代わりにビットを使用する</span><span class="sxs-lookup"><span data-stu-id="45883-131">Do not use Delivery Optimization and use BITS instead</span></span>|



