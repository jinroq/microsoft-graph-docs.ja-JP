---
title: androidWorkProfileVpnConnectionType 列挙型
description: Android の作業プロファイルの VPN 接続の種類です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecef95a2426890573b2317f665d155b82a1a3b11
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983192"
---
# <a name="androidworkprofilevpnconnectiontype-enum-type"></a><span data-ttu-id="15ea6-103">androidWorkProfileVpnConnectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="15ea6-103">androidWorkProfileVpnConnectionType enum type</span></span>

> <span data-ttu-id="15ea6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15ea6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15ea6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15ea6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15ea6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15ea6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15ea6-107">Android の作業プロファイルの VPN 接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="15ea6-107">Android Work Profile VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="15ea6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="15ea6-108">Members</span></span>
|<span data-ttu-id="15ea6-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="15ea6-109">Member</span></span>|<span data-ttu-id="15ea6-110">値</span><span class="sxs-lookup"><span data-stu-id="15ea6-110">Value</span></span>|<span data-ttu-id="15ea6-111">説明</span><span class="sxs-lookup"><span data-stu-id="15ea6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ea6-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="15ea6-112">ciscoAnyConnect</span></span>|<span data-ttu-id="15ea6-113">0</span><span class="sxs-lookup"><span data-stu-id="15ea6-113">0</span></span>|<span data-ttu-id="15ea6-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="15ea6-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="15ea6-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="15ea6-115">pulseSecure</span></span>|<span data-ttu-id="15ea6-116">1</span><span class="sxs-lookup"><span data-stu-id="15ea6-116">1</span></span>|<span data-ttu-id="15ea6-117">パルスをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="15ea6-117">Pulse Secure.</span></span>|
|<span data-ttu-id="15ea6-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="15ea6-118">f5EdgeClient</span></span>|<span data-ttu-id="15ea6-119">2</span><span class="sxs-lookup"><span data-stu-id="15ea6-119">2</span></span>|<span data-ttu-id="15ea6-120">F5 キーを押してエッジのクライアントです。</span><span class="sxs-lookup"><span data-stu-id="15ea6-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="15ea6-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="15ea6-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="15ea6-122">3</span><span class="sxs-lookup"><span data-stu-id="15ea6-122">3</span></span>|<span data-ttu-id="15ea6-123">Dell SonicWALL モバイル接続します。</span><span class="sxs-lookup"><span data-stu-id="15ea6-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="15ea6-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="15ea6-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="15ea6-125">4</span><span class="sxs-lookup"><span data-stu-id="15ea6-125">4</span></span>|<span data-ttu-id="15ea6-126">ポイント カプセル VPN を確認してください。</span><span class="sxs-lookup"><span data-stu-id="15ea6-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="15ea6-127">citrix</span><span class="sxs-lookup"><span data-stu-id="15ea6-127">citrix</span></span>|<span data-ttu-id="15ea6-128">5</span><span class="sxs-lookup"><span data-stu-id="15ea6-128">5</span></span>|<span data-ttu-id="15ea6-129">Citrix</span><span class="sxs-lookup"><span data-stu-id="15ea6-129">Citrix</span></span>|
|<span data-ttu-id="15ea6-130">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="15ea6-130">paloAltoGlobalProtect</span></span>|<span data-ttu-id="15ea6-131">6</span><span class="sxs-lookup"><span data-stu-id="15ea6-131">6</span></span>|<span data-ttu-id="15ea6-132">パロアルトの Alto ネットワーク GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="15ea6-132">Palo Alto Networks GlobalProtect.</span></span>|





