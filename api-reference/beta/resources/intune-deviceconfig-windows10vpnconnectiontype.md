---
title: windows10VpnConnectionType 列挙型
description: VPN 接続の種類。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b3114c5d608cfed786fab8d2734d723682670ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395938"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="d6921-103">windows10VpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d6921-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="d6921-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6921-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d6921-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6921-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6921-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6921-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6921-107">VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="d6921-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="d6921-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6921-108">Members</span></span>
|<span data-ttu-id="d6921-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6921-109">Member</span></span>|<span data-ttu-id="d6921-110">値</span><span class="sxs-lookup"><span data-stu-id="d6921-110">Value</span></span>|<span data-ttu-id="d6921-111">説明</span><span class="sxs-lookup"><span data-stu-id="d6921-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6921-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="d6921-112">pulseSecure</span></span>|<span data-ttu-id="d6921-113">0</span><span class="sxs-lookup"><span data-stu-id="d6921-113">0</span></span>|<span data-ttu-id="d6921-114">パルスをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="d6921-114">Pulse Secure.</span></span>|
|<span data-ttu-id="d6921-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="d6921-115">f5EdgeClient</span></span>|<span data-ttu-id="d6921-116">1</span><span class="sxs-lookup"><span data-stu-id="d6921-116">1</span></span>|<span data-ttu-id="d6921-117">F5 キーを押してエッジのクライアントです。</span><span class="sxs-lookup"><span data-stu-id="d6921-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="d6921-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="d6921-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="d6921-119">2</span><span class="sxs-lookup"><span data-stu-id="d6921-119">2</span></span>|<span data-ttu-id="d6921-120">Dell SonicWALL モバイル接続します。</span><span class="sxs-lookup"><span data-stu-id="d6921-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="d6921-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="d6921-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="d6921-122">3</span><span class="sxs-lookup"><span data-stu-id="d6921-122">3</span></span>|<span data-ttu-id="d6921-123">ポイント カプセル VPN を確認してください。</span><span class="sxs-lookup"><span data-stu-id="d6921-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="d6921-124">自動</span><span class="sxs-lookup"><span data-stu-id="d6921-124">automatic</span></span>|<span data-ttu-id="d6921-125">4</span><span class="sxs-lookup"><span data-stu-id="d6921-125">4</span></span>|<span data-ttu-id="d6921-126">自動</span><span class="sxs-lookup"><span data-stu-id="d6921-126">Automatic.</span></span>|
|<span data-ttu-id="d6921-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="d6921-127">ikEv2</span></span>|<span data-ttu-id="d6921-128">5</span><span class="sxs-lookup"><span data-stu-id="d6921-128">5</span></span>|<span data-ttu-id="d6921-129">IKEv2。</span><span class="sxs-lookup"><span data-stu-id="d6921-129">IKEv2.</span></span>|
|<span data-ttu-id="d6921-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="d6921-130">l2tp</span></span>|<span data-ttu-id="d6921-131">6</span><span class="sxs-lookup"><span data-stu-id="d6921-131">6</span></span>|<span data-ttu-id="d6921-132">L2TP します。</span><span class="sxs-lookup"><span data-stu-id="d6921-132">L2TP.</span></span>|
|<span data-ttu-id="d6921-133">pptp</span><span class="sxs-lookup"><span data-stu-id="d6921-133">pptp</span></span>|<span data-ttu-id="d6921-134">7</span><span class="sxs-lookup"><span data-stu-id="d6921-134">7</span></span>|<span data-ttu-id="d6921-135">PPTP です。</span><span class="sxs-lookup"><span data-stu-id="d6921-135">PPTP.</span></span>|
|<span data-ttu-id="d6921-136">citrix</span><span class="sxs-lookup"><span data-stu-id="d6921-136">citrix</span></span>|<span data-ttu-id="d6921-137">8</span><span class="sxs-lookup"><span data-stu-id="d6921-137">8</span></span>|<span data-ttu-id="d6921-138">Citrix。</span><span class="sxs-lookup"><span data-stu-id="d6921-138">Citrix.</span></span>|
|<span data-ttu-id="d6921-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="d6921-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="d6921-140">9</span><span class="sxs-lookup"><span data-stu-id="d6921-140">9</span></span>|<span data-ttu-id="d6921-141">パロアルトの Alto ネットワーク GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="d6921-141">Palo Alto Networks GlobalProtect.</span></span>|




