---
title: appleVpnConnectionType 列挙型
description: Apple 社の VPN 接続の種類です。
ms.openlocfilehash: 5308fd8e5876db1d1a38248776c269ce5d80ad38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068245"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="04bce-103">appleVpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="04bce-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="04bce-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04bce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04bce-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04bce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04bce-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04bce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04bce-107">Apple 社の VPN 接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="04bce-107">Apple VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="04bce-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="04bce-108">Members</span></span>
|<span data-ttu-id="04bce-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="04bce-109">Member</span></span>|<span data-ttu-id="04bce-110">値</span><span class="sxs-lookup"><span data-stu-id="04bce-110">Value</span></span>|<span data-ttu-id="04bce-111">説明</span><span class="sxs-lookup"><span data-stu-id="04bce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04bce-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="04bce-112">ciscoAnyConnect</span></span>|<span data-ttu-id="04bce-113">0</span><span class="sxs-lookup"><span data-stu-id="04bce-113">0</span></span>|<span data-ttu-id="04bce-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="04bce-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="04bce-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="04bce-115">pulseSecure</span></span>|<span data-ttu-id="04bce-116">1</span><span class="sxs-lookup"><span data-stu-id="04bce-116">1</span></span>|<span data-ttu-id="04bce-117">パルスをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="04bce-117">Pulse Secure.</span></span>|
|<span data-ttu-id="04bce-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="04bce-118">f5EdgeClient</span></span>|<span data-ttu-id="04bce-119">2</span><span class="sxs-lookup"><span data-stu-id="04bce-119">2</span></span>|<span data-ttu-id="04bce-120">F5 キーを押してエッジのクライアントです。</span><span class="sxs-lookup"><span data-stu-id="04bce-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="04bce-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="04bce-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="04bce-122">3</span><span class="sxs-lookup"><span data-stu-id="04bce-122">3</span></span>|<span data-ttu-id="04bce-123">Dell SonicWALL モバイル接続します。</span><span class="sxs-lookup"><span data-stu-id="04bce-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="04bce-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="04bce-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="04bce-125">4</span><span class="sxs-lookup"><span data-stu-id="04bce-125">4</span></span>|<span data-ttu-id="04bce-126">ポイント カプセル VPN を確認してください。</span><span class="sxs-lookup"><span data-stu-id="04bce-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="04bce-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="04bce-127">customVpn</span></span>|<span data-ttu-id="04bce-128">5</span><span class="sxs-lookup"><span data-stu-id="04bce-128">5</span></span>|<span data-ttu-id="04bce-129">VPN のユーザーを設定します。</span><span class="sxs-lookup"><span data-stu-id="04bce-129">Custom VPN.</span></span>|
|<span data-ttu-id="04bce-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="04bce-130">ciscoIPSec</span></span>|<span data-ttu-id="04bce-131">6</span><span class="sxs-lookup"><span data-stu-id="04bce-131">6</span></span>|<span data-ttu-id="04bce-132">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="04bce-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="04bce-133">citrix</span><span class="sxs-lookup"><span data-stu-id="04bce-133">citrix</span></span>|<span data-ttu-id="04bce-134">7</span><span class="sxs-lookup"><span data-stu-id="04bce-134">7</span></span>|<span data-ttu-id="04bce-135">Citrix。</span><span class="sxs-lookup"><span data-stu-id="04bce-135">Citrix.</span></span>|
|<span data-ttu-id="04bce-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="04bce-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="04bce-137">8</span><span class="sxs-lookup"><span data-stu-id="04bce-137">8</span></span>|<span data-ttu-id="04bce-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="04bce-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="04bce-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="04bce-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="04bce-140">9</span><span class="sxs-lookup"><span data-stu-id="04bce-140">9</span></span>|<span data-ttu-id="04bce-141">パロアルトの Alto ネットワーク GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="04bce-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="04bce-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="04bce-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="04bce-143">10</span><span class="sxs-lookup"><span data-stu-id="04bce-143">10</span></span>|<span data-ttu-id="04bce-144">Zscaler プライベート アクセス。</span><span class="sxs-lookup"><span data-stu-id="04bce-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="04bce-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="04bce-145">f5Access2018</span></span>|<span data-ttu-id="04bce-146">11</span><span class="sxs-lookup"><span data-stu-id="04bce-146">11</span></span>|<span data-ttu-id="04bce-147">F5 キーを押してアクセス 2018。</span><span class="sxs-lookup"><span data-stu-id="04bce-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="04bce-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="04bce-148">citrixSso</span></span>|<span data-ttu-id="04bce-149">12</span><span class="sxs-lookup"><span data-stu-id="04bce-149">12</span></span>|<span data-ttu-id="04bce-150">Citrix Sso です。</span><span class="sxs-lookup"><span data-stu-id="04bce-150">Citrix Sso.</span></span>|
|<span data-ttu-id="04bce-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="04bce-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="04bce-152">13</span><span class="sxs-lookup"><span data-stu-id="04bce-152">13</span></span>|<span data-ttu-id="04bce-153">パロアルトでは、GlobalProtect V2 をネットワークします。</span><span class="sxs-lookup"><span data-stu-id="04bce-153">Palo Alto Networks GlobalProtect V2.</span></span>|





