---
title: appleVpnConnectionType 列挙型
description: Apple 社の VPN 接続の種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f40281934aa241f245772e0bc4c5cd5bbbd0ec33
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415678"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="76a32-103">appleVpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="76a32-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="76a32-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76a32-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76a32-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76a32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76a32-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76a32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76a32-107">Apple 社の VPN 接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="76a32-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="76a32-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="76a32-108">Members</span></span>
|<span data-ttu-id="76a32-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="76a32-109">Member</span></span>|<span data-ttu-id="76a32-110">値</span><span class="sxs-lookup"><span data-stu-id="76a32-110">Value</span></span>|<span data-ttu-id="76a32-111">説明</span><span class="sxs-lookup"><span data-stu-id="76a32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76a32-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="76a32-112">ciscoAnyConnect</span></span>|<span data-ttu-id="76a32-113">0</span><span class="sxs-lookup"><span data-stu-id="76a32-113">0</span></span>|<span data-ttu-id="76a32-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="76a32-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="76a32-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="76a32-115">pulseSecure</span></span>|<span data-ttu-id="76a32-116">1</span><span class="sxs-lookup"><span data-stu-id="76a32-116">1</span></span>|<span data-ttu-id="76a32-117">パルスをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="76a32-117">Pulse Secure.</span></span>|
|<span data-ttu-id="76a32-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="76a32-118">f5EdgeClient</span></span>|<span data-ttu-id="76a32-119">2</span><span class="sxs-lookup"><span data-stu-id="76a32-119">2</span></span>|<span data-ttu-id="76a32-120">F5 キーを押してエッジのクライアントです。</span><span class="sxs-lookup"><span data-stu-id="76a32-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="76a32-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="76a32-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="76a32-122">3</span><span class="sxs-lookup"><span data-stu-id="76a32-122">3</span></span>|<span data-ttu-id="76a32-123">Dell SonicWALL モバイル接続します。</span><span class="sxs-lookup"><span data-stu-id="76a32-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="76a32-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="76a32-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="76a32-125">4</span><span class="sxs-lookup"><span data-stu-id="76a32-125">4</span></span>|<span data-ttu-id="76a32-126">ポイント カプセル VPN を確認してください。</span><span class="sxs-lookup"><span data-stu-id="76a32-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="76a32-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="76a32-127">customVpn</span></span>|<span data-ttu-id="76a32-128">5</span><span class="sxs-lookup"><span data-stu-id="76a32-128">5</span></span>|<span data-ttu-id="76a32-129">VPN のユーザーを設定します。</span><span class="sxs-lookup"><span data-stu-id="76a32-129">Custom VPN.</span></span>|
|<span data-ttu-id="76a32-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="76a32-130">ciscoIPSec</span></span>|<span data-ttu-id="76a32-131">6</span><span class="sxs-lookup"><span data-stu-id="76a32-131">6</span></span>|<span data-ttu-id="76a32-132">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="76a32-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="76a32-133">citrix</span><span class="sxs-lookup"><span data-stu-id="76a32-133">citrix</span></span>|<span data-ttu-id="76a32-134">7</span><span class="sxs-lookup"><span data-stu-id="76a32-134">7</span></span>|<span data-ttu-id="76a32-135">Citrix。</span><span class="sxs-lookup"><span data-stu-id="76a32-135">Citrix.</span></span>|
|<span data-ttu-id="76a32-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="76a32-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="76a32-137">8</span><span class="sxs-lookup"><span data-stu-id="76a32-137">8</span></span>|<span data-ttu-id="76a32-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="76a32-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="76a32-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="76a32-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="76a32-140">9</span><span class="sxs-lookup"><span data-stu-id="76a32-140">9</span></span>|<span data-ttu-id="76a32-141">パロアルトの Alto ネットワーク GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="76a32-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="76a32-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="76a32-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="76a32-143">10</span><span class="sxs-lookup"><span data-stu-id="76a32-143">10</span></span>|<span data-ttu-id="76a32-144">Zscaler プライベート アクセス。</span><span class="sxs-lookup"><span data-stu-id="76a32-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="76a32-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="76a32-145">f5Access2018</span></span>|<span data-ttu-id="76a32-146">11</span><span class="sxs-lookup"><span data-stu-id="76a32-146">11</span></span>|<span data-ttu-id="76a32-147">F5 キーを押してアクセス 2018。</span><span class="sxs-lookup"><span data-stu-id="76a32-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="76a32-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="76a32-148">citrixSso</span></span>|<span data-ttu-id="76a32-149">12</span><span class="sxs-lookup"><span data-stu-id="76a32-149">12</span></span>|<span data-ttu-id="76a32-150">Citrix Sso です。</span><span class="sxs-lookup"><span data-stu-id="76a32-150">Citrix Sso.</span></span>|
|<span data-ttu-id="76a32-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="76a32-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="76a32-152">13</span><span class="sxs-lookup"><span data-stu-id="76a32-152">13</span></span>|<span data-ttu-id="76a32-153">パロアルトでは、GlobalProtect V2 をネットワークします。</span><span class="sxs-lookup"><span data-stu-id="76a32-153">Palo Alto Networks GlobalProtect V2.</span></span>|




