---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックの規則のルーティング ポリシーを指定します。
ms.openlocfilehash: df51851ef0820f5982a6689421503364e9064c78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069238"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="5ff4f-103">vpnTrafficRuleRoutingPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5ff4f-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="5ff4f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ff4f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ff4f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ff4f-107">VPN トラフィックの規則のルーティング ポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="5ff4f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ff4f-108">Members</span></span>
|<span data-ttu-id="5ff4f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ff4f-109">Member</span></span>|<span data-ttu-id="5ff4f-110">値</span><span class="sxs-lookup"><span data-stu-id="5ff4f-110">Value</span></span>|<span data-ttu-id="5ff4f-111">説明</span><span class="sxs-lookup"><span data-stu-id="5ff4f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ff4f-112">none</span><span class="sxs-lookup"><span data-stu-id="5ff4f-112">none</span></span>|<span data-ttu-id="5ff4f-113">0</span><span class="sxs-lookup"><span data-stu-id="5ff4f-113">0</span></span>|<span data-ttu-id="5ff4f-114">ルーティング ポリシーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-114">No routing policy specified.</span></span>|
|<span data-ttu-id="5ff4f-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="5ff4f-115">splitTunnel</span></span>|<span data-ttu-id="5ff4f-116">1</span><span class="sxs-lookup"><span data-stu-id="5ff4f-116">1</span></span>|<span data-ttu-id="5ff4f-117">指定したアプリケーションのネットワーク トラフィックは、VPN を介してルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="5ff4f-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="5ff4f-118">forceTunnel</span></span>|<span data-ttu-id="5ff4f-119">2</span><span class="sxs-lookup"><span data-stu-id="5ff4f-119">2</span></span>|<span data-ttu-id="5ff4f-120">すべてのネットワーク トラフィックは、VPN を介してルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-120">All network traffic will be routed through the VPN.</span></span>|





