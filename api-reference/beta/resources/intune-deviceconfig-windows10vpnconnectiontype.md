---
title: windows10VpnConnectionType 列挙型
description: VPN 接続の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ac61b494fc261832a864c4c87998532a863f87b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774142"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="17c70-103">windows10VpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="17c70-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="17c70-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17c70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17c70-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="17c70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17c70-106">VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="17c70-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="17c70-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="17c70-107">Members</span></span>
|<span data-ttu-id="17c70-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="17c70-108">Member</span></span>|<span data-ttu-id="17c70-109">値</span><span class="sxs-lookup"><span data-stu-id="17c70-109">Value</span></span>|<span data-ttu-id="17c70-110">説明</span><span class="sxs-lookup"><span data-stu-id="17c70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17c70-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="17c70-111">pulseSecure</span></span>|<span data-ttu-id="17c70-112">.0</span><span class="sxs-lookup"><span data-stu-id="17c70-112">0</span></span>|<span data-ttu-id="17c70-113">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="17c70-113">Pulse Secure.</span></span>|
|<span data-ttu-id="17c70-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="17c70-114">f5EdgeClient</span></span>|<span data-ttu-id="17c70-115">1-d</span><span class="sxs-lookup"><span data-stu-id="17c70-115">1</span></span>|<span data-ttu-id="17c70-116">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="17c70-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="17c70-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="17c70-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="17c70-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="17c70-118">2</span></span>|<span data-ttu-id="17c70-119">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="17c70-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="17c70-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="17c70-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="17c70-121">1/3</span><span class="sxs-lookup"><span data-stu-id="17c70-121">3</span></span>|<span data-ttu-id="17c70-122">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="17c70-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="17c70-123">自動</span><span class="sxs-lookup"><span data-stu-id="17c70-123">automatic</span></span>|<span data-ttu-id="17c70-124">2/4</span><span class="sxs-lookup"><span data-stu-id="17c70-124">4</span></span>|<span data-ttu-id="17c70-125">自動</span><span class="sxs-lookup"><span data-stu-id="17c70-125">Automatic.</span></span>|
|<span data-ttu-id="17c70-126">対する</span><span class="sxs-lookup"><span data-stu-id="17c70-126">ikEv2</span></span>|<span data-ttu-id="17c70-127">5</span><span class="sxs-lookup"><span data-stu-id="17c70-127">5</span></span>|<span data-ttu-id="17c70-128">対する.</span><span class="sxs-lookup"><span data-stu-id="17c70-128">IKEv2.</span></span>|
|<span data-ttu-id="17c70-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="17c70-129">l2tp</span></span>|<span data-ttu-id="17c70-130">シックス</span><span class="sxs-lookup"><span data-stu-id="17c70-130">6</span></span>|<span data-ttu-id="17c70-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="17c70-131">L2TP.</span></span>|
|<span data-ttu-id="17c70-132">pptp</span><span class="sxs-lookup"><span data-stu-id="17c70-132">pptp</span></span>|<span data-ttu-id="17c70-133">7</span><span class="sxs-lookup"><span data-stu-id="17c70-133">7</span></span>|<span data-ttu-id="17c70-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="17c70-134">PPTP.</span></span>|
|<span data-ttu-id="17c70-135">社</span><span class="sxs-lookup"><span data-stu-id="17c70-135">citrix</span></span>|<span data-ttu-id="17c70-136">~</span><span class="sxs-lookup"><span data-stu-id="17c70-136">8</span></span>|<span data-ttu-id="17c70-137">社.</span><span class="sxs-lookup"><span data-stu-id="17c70-137">Citrix.</span></span>|
|<span data-ttu-id="17c70-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="17c70-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="17c70-139">i-9</span><span class="sxs-lookup"><span data-stu-id="17c70-139">9</span></span>|<span data-ttu-id="17c70-140">Palo Alto Networks globalprotect。</span><span class="sxs-lookup"><span data-stu-id="17c70-140">Palo Alto Networks GlobalProtect.</span></span>|





