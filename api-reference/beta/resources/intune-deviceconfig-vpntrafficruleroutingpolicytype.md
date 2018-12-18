---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックの規則のルーティング ポリシーを指定します。
author: tfitzmac
ms.openlocfilehash: 5aa3f44f0e4ccf177154f97e9849093c52728b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343422"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="edf5e-103">vpnTrafficRuleRoutingPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="edf5e-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="edf5e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="edf5e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edf5e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="edf5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="edf5e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="edf5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edf5e-107">VPN トラフィックの規則のルーティング ポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="edf5e-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="edf5e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="edf5e-108">Members</span></span>
|<span data-ttu-id="edf5e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="edf5e-109">Member</span></span>|<span data-ttu-id="edf5e-110">値</span><span class="sxs-lookup"><span data-stu-id="edf5e-110">Value</span></span>|<span data-ttu-id="edf5e-111">説明</span><span class="sxs-lookup"><span data-stu-id="edf5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edf5e-112">none</span><span class="sxs-lookup"><span data-stu-id="edf5e-112">none</span></span>|<span data-ttu-id="edf5e-113">0</span><span class="sxs-lookup"><span data-stu-id="edf5e-113">0</span></span>|<span data-ttu-id="edf5e-114">ルーティング ポリシーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="edf5e-114">No routing policy specified.</span></span>|
|<span data-ttu-id="edf5e-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="edf5e-115">splitTunnel</span></span>|<span data-ttu-id="edf5e-116">1</span><span class="sxs-lookup"><span data-stu-id="edf5e-116">1</span></span>|<span data-ttu-id="edf5e-117">指定したアプリケーションのネットワーク トラフィックは、VPN を介してルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="edf5e-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="edf5e-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="edf5e-118">forceTunnel</span></span>|<span data-ttu-id="edf5e-119">2</span><span class="sxs-lookup"><span data-stu-id="edf5e-119">2</span></span>|<span data-ttu-id="edf5e-120">すべてのネットワーク トラフィックは、VPN を介してルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="edf5e-120">All network traffic will be routed through the VPN.</span></span>|





