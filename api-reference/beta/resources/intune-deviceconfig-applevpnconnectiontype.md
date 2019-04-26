---
title: りんご evpnconnectiontype 列挙型
description: Apple VPN 接続の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cbb3b3ba87a65d248da248bfe66abb426fdd764
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562322"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="f12b7-103">りんご evpnconnectiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="f12b7-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="f12b7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f12b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f12b7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f12b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f12b7-106">Apple VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="f12b7-106">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="f12b7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f12b7-107">Members</span></span>
|<span data-ttu-id="f12b7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f12b7-108">Member</span></span>|<span data-ttu-id="f12b7-109">値</span><span class="sxs-lookup"><span data-stu-id="f12b7-109">Value</span></span>|<span data-ttu-id="f12b7-110">説明</span><span class="sxs-lookup"><span data-stu-id="f12b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f12b7-111">ciscoanyconnect</span><span class="sxs-lookup"><span data-stu-id="f12b7-111">ciscoAnyConnect</span></span>|<span data-ttu-id="f12b7-112">.0</span><span class="sxs-lookup"><span data-stu-id="f12b7-112">0</span></span>|<span data-ttu-id="f12b7-113">Cisco anyconnect。</span><span class="sxs-lookup"><span data-stu-id="f12b7-113">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="f12b7-114">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="f12b7-114">pulseSecure</span></span>|<span data-ttu-id="f12b7-115">1 </span><span class="sxs-lookup"><span data-stu-id="f12b7-115">1</span></span>|<span data-ttu-id="f12b7-116">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="f12b7-116">Pulse Secure.</span></span>|
|<span data-ttu-id="f12b7-117">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="f12b7-117">f5EdgeClient</span></span>|<span data-ttu-id="f12b7-118">2 </span><span class="sxs-lookup"><span data-stu-id="f12b7-118">2</span></span>|<span data-ttu-id="f12b7-119">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="f12b7-119">F5 Edge Client.</span></span>|
|<span data-ttu-id="f12b7-120">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="f12b7-120">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="f12b7-121">3 </span><span class="sxs-lookup"><span data-stu-id="f12b7-121">3</span></span>|<span data-ttu-id="f12b7-122">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="f12b7-122">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="f12b7-123">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="f12b7-123">checkPointCapsuleVpn</span></span>|<span data-ttu-id="f12b7-124">4 </span><span class="sxs-lookup"><span data-stu-id="f12b7-124">4</span></span>|<span data-ttu-id="f12b7-125">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="f12b7-125">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="f12b7-126">customvpn</span><span class="sxs-lookup"><span data-stu-id="f12b7-126">customVpn</span></span>|<span data-ttu-id="f12b7-127">5 </span><span class="sxs-lookup"><span data-stu-id="f12b7-127">5</span></span>|<span data-ttu-id="f12b7-128">カスタム VPN。</span><span class="sxs-lookup"><span data-stu-id="f12b7-128">Custom VPN.</span></span>|
|<span data-ttu-id="f12b7-129">ciscoipsec</span><span class="sxs-lookup"><span data-stu-id="f12b7-129">ciscoIPSec</span></span>|<span data-ttu-id="f12b7-130">6 </span><span class="sxs-lookup"><span data-stu-id="f12b7-130">6</span></span>|<span data-ttu-id="f12b7-131">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="f12b7-131">Cisco (IPSec).</span></span>|
|<span data-ttu-id="f12b7-132">社</span><span class="sxs-lookup"><span data-stu-id="f12b7-132">citrix</span></span>|<span data-ttu-id="f12b7-133">7 </span><span class="sxs-lookup"><span data-stu-id="f12b7-133">7</span></span>|<span data-ttu-id="f12b7-134">社.</span><span class="sxs-lookup"><span data-stu-id="f12b7-134">Citrix.</span></span>|
|<span data-ttu-id="f12b7-135">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="f12b7-135">ciscoAnyConnectV2</span></span>|<span data-ttu-id="f12b7-136">8 </span><span class="sxs-lookup"><span data-stu-id="f12b7-136">8</span></span>|<span data-ttu-id="f12b7-137">Cisco anyconnect V2。</span><span class="sxs-lookup"><span data-stu-id="f12b7-137">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="f12b7-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="f12b7-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="f12b7-139">9 </span><span class="sxs-lookup"><span data-stu-id="f12b7-139">9</span></span>|<span data-ttu-id="f12b7-140">Palo Alto Networks globalprotect。</span><span class="sxs-lookup"><span data-stu-id="f12b7-140">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="f12b7-141">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="f12b7-141">zscalerPrivateAccess</span></span>|<span data-ttu-id="f12b7-142">10  </span><span class="sxs-lookup"><span data-stu-id="f12b7-142">10</span></span>|<span data-ttu-id="f12b7-143">Zscaler プライベートアクセス。</span><span class="sxs-lookup"><span data-stu-id="f12b7-143">Zscaler Private Access.</span></span>|
|<span data-ttu-id="f12b7-144">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="f12b7-144">f5Access2018</span></span>|<span data-ttu-id="f12b7-145">11 </span><span class="sxs-lookup"><span data-stu-id="f12b7-145">11</span></span>|<span data-ttu-id="f12b7-146">F5 キーを押してアクセス2018。</span><span class="sxs-lookup"><span data-stu-id="f12b7-146">F5 Access 2018.</span></span>|
|<span data-ttu-id="f12b7-147">citrixSso</span><span class="sxs-lookup"><span data-stu-id="f12b7-147">citrixSso</span></span>|<span data-ttu-id="f12b7-148">12 </span><span class="sxs-lookup"><span data-stu-id="f12b7-148">12</span></span>|<span data-ttu-id="f12b7-149">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="f12b7-149">Citrix Sso.</span></span>|
|<span data-ttu-id="f12b7-150">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="f12b7-150">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="f12b7-151">13 </span><span class="sxs-lookup"><span data-stu-id="f12b7-151">13</span></span>|<span data-ttu-id="f12b7-152">Palo Alto Networks globalprotect V2。</span><span class="sxs-lookup"><span data-stu-id="f12b7-152">Palo Alto Networks GlobalProtect V2.</span></span>|





