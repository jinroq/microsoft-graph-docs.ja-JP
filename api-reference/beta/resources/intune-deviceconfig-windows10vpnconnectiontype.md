---
title: windows10VpnConnectionType 列挙型
description: VPN 接続の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5e0e3248315fc598d95ea3eb2bb46a6445a5968
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166711"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="ba750-103">windows10VpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ba750-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="ba750-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba750-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba750-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba750-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba750-106">VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="ba750-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="ba750-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ba750-107">Members</span></span>
|<span data-ttu-id="ba750-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ba750-108">Member</span></span>|<span data-ttu-id="ba750-109">値</span><span class="sxs-lookup"><span data-stu-id="ba750-109">Value</span></span>|<span data-ttu-id="ba750-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba750-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba750-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="ba750-111">pulseSecure</span></span>|<span data-ttu-id="ba750-112">.0</span><span class="sxs-lookup"><span data-stu-id="ba750-112">0</span></span>|<span data-ttu-id="ba750-113">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="ba750-113">Pulse Secure.</span></span>|
|<span data-ttu-id="ba750-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="ba750-114">f5EdgeClient</span></span>|<span data-ttu-id="ba750-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ba750-115">1</span></span>|<span data-ttu-id="ba750-116">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="ba750-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="ba750-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="ba750-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="ba750-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ba750-118">2</span></span>|<span data-ttu-id="ba750-119">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="ba750-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="ba750-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="ba750-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="ba750-121">1/3</span><span class="sxs-lookup"><span data-stu-id="ba750-121">3</span></span>|<span data-ttu-id="ba750-122">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="ba750-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ba750-123">自動</span><span class="sxs-lookup"><span data-stu-id="ba750-123">automatic</span></span>|<span data-ttu-id="ba750-124">2/4</span><span class="sxs-lookup"><span data-stu-id="ba750-124">4</span></span>|<span data-ttu-id="ba750-125">自動</span><span class="sxs-lookup"><span data-stu-id="ba750-125">Automatic.</span></span>|
|<span data-ttu-id="ba750-126">対する</span><span class="sxs-lookup"><span data-stu-id="ba750-126">ikEv2</span></span>|<span data-ttu-id="ba750-127">5</span><span class="sxs-lookup"><span data-stu-id="ba750-127">5</span></span>|<span data-ttu-id="ba750-128">対する.</span><span class="sxs-lookup"><span data-stu-id="ba750-128">IKEv2.</span></span>|
|<span data-ttu-id="ba750-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="ba750-129">l2tp</span></span>|<span data-ttu-id="ba750-130">シックス</span><span class="sxs-lookup"><span data-stu-id="ba750-130">6</span></span>|<span data-ttu-id="ba750-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="ba750-131">L2TP.</span></span>|
|<span data-ttu-id="ba750-132">pptp</span><span class="sxs-lookup"><span data-stu-id="ba750-132">pptp</span></span>|<span data-ttu-id="ba750-133">7</span><span class="sxs-lookup"><span data-stu-id="ba750-133">7</span></span>|<span data-ttu-id="ba750-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="ba750-134">PPTP.</span></span>|
|<span data-ttu-id="ba750-135">社</span><span class="sxs-lookup"><span data-stu-id="ba750-135">citrix</span></span>|<span data-ttu-id="ba750-136">~</span><span class="sxs-lookup"><span data-stu-id="ba750-136">8</span></span>|<span data-ttu-id="ba750-137">社.</span><span class="sxs-lookup"><span data-stu-id="ba750-137">Citrix.</span></span>|
|<span data-ttu-id="ba750-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="ba750-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="ba750-139">i-9</span><span class="sxs-lookup"><span data-stu-id="ba750-139">9</span></span>|<span data-ttu-id="ba750-140">Palo Alto Networks globalprotect。</span><span class="sxs-lookup"><span data-stu-id="ba750-140">Palo Alto Networks GlobalProtect.</span></span>|




