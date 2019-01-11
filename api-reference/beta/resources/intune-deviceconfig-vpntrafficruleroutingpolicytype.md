---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックの規則のルーティング ポリシーを指定します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b44a2b58cc42e9f3f88964d79473327f4ca2b74
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855322"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="c46a5-103">vpnTrafficRuleRoutingPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c46a5-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="c46a5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c46a5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c46a5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c46a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c46a5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c46a5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c46a5-107">VPN トラフィックの規則のルーティング ポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="c46a5-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="c46a5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c46a5-108">Members</span></span>
|<span data-ttu-id="c46a5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c46a5-109">Member</span></span>|<span data-ttu-id="c46a5-110">値</span><span class="sxs-lookup"><span data-stu-id="c46a5-110">Value</span></span>|<span data-ttu-id="c46a5-111">説明</span><span class="sxs-lookup"><span data-stu-id="c46a5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c46a5-112">none</span><span class="sxs-lookup"><span data-stu-id="c46a5-112">none</span></span>|<span data-ttu-id="c46a5-113">0</span><span class="sxs-lookup"><span data-stu-id="c46a5-113">0</span></span>|<span data-ttu-id="c46a5-114">ルーティング ポリシーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="c46a5-114">No routing policy specified.</span></span>|
|<span data-ttu-id="c46a5-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="c46a5-115">splitTunnel</span></span>|<span data-ttu-id="c46a5-116">1</span><span class="sxs-lookup"><span data-stu-id="c46a5-116">1</span></span>|<span data-ttu-id="c46a5-117">指定したアプリケーションのネットワーク トラフィックは、VPN を介してルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="c46a5-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="c46a5-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="c46a5-118">forceTunnel</span></span>|<span data-ttu-id="c46a5-119">2</span><span class="sxs-lookup"><span data-stu-id="c46a5-119">2</span></span>|<span data-ttu-id="c46a5-120">すべてのネットワーク トラフィックは、VPN を介してルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="c46a5-120">All network traffic will be routed through the VPN.</span></span>|





