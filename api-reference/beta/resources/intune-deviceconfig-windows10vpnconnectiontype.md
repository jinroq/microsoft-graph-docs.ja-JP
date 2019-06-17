---
title: windows10VpnConnectionType 列挙型
description: VPN 接続の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c44c2a6e9f576f6ba77c0e4b4954019ade655bc5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982106"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="9b53e-103">windows10VpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9b53e-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="9b53e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b53e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b53e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b53e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b53e-106">VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="9b53e-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="9b53e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9b53e-107">Members</span></span>
|<span data-ttu-id="9b53e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9b53e-108">Member</span></span>|<span data-ttu-id="9b53e-109">値</span><span class="sxs-lookup"><span data-stu-id="9b53e-109">Value</span></span>|<span data-ttu-id="9b53e-110">説明</span><span class="sxs-lookup"><span data-stu-id="9b53e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b53e-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="9b53e-111">pulseSecure</span></span>|<span data-ttu-id="9b53e-112">.0</span><span class="sxs-lookup"><span data-stu-id="9b53e-112">0</span></span>|<span data-ttu-id="9b53e-113">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="9b53e-113">Pulse Secure.</span></span>|
|<span data-ttu-id="9b53e-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="9b53e-114">f5EdgeClient</span></span>|<span data-ttu-id="9b53e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9b53e-115">1</span></span>|<span data-ttu-id="9b53e-116">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="9b53e-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="9b53e-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="9b53e-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="9b53e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9b53e-118">2</span></span>|<span data-ttu-id="9b53e-119">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="9b53e-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="9b53e-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="9b53e-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="9b53e-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9b53e-121">3</span></span>|<span data-ttu-id="9b53e-122">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="9b53e-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="9b53e-123">自動</span><span class="sxs-lookup"><span data-stu-id="9b53e-123">automatic</span></span>|<span data-ttu-id="9b53e-124">2/4</span><span class="sxs-lookup"><span data-stu-id="9b53e-124">4</span></span>|<span data-ttu-id="9b53e-125">自動</span><span class="sxs-lookup"><span data-stu-id="9b53e-125">Automatic.</span></span>|
|<span data-ttu-id="9b53e-126">対する</span><span class="sxs-lookup"><span data-stu-id="9b53e-126">ikEv2</span></span>|<span data-ttu-id="9b53e-127">5</span><span class="sxs-lookup"><span data-stu-id="9b53e-127">5</span></span>|<span data-ttu-id="9b53e-128">対する.</span><span class="sxs-lookup"><span data-stu-id="9b53e-128">IKEv2.</span></span>|
|<span data-ttu-id="9b53e-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="9b53e-129">l2tp</span></span>|<span data-ttu-id="9b53e-130">シックス</span><span class="sxs-lookup"><span data-stu-id="9b53e-130">6</span></span>|<span data-ttu-id="9b53e-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="9b53e-131">L2TP.</span></span>|
|<span data-ttu-id="9b53e-132">pptp</span><span class="sxs-lookup"><span data-stu-id="9b53e-132">pptp</span></span>|<span data-ttu-id="9b53e-133">7</span><span class="sxs-lookup"><span data-stu-id="9b53e-133">7</span></span>|<span data-ttu-id="9b53e-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="9b53e-134">PPTP.</span></span>|
|<span data-ttu-id="9b53e-135">社</span><span class="sxs-lookup"><span data-stu-id="9b53e-135">citrix</span></span>|<span data-ttu-id="9b53e-136">8 </span><span class="sxs-lookup"><span data-stu-id="9b53e-136">8</span></span>|<span data-ttu-id="9b53e-137">社.</span><span class="sxs-lookup"><span data-stu-id="9b53e-137">Citrix.</span></span>|
|<span data-ttu-id="9b53e-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="9b53e-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="9b53e-139">9 </span><span class="sxs-lookup"><span data-stu-id="9b53e-139">9</span></span>|<span data-ttu-id="9b53e-140">Palo Alto Networks GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="9b53e-140">Palo Alto Networks GlobalProtect.</span></span>|





