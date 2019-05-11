---
title: りんご Evpnconnectiontype 列挙型
description: Apple VPN 接続の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a1e6303f43abdd0ffbef8038022c3647d7211d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947772"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="5cf76-103">りんご Evpnconnectiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="5cf76-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="5cf76-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cf76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cf76-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5cf76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cf76-106">Apple VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="5cf76-106">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="5cf76-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5cf76-107">Members</span></span>
|<span data-ttu-id="5cf76-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5cf76-108">Member</span></span>|<span data-ttu-id="5cf76-109">値</span><span class="sxs-lookup"><span data-stu-id="5cf76-109">Value</span></span>|<span data-ttu-id="5cf76-110">説明</span><span class="sxs-lookup"><span data-stu-id="5cf76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cf76-111">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="5cf76-111">ciscoAnyConnect</span></span>|<span data-ttu-id="5cf76-112">.0</span><span class="sxs-lookup"><span data-stu-id="5cf76-112">0</span></span>|<span data-ttu-id="5cf76-113">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="5cf76-113">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="5cf76-114">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="5cf76-114">pulseSecure</span></span>|<span data-ttu-id="5cf76-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5cf76-115">1</span></span>|<span data-ttu-id="5cf76-116">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="5cf76-116">Pulse Secure.</span></span>|
|<span data-ttu-id="5cf76-117">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="5cf76-117">f5EdgeClient</span></span>|<span data-ttu-id="5cf76-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5cf76-118">2</span></span>|<span data-ttu-id="5cf76-119">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="5cf76-119">F5 Edge Client.</span></span>|
|<span data-ttu-id="5cf76-120">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="5cf76-120">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="5cf76-121">1/3</span><span class="sxs-lookup"><span data-stu-id="5cf76-121">3</span></span>|<span data-ttu-id="5cf76-122">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="5cf76-122">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="5cf76-123">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="5cf76-123">checkPointCapsuleVpn</span></span>|<span data-ttu-id="5cf76-124">2/4</span><span class="sxs-lookup"><span data-stu-id="5cf76-124">4</span></span>|<span data-ttu-id="5cf76-125">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="5cf76-125">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="5cf76-126">customVpn</span><span class="sxs-lookup"><span data-stu-id="5cf76-126">customVpn</span></span>|<span data-ttu-id="5cf76-127">5</span><span class="sxs-lookup"><span data-stu-id="5cf76-127">5</span></span>|<span data-ttu-id="5cf76-128">カスタム VPN。</span><span class="sxs-lookup"><span data-stu-id="5cf76-128">Custom VPN.</span></span>|
|<span data-ttu-id="5cf76-129">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="5cf76-129">ciscoIPSec</span></span>|<span data-ttu-id="5cf76-130">シックス</span><span class="sxs-lookup"><span data-stu-id="5cf76-130">6</span></span>|<span data-ttu-id="5cf76-131">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="5cf76-131">Cisco (IPSec).</span></span>|
|<span data-ttu-id="5cf76-132">社</span><span class="sxs-lookup"><span data-stu-id="5cf76-132">citrix</span></span>|<span data-ttu-id="5cf76-133">7</span><span class="sxs-lookup"><span data-stu-id="5cf76-133">7</span></span>|<span data-ttu-id="5cf76-134">社.</span><span class="sxs-lookup"><span data-stu-id="5cf76-134">Citrix.</span></span>|
|<span data-ttu-id="5cf76-135">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="5cf76-135">ciscoAnyConnectV2</span></span>|<span data-ttu-id="5cf76-136">8 </span><span class="sxs-lookup"><span data-stu-id="5cf76-136">8</span></span>|<span data-ttu-id="5cf76-137">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="5cf76-137">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="5cf76-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="5cf76-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="5cf76-139">9 </span><span class="sxs-lookup"><span data-stu-id="5cf76-139">9</span></span>|<span data-ttu-id="5cf76-140">Palo Alto Networks GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="5cf76-140">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="5cf76-141">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="5cf76-141">zscalerPrivateAccess</span></span>|<span data-ttu-id="5cf76-142">10 </span><span class="sxs-lookup"><span data-stu-id="5cf76-142">10</span></span>|<span data-ttu-id="5cf76-143">Zscaler プライベートアクセス。</span><span class="sxs-lookup"><span data-stu-id="5cf76-143">Zscaler Private Access.</span></span>|
|<span data-ttu-id="5cf76-144">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="5cf76-144">f5Access2018</span></span>|<span data-ttu-id="5cf76-145">#</span><span class="sxs-lookup"><span data-stu-id="5cf76-145">11</span></span>|<span data-ttu-id="5cf76-146">F5 キーを押してアクセス2018。</span><span class="sxs-lookup"><span data-stu-id="5cf76-146">F5 Access 2018.</span></span>|
|<span data-ttu-id="5cf76-147">citrixSso</span><span class="sxs-lookup"><span data-stu-id="5cf76-147">citrixSso</span></span>|<span data-ttu-id="5cf76-148">個</span><span class="sxs-lookup"><span data-stu-id="5cf76-148">12</span></span>|<span data-ttu-id="5cf76-149">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="5cf76-149">Citrix Sso.</span></span>|
|<span data-ttu-id="5cf76-150">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="5cf76-150">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="5cf76-151">スリー</span><span class="sxs-lookup"><span data-stu-id="5cf76-151">13</span></span>|<span data-ttu-id="5cf76-152">Palo Alto Networks GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="5cf76-152">Palo Alto Networks GlobalProtect V2.</span></span>|




