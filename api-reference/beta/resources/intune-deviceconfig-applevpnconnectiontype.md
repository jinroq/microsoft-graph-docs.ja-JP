---
title: appleVpnConnectionType 列挙型
description: Apple 社の VPN 接続の種類です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94b39d6804a304cf84e6dbefa3ef715f837b55af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912695"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="6a770-103">appleVpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6a770-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="6a770-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a770-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a770-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a770-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a770-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a770-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a770-107">Apple 社の VPN 接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="6a770-107">Apple VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="6a770-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6a770-108">Members</span></span>
|<span data-ttu-id="6a770-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6a770-109">Member</span></span>|<span data-ttu-id="6a770-110">値</span><span class="sxs-lookup"><span data-stu-id="6a770-110">Value</span></span>|<span data-ttu-id="6a770-111">説明</span><span class="sxs-lookup"><span data-stu-id="6a770-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a770-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="6a770-112">ciscoAnyConnect</span></span>|<span data-ttu-id="6a770-113">0</span><span class="sxs-lookup"><span data-stu-id="6a770-113">0</span></span>|<span data-ttu-id="6a770-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="6a770-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="6a770-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="6a770-115">pulseSecure</span></span>|<span data-ttu-id="6a770-116">1</span><span class="sxs-lookup"><span data-stu-id="6a770-116">1</span></span>|<span data-ttu-id="6a770-117">パルスをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="6a770-117">Pulse Secure.</span></span>|
|<span data-ttu-id="6a770-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="6a770-118">f5EdgeClient</span></span>|<span data-ttu-id="6a770-119">2</span><span class="sxs-lookup"><span data-stu-id="6a770-119">2</span></span>|<span data-ttu-id="6a770-120">F5 キーを押してエッジのクライアントです。</span><span class="sxs-lookup"><span data-stu-id="6a770-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="6a770-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="6a770-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="6a770-122">3</span><span class="sxs-lookup"><span data-stu-id="6a770-122">3</span></span>|<span data-ttu-id="6a770-123">Dell SonicWALL モバイル接続します。</span><span class="sxs-lookup"><span data-stu-id="6a770-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="6a770-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="6a770-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="6a770-125">4</span><span class="sxs-lookup"><span data-stu-id="6a770-125">4</span></span>|<span data-ttu-id="6a770-126">ポイント カプセル VPN を確認してください。</span><span class="sxs-lookup"><span data-stu-id="6a770-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="6a770-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="6a770-127">customVpn</span></span>|<span data-ttu-id="6a770-128">5</span><span class="sxs-lookup"><span data-stu-id="6a770-128">5</span></span>|<span data-ttu-id="6a770-129">VPN のユーザーを設定します。</span><span class="sxs-lookup"><span data-stu-id="6a770-129">Custom VPN.</span></span>|
|<span data-ttu-id="6a770-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="6a770-130">ciscoIPSec</span></span>|<span data-ttu-id="6a770-131">6</span><span class="sxs-lookup"><span data-stu-id="6a770-131">6</span></span>|<span data-ttu-id="6a770-132">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="6a770-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="6a770-133">citrix</span><span class="sxs-lookup"><span data-stu-id="6a770-133">citrix</span></span>|<span data-ttu-id="6a770-134">7</span><span class="sxs-lookup"><span data-stu-id="6a770-134">7</span></span>|<span data-ttu-id="6a770-135">Citrix。</span><span class="sxs-lookup"><span data-stu-id="6a770-135">Citrix.</span></span>|
|<span data-ttu-id="6a770-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="6a770-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="6a770-137">8</span><span class="sxs-lookup"><span data-stu-id="6a770-137">8</span></span>|<span data-ttu-id="6a770-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="6a770-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="6a770-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="6a770-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="6a770-140">9</span><span class="sxs-lookup"><span data-stu-id="6a770-140">9</span></span>|<span data-ttu-id="6a770-141">パロアルトの Alto ネットワーク GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="6a770-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="6a770-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="6a770-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="6a770-143">10</span><span class="sxs-lookup"><span data-stu-id="6a770-143">10</span></span>|<span data-ttu-id="6a770-144">Zscaler プライベート アクセス。</span><span class="sxs-lookup"><span data-stu-id="6a770-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="6a770-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="6a770-145">f5Access2018</span></span>|<span data-ttu-id="6a770-146">11</span><span class="sxs-lookup"><span data-stu-id="6a770-146">11</span></span>|<span data-ttu-id="6a770-147">F5 キーを押してアクセス 2018。</span><span class="sxs-lookup"><span data-stu-id="6a770-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="6a770-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="6a770-148">citrixSso</span></span>|<span data-ttu-id="6a770-149">12</span><span class="sxs-lookup"><span data-stu-id="6a770-149">12</span></span>|<span data-ttu-id="6a770-150">Citrix Sso です。</span><span class="sxs-lookup"><span data-stu-id="6a770-150">Citrix Sso.</span></span>|
|<span data-ttu-id="6a770-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="6a770-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="6a770-152">13</span><span class="sxs-lookup"><span data-stu-id="6a770-152">13</span></span>|<span data-ttu-id="6a770-153">パロアルトでは、GlobalProtect V2 をネットワークします。</span><span class="sxs-lookup"><span data-stu-id="6a770-153">Palo Alto Networks GlobalProtect V2.</span></span>|





