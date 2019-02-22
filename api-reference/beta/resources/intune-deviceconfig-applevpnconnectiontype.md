---
title: りんご evpnconnectiontype 列挙型
description: Apple VPN 接続の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53ed413b05e29a10cebf151c718e55c75de702c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155602"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="7bf8e-103">りんご evpnconnectiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="7bf8e-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="7bf8e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bf8e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bf8e-106">Apple VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-106">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="7bf8e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7bf8e-107">Members</span></span>
|<span data-ttu-id="7bf8e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7bf8e-108">Member</span></span>|<span data-ttu-id="7bf8e-109">値</span><span class="sxs-lookup"><span data-stu-id="7bf8e-109">Value</span></span>|<span data-ttu-id="7bf8e-110">説明</span><span class="sxs-lookup"><span data-stu-id="7bf8e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bf8e-111">ciscoanyconnect</span><span class="sxs-lookup"><span data-stu-id="7bf8e-111">ciscoAnyConnect</span></span>|<span data-ttu-id="7bf8e-112">.0</span><span class="sxs-lookup"><span data-stu-id="7bf8e-112">0</span></span>|<span data-ttu-id="7bf8e-113">Cisco anyconnect。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-113">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="7bf8e-114">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="7bf8e-114">pulseSecure</span></span>|<span data-ttu-id="7bf8e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7bf8e-115">1</span></span>|<span data-ttu-id="7bf8e-116">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-116">Pulse Secure.</span></span>|
|<span data-ttu-id="7bf8e-117">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="7bf8e-117">f5EdgeClient</span></span>|<span data-ttu-id="7bf8e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7bf8e-118">2</span></span>|<span data-ttu-id="7bf8e-119">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-119">F5 Edge Client.</span></span>|
|<span data-ttu-id="7bf8e-120">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="7bf8e-120">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="7bf8e-121">1/3</span><span class="sxs-lookup"><span data-stu-id="7bf8e-121">3</span></span>|<span data-ttu-id="7bf8e-122">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-122">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="7bf8e-123">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="7bf8e-123">checkPointCapsuleVpn</span></span>|<span data-ttu-id="7bf8e-124">2/4</span><span class="sxs-lookup"><span data-stu-id="7bf8e-124">4</span></span>|<span data-ttu-id="7bf8e-125">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-125">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="7bf8e-126">customvpn</span><span class="sxs-lookup"><span data-stu-id="7bf8e-126">customVpn</span></span>|<span data-ttu-id="7bf8e-127">5</span><span class="sxs-lookup"><span data-stu-id="7bf8e-127">5</span></span>|<span data-ttu-id="7bf8e-128">カスタム VPN。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-128">Custom VPN.</span></span>|
|<span data-ttu-id="7bf8e-129">ciscoipsec</span><span class="sxs-lookup"><span data-stu-id="7bf8e-129">ciscoIPSec</span></span>|<span data-ttu-id="7bf8e-130">シックス</span><span class="sxs-lookup"><span data-stu-id="7bf8e-130">6</span></span>|<span data-ttu-id="7bf8e-131">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-131">Cisco (IPSec).</span></span>|
|<span data-ttu-id="7bf8e-132">社</span><span class="sxs-lookup"><span data-stu-id="7bf8e-132">citrix</span></span>|<span data-ttu-id="7bf8e-133">7</span><span class="sxs-lookup"><span data-stu-id="7bf8e-133">7</span></span>|<span data-ttu-id="7bf8e-134">社.</span><span class="sxs-lookup"><span data-stu-id="7bf8e-134">Citrix.</span></span>|
|<span data-ttu-id="7bf8e-135">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="7bf8e-135">ciscoAnyConnectV2</span></span>|<span data-ttu-id="7bf8e-136">~</span><span class="sxs-lookup"><span data-stu-id="7bf8e-136">8</span></span>|<span data-ttu-id="7bf8e-137">Cisco anyconnect V2。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-137">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="7bf8e-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="7bf8e-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="7bf8e-139">i-9</span><span class="sxs-lookup"><span data-stu-id="7bf8e-139">9</span></span>|<span data-ttu-id="7bf8e-140">Palo Alto Networks globalprotect。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-140">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="7bf8e-141">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="7bf8e-141">zscalerPrivateAccess</span></span>|<span data-ttu-id="7bf8e-142">個</span><span class="sxs-lookup"><span data-stu-id="7bf8e-142">10</span></span>|<span data-ttu-id="7bf8e-143">Zscaler プライベートアクセス。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-143">Zscaler Private Access.</span></span>|
|<span data-ttu-id="7bf8e-144">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="7bf8e-144">f5Access2018</span></span>|<span data-ttu-id="7bf8e-145">#</span><span class="sxs-lookup"><span data-stu-id="7bf8e-145">11</span></span>|<span data-ttu-id="7bf8e-146">F5 キーを押してアクセス2018。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-146">F5 Access 2018.</span></span>|
|<span data-ttu-id="7bf8e-147">citrixSso</span><span class="sxs-lookup"><span data-stu-id="7bf8e-147">citrixSso</span></span>|<span data-ttu-id="7bf8e-148">個</span><span class="sxs-lookup"><span data-stu-id="7bf8e-148">12</span></span>|<span data-ttu-id="7bf8e-149">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-149">Citrix Sso.</span></span>|
|<span data-ttu-id="7bf8e-150">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="7bf8e-150">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="7bf8e-151">スリー</span><span class="sxs-lookup"><span data-stu-id="7bf8e-151">13</span></span>|<span data-ttu-id="7bf8e-152">Palo Alto Networks globalprotect V2。</span><span class="sxs-lookup"><span data-stu-id="7bf8e-152">Palo Alto Networks GlobalProtect V2.</span></span>|




