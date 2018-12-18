---
title: appleVpnConnectionType 列挙型
description: Apple 社の VPN 接続の種類です。
author: tfitzmac
ms.openlocfilehash: 0904dbff2c9d30b362e3a024f4ff57fbd0769bb3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348560"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="c3f7f-103">appleVpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c3f7f-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="c3f7f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3f7f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3f7f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3f7f-107">Apple 社の VPN 接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-107">Apple VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="c3f7f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c3f7f-108">Members</span></span>
|<span data-ttu-id="c3f7f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c3f7f-109">Member</span></span>|<span data-ttu-id="c3f7f-110">値</span><span class="sxs-lookup"><span data-stu-id="c3f7f-110">Value</span></span>|<span data-ttu-id="c3f7f-111">説明</span><span class="sxs-lookup"><span data-stu-id="c3f7f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3f7f-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="c3f7f-112">ciscoAnyConnect</span></span>|<span data-ttu-id="c3f7f-113">0</span><span class="sxs-lookup"><span data-stu-id="c3f7f-113">0</span></span>|<span data-ttu-id="c3f7f-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="c3f7f-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="c3f7f-115">pulseSecure</span></span>|<span data-ttu-id="c3f7f-116">1</span><span class="sxs-lookup"><span data-stu-id="c3f7f-116">1</span></span>|<span data-ttu-id="c3f7f-117">パルスをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-117">Pulse Secure.</span></span>|
|<span data-ttu-id="c3f7f-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="c3f7f-118">f5EdgeClient</span></span>|<span data-ttu-id="c3f7f-119">2</span><span class="sxs-lookup"><span data-stu-id="c3f7f-119">2</span></span>|<span data-ttu-id="c3f7f-120">F5 キーを押してエッジのクライアントです。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="c3f7f-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="c3f7f-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="c3f7f-122">3</span><span class="sxs-lookup"><span data-stu-id="c3f7f-122">3</span></span>|<span data-ttu-id="c3f7f-123">Dell SonicWALL モバイル接続します。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="c3f7f-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="c3f7f-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="c3f7f-125">4</span><span class="sxs-lookup"><span data-stu-id="c3f7f-125">4</span></span>|<span data-ttu-id="c3f7f-126">ポイント カプセル VPN を確認してください。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="c3f7f-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="c3f7f-127">customVpn</span></span>|<span data-ttu-id="c3f7f-128">5</span><span class="sxs-lookup"><span data-stu-id="c3f7f-128">5</span></span>|<span data-ttu-id="c3f7f-129">VPN のユーザーを設定します。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-129">Custom VPN.</span></span>|
|<span data-ttu-id="c3f7f-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="c3f7f-130">ciscoIPSec</span></span>|<span data-ttu-id="c3f7f-131">6</span><span class="sxs-lookup"><span data-stu-id="c3f7f-131">6</span></span>|<span data-ttu-id="c3f7f-132">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="c3f7f-133">citrix</span><span class="sxs-lookup"><span data-stu-id="c3f7f-133">citrix</span></span>|<span data-ttu-id="c3f7f-134">7</span><span class="sxs-lookup"><span data-stu-id="c3f7f-134">7</span></span>|<span data-ttu-id="c3f7f-135">Citrix。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-135">Citrix.</span></span>|
|<span data-ttu-id="c3f7f-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="c3f7f-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="c3f7f-137">8</span><span class="sxs-lookup"><span data-stu-id="c3f7f-137">8</span></span>|<span data-ttu-id="c3f7f-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="c3f7f-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="c3f7f-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="c3f7f-140">9</span><span class="sxs-lookup"><span data-stu-id="c3f7f-140">9</span></span>|<span data-ttu-id="c3f7f-141">パロアルトの Alto ネットワーク GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="c3f7f-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="c3f7f-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="c3f7f-143">10</span><span class="sxs-lookup"><span data-stu-id="c3f7f-143">10</span></span>|<span data-ttu-id="c3f7f-144">Zscaler プライベート アクセス。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="c3f7f-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="c3f7f-145">f5Access2018</span></span>|<span data-ttu-id="c3f7f-146">11</span><span class="sxs-lookup"><span data-stu-id="c3f7f-146">11</span></span>|<span data-ttu-id="c3f7f-147">F5 キーを押してアクセス 2018。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="c3f7f-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="c3f7f-148">citrixSso</span></span>|<span data-ttu-id="c3f7f-149">12</span><span class="sxs-lookup"><span data-stu-id="c3f7f-149">12</span></span>|<span data-ttu-id="c3f7f-150">Citrix Sso です。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-150">Citrix Sso.</span></span>|
|<span data-ttu-id="c3f7f-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="c3f7f-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="c3f7f-152">13</span><span class="sxs-lookup"><span data-stu-id="c3f7f-152">13</span></span>|<span data-ttu-id="c3f7f-153">パロアルトでは、GlobalProtect V2 をネットワークします。</span><span class="sxs-lookup"><span data-stu-id="c3f7f-153">Palo Alto Networks GlobalProtect V2.</span></span>|





