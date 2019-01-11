---
title: windows10VpnConnectionType 列挙型
description: VPN 接続の種類。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4076ddcfbb0f391b2ade47dbea1e10113f0f6110
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855350"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="df903-103">windows10VpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="df903-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="df903-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df903-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df903-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df903-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df903-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="df903-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df903-107">VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="df903-107">VPN connection types.</span></span>
## <a name="members"></a><span data-ttu-id="df903-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="df903-108">Members</span></span>
|<span data-ttu-id="df903-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="df903-109">Member</span></span>|<span data-ttu-id="df903-110">値</span><span class="sxs-lookup"><span data-stu-id="df903-110">Value</span></span>|<span data-ttu-id="df903-111">説明</span><span class="sxs-lookup"><span data-stu-id="df903-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df903-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="df903-112">pulseSecure</span></span>|<span data-ttu-id="df903-113">0</span><span class="sxs-lookup"><span data-stu-id="df903-113">0</span></span>|<span data-ttu-id="df903-114">パルスをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="df903-114">Pulse Secure.</span></span>|
|<span data-ttu-id="df903-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="df903-115">f5EdgeClient</span></span>|<span data-ttu-id="df903-116">1</span><span class="sxs-lookup"><span data-stu-id="df903-116">1</span></span>|<span data-ttu-id="df903-117">F5 キーを押してエッジのクライアントです。</span><span class="sxs-lookup"><span data-stu-id="df903-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="df903-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="df903-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="df903-119">2</span><span class="sxs-lookup"><span data-stu-id="df903-119">2</span></span>|<span data-ttu-id="df903-120">Dell SonicWALL モバイル接続します。</span><span class="sxs-lookup"><span data-stu-id="df903-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="df903-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="df903-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="df903-122">3</span><span class="sxs-lookup"><span data-stu-id="df903-122">3</span></span>|<span data-ttu-id="df903-123">ポイント カプセル VPN を確認してください。</span><span class="sxs-lookup"><span data-stu-id="df903-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="df903-124">自動</span><span class="sxs-lookup"><span data-stu-id="df903-124">automatic</span></span>|<span data-ttu-id="df903-125">4</span><span class="sxs-lookup"><span data-stu-id="df903-125">4</span></span>|<span data-ttu-id="df903-126">自動</span><span class="sxs-lookup"><span data-stu-id="df903-126">Automatic.</span></span>|
|<span data-ttu-id="df903-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="df903-127">ikEv2</span></span>|<span data-ttu-id="df903-128">5</span><span class="sxs-lookup"><span data-stu-id="df903-128">5</span></span>|<span data-ttu-id="df903-129">IKEv2。</span><span class="sxs-lookup"><span data-stu-id="df903-129">IKEv2.</span></span>|
|<span data-ttu-id="df903-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="df903-130">l2tp</span></span>|<span data-ttu-id="df903-131">6</span><span class="sxs-lookup"><span data-stu-id="df903-131">6</span></span>|<span data-ttu-id="df903-132">L2TP します。</span><span class="sxs-lookup"><span data-stu-id="df903-132">L2TP.</span></span>|
|<span data-ttu-id="df903-133">pptp</span><span class="sxs-lookup"><span data-stu-id="df903-133">pptp</span></span>|<span data-ttu-id="df903-134">7</span><span class="sxs-lookup"><span data-stu-id="df903-134">7</span></span>|<span data-ttu-id="df903-135">PPTP です。</span><span class="sxs-lookup"><span data-stu-id="df903-135">PPTP.</span></span>|
|<span data-ttu-id="df903-136">citrix</span><span class="sxs-lookup"><span data-stu-id="df903-136">citrix</span></span>|<span data-ttu-id="df903-137">8</span><span class="sxs-lookup"><span data-stu-id="df903-137">8</span></span>|<span data-ttu-id="df903-138">Citrix。</span><span class="sxs-lookup"><span data-stu-id="df903-138">Citrix.</span></span>|
|<span data-ttu-id="df903-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="df903-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="df903-140">9</span><span class="sxs-lookup"><span data-stu-id="df903-140">9</span></span>|<span data-ttu-id="df903-141">パロアルトの Alto ネットワーク GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="df903-141">Palo Alto Networks GlobalProtect.</span></span>|





