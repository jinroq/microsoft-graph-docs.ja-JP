---
title: windows10VpnConnectionType 列挙型
description: VPN 接続の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ac61b494fc261832a864c4c87998532a863f87b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572032"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="9cea6-103">windows10VpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9cea6-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="9cea6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cea6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cea6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9cea6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cea6-106">VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="9cea6-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="9cea6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9cea6-107">Members</span></span>
|<span data-ttu-id="9cea6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9cea6-108">Member</span></span>|<span data-ttu-id="9cea6-109">値</span><span class="sxs-lookup"><span data-stu-id="9cea6-109">Value</span></span>|<span data-ttu-id="9cea6-110">説明</span><span class="sxs-lookup"><span data-stu-id="9cea6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cea6-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="9cea6-111">pulseSecure</span></span>|<span data-ttu-id="9cea6-112">.0</span><span class="sxs-lookup"><span data-stu-id="9cea6-112">0</span></span>|<span data-ttu-id="9cea6-113">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="9cea6-113">Pulse Secure.</span></span>|
|<span data-ttu-id="9cea6-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="9cea6-114">f5EdgeClient</span></span>|<span data-ttu-id="9cea6-115">1 </span><span class="sxs-lookup"><span data-stu-id="9cea6-115">1</span></span>|<span data-ttu-id="9cea6-116">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="9cea6-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="9cea6-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="9cea6-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="9cea6-118">2 </span><span class="sxs-lookup"><span data-stu-id="9cea6-118">2</span></span>|<span data-ttu-id="9cea6-119">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="9cea6-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="9cea6-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="9cea6-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="9cea6-121">3 </span><span class="sxs-lookup"><span data-stu-id="9cea6-121">3</span></span>|<span data-ttu-id="9cea6-122">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="9cea6-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="9cea6-123">自動</span><span class="sxs-lookup"><span data-stu-id="9cea6-123">automatic</span></span>|<span data-ttu-id="9cea6-124">4 </span><span class="sxs-lookup"><span data-stu-id="9cea6-124">4</span></span>|<span data-ttu-id="9cea6-125">自動</span><span class="sxs-lookup"><span data-stu-id="9cea6-125">Automatic.</span></span>|
|<span data-ttu-id="9cea6-126">対する</span><span class="sxs-lookup"><span data-stu-id="9cea6-126">ikEv2</span></span>|<span data-ttu-id="9cea6-127">5 </span><span class="sxs-lookup"><span data-stu-id="9cea6-127">5</span></span>|<span data-ttu-id="9cea6-128">対する.</span><span class="sxs-lookup"><span data-stu-id="9cea6-128">IKEv2.</span></span>|
|<span data-ttu-id="9cea6-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="9cea6-129">l2tp</span></span>|<span data-ttu-id="9cea6-130">6 </span><span class="sxs-lookup"><span data-stu-id="9cea6-130">6</span></span>|<span data-ttu-id="9cea6-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="9cea6-131">L2TP.</span></span>|
|<span data-ttu-id="9cea6-132">pptp</span><span class="sxs-lookup"><span data-stu-id="9cea6-132">pptp</span></span>|<span data-ttu-id="9cea6-133">7 </span><span class="sxs-lookup"><span data-stu-id="9cea6-133">7</span></span>|<span data-ttu-id="9cea6-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="9cea6-134">PPTP.</span></span>|
|<span data-ttu-id="9cea6-135">社</span><span class="sxs-lookup"><span data-stu-id="9cea6-135">citrix</span></span>|<span data-ttu-id="9cea6-136">8 </span><span class="sxs-lookup"><span data-stu-id="9cea6-136">8</span></span>|<span data-ttu-id="9cea6-137">社.</span><span class="sxs-lookup"><span data-stu-id="9cea6-137">Citrix.</span></span>|
|<span data-ttu-id="9cea6-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="9cea6-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="9cea6-139">9 </span><span class="sxs-lookup"><span data-stu-id="9cea6-139">9</span></span>|<span data-ttu-id="9cea6-140">Palo Alto Networks globalprotect。</span><span class="sxs-lookup"><span data-stu-id="9cea6-140">Palo Alto Networks GlobalProtect.</span></span>|





