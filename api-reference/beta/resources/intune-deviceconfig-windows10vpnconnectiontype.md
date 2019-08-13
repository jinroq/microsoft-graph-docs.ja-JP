---
title: windows10VpnConnectionType 列挙型
description: VPN 接続の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f16b905161a88b8e07f8f2d3b3f343ac2d693bef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369697"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="b44f1-103">windows10VpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b44f1-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="b44f1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b44f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b44f1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b44f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b44f1-106">VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="b44f1-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="b44f1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b44f1-107">Members</span></span>
|<span data-ttu-id="b44f1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b44f1-108">Member</span></span>|<span data-ttu-id="b44f1-109">値</span><span class="sxs-lookup"><span data-stu-id="b44f1-109">Value</span></span>|<span data-ttu-id="b44f1-110">説明</span><span class="sxs-lookup"><span data-stu-id="b44f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b44f1-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="b44f1-111">pulseSecure</span></span>|<span data-ttu-id="b44f1-112">.0</span><span class="sxs-lookup"><span data-stu-id="b44f1-112">0</span></span>|<span data-ttu-id="b44f1-113">パルスがセキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="b44f1-113">Pulse Secure.</span></span>|
|<span data-ttu-id="b44f1-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="b44f1-114">f5EdgeClient</span></span>|<span data-ttu-id="b44f1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="b44f1-115">1</span></span>|<span data-ttu-id="b44f1-116">F5 キーを押したエッジクライアント。</span><span class="sxs-lookup"><span data-stu-id="b44f1-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="b44f1-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="b44f1-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="b44f1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b44f1-118">2</span></span>|<span data-ttu-id="b44f1-119">Dell SonicWALL モバイル接続。</span><span class="sxs-lookup"><span data-stu-id="b44f1-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="b44f1-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="b44f1-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="b44f1-121">1/3</span><span class="sxs-lookup"><span data-stu-id="b44f1-121">3</span></span>|<span data-ttu-id="b44f1-122">[カプセル接続] VPN をチェックします。</span><span class="sxs-lookup"><span data-stu-id="b44f1-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="b44f1-123">自動</span><span class="sxs-lookup"><span data-stu-id="b44f1-123">automatic</span></span>|<span data-ttu-id="b44f1-124">2/4</span><span class="sxs-lookup"><span data-stu-id="b44f1-124">4</span></span>|<span data-ttu-id="b44f1-125">自動</span><span class="sxs-lookup"><span data-stu-id="b44f1-125">Automatic.</span></span>|
|<span data-ttu-id="b44f1-126">対する</span><span class="sxs-lookup"><span data-stu-id="b44f1-126">ikEv2</span></span>|<span data-ttu-id="b44f1-127">5</span><span class="sxs-lookup"><span data-stu-id="b44f1-127">5</span></span>|<span data-ttu-id="b44f1-128">対する.</span><span class="sxs-lookup"><span data-stu-id="b44f1-128">IKEv2.</span></span>|
|<span data-ttu-id="b44f1-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="b44f1-129">l2tp</span></span>|<span data-ttu-id="b44f1-130">シックス</span><span class="sxs-lookup"><span data-stu-id="b44f1-130">6</span></span>|<span data-ttu-id="b44f1-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="b44f1-131">L2TP.</span></span>|
|<span data-ttu-id="b44f1-132">pptp</span><span class="sxs-lookup"><span data-stu-id="b44f1-132">pptp</span></span>|<span data-ttu-id="b44f1-133">7</span><span class="sxs-lookup"><span data-stu-id="b44f1-133">7</span></span>|<span data-ttu-id="b44f1-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="b44f1-134">PPTP.</span></span>|
|<span data-ttu-id="b44f1-135">社</span><span class="sxs-lookup"><span data-stu-id="b44f1-135">citrix</span></span>|<span data-ttu-id="b44f1-136">8 </span><span class="sxs-lookup"><span data-stu-id="b44f1-136">8</span></span>|<span data-ttu-id="b44f1-137">社.</span><span class="sxs-lookup"><span data-stu-id="b44f1-137">Citrix.</span></span>|
|<span data-ttu-id="b44f1-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="b44f1-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="b44f1-139">9 </span><span class="sxs-lookup"><span data-stu-id="b44f1-139">9</span></span>|<span data-ttu-id="b44f1-140">Palo Alto Networks GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="b44f1-140">Palo Alto Networks GlobalProtect.</span></span>|



