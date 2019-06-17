---
title: りんご Evpnconnectiontype 列挙型
description: Apple VPN 接続の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f394f2d155ffb272b3b11f55eb8a09cafac63f26
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987657"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="4504d-103">りんご Evpnconnectiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="4504d-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="4504d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4504d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4504d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4504d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4504d-106">Apple VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="4504d-106">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="4504d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4504d-107">Members</span></span>
|<span data-ttu-id="4504d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4504d-108">Member</span></span>|<span data-ttu-id="4504d-109">値</span><span class="sxs-lookup"><span data-stu-id="4504d-109">Value</span></span>|<span data-ttu-id="4504d-110">説明</span><span class="sxs-lookup"><span data-stu-id="4504d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4504d-111">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="4504d-111">ciscoAnyConnect</span></span>|<span data-ttu-id="4504d-112">.0</span><span class="sxs-lookup"><span data-stu-id="4504d-112">0</span></span>|<span data-ttu-id="4504d-113">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="4504d-113">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="4504d-114">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="4504d-114">pulseSecure</span></span>|<span data-ttu-id="4504d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="4504d-115">1</span></span>|<span data-ttu-id="4504d-116">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="4504d-116">Pulse Secure.</span></span>|
|<span data-ttu-id="4504d-117">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="4504d-117">f5EdgeClient</span></span>|<span data-ttu-id="4504d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4504d-118">2</span></span>|<span data-ttu-id="4504d-119">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="4504d-119">F5 Edge Client.</span></span>|
|<span data-ttu-id="4504d-120">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="4504d-120">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="4504d-121">1/3</span><span class="sxs-lookup"><span data-stu-id="4504d-121">3</span></span>|<span data-ttu-id="4504d-122">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="4504d-122">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="4504d-123">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="4504d-123">checkPointCapsuleVpn</span></span>|<span data-ttu-id="4504d-124">2/4</span><span class="sxs-lookup"><span data-stu-id="4504d-124">4</span></span>|<span data-ttu-id="4504d-125">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="4504d-125">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="4504d-126">customVpn</span><span class="sxs-lookup"><span data-stu-id="4504d-126">customVpn</span></span>|<span data-ttu-id="4504d-127">5</span><span class="sxs-lookup"><span data-stu-id="4504d-127">5</span></span>|<span data-ttu-id="4504d-128">カスタム VPN。</span><span class="sxs-lookup"><span data-stu-id="4504d-128">Custom VPN.</span></span>|
|<span data-ttu-id="4504d-129">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="4504d-129">ciscoIPSec</span></span>|<span data-ttu-id="4504d-130">シックス</span><span class="sxs-lookup"><span data-stu-id="4504d-130">6</span></span>|<span data-ttu-id="4504d-131">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="4504d-131">Cisco (IPSec).</span></span>|
|<span data-ttu-id="4504d-132">社</span><span class="sxs-lookup"><span data-stu-id="4504d-132">citrix</span></span>|<span data-ttu-id="4504d-133">7</span><span class="sxs-lookup"><span data-stu-id="4504d-133">7</span></span>|<span data-ttu-id="4504d-134">社.</span><span class="sxs-lookup"><span data-stu-id="4504d-134">Citrix.</span></span>|
|<span data-ttu-id="4504d-135">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="4504d-135">ciscoAnyConnectV2</span></span>|<span data-ttu-id="4504d-136">8 </span><span class="sxs-lookup"><span data-stu-id="4504d-136">8</span></span>|<span data-ttu-id="4504d-137">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="4504d-137">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="4504d-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="4504d-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="4504d-139">9 </span><span class="sxs-lookup"><span data-stu-id="4504d-139">9</span></span>|<span data-ttu-id="4504d-140">Palo Alto Networks GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="4504d-140">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="4504d-141">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="4504d-141">zscalerPrivateAccess</span></span>|<span data-ttu-id="4504d-142">10 </span><span class="sxs-lookup"><span data-stu-id="4504d-142">10</span></span>|<span data-ttu-id="4504d-143">Zscaler プライベートアクセス。</span><span class="sxs-lookup"><span data-stu-id="4504d-143">Zscaler Private Access.</span></span>|
|<span data-ttu-id="4504d-144">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="4504d-144">f5Access2018</span></span>|<span data-ttu-id="4504d-145">#</span><span class="sxs-lookup"><span data-stu-id="4504d-145">11</span></span>|<span data-ttu-id="4504d-146">F5 キーを押してアクセス2018。</span><span class="sxs-lookup"><span data-stu-id="4504d-146">F5 Access 2018.</span></span>|
|<span data-ttu-id="4504d-147">citrixSso</span><span class="sxs-lookup"><span data-stu-id="4504d-147">citrixSso</span></span>|<span data-ttu-id="4504d-148">個</span><span class="sxs-lookup"><span data-stu-id="4504d-148">12</span></span>|<span data-ttu-id="4504d-149">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="4504d-149">Citrix Sso.</span></span>|
|<span data-ttu-id="4504d-150">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="4504d-150">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="4504d-151">スリー</span><span class="sxs-lookup"><span data-stu-id="4504d-151">13</span></span>|<span data-ttu-id="4504d-152">Palo Alto Networks GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="4504d-152">Palo Alto Networks GlobalProtect V2.</span></span>|
|<span data-ttu-id="4504d-153">対する</span><span class="sxs-lookup"><span data-stu-id="4504d-153">ikEv2</span></span>|<span data-ttu-id="4504d-154">第</span><span class="sxs-lookup"><span data-stu-id="4504d-154">14</span></span>|<span data-ttu-id="4504d-155">対する.</span><span class="sxs-lookup"><span data-stu-id="4504d-155">IKEv2.</span></span>|





