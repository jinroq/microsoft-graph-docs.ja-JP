---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックの規則のルーティング ポリシーを指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c8ec4303dc16c7cb0606e4b9cf86594446f571e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974953"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="77757-103">vpnTrafficRuleRoutingPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="77757-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="77757-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77757-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77757-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77757-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77757-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="77757-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77757-107">VPN トラフィックの規則のルーティング ポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="77757-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="77757-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="77757-108">Members</span></span>
|<span data-ttu-id="77757-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="77757-109">Member</span></span>|<span data-ttu-id="77757-110">値</span><span class="sxs-lookup"><span data-stu-id="77757-110">Value</span></span>|<span data-ttu-id="77757-111">説明</span><span class="sxs-lookup"><span data-stu-id="77757-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77757-112">none</span><span class="sxs-lookup"><span data-stu-id="77757-112">none</span></span>|<span data-ttu-id="77757-113">0</span><span class="sxs-lookup"><span data-stu-id="77757-113">0</span></span>|<span data-ttu-id="77757-114">ルーティング ポリシーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="77757-114">No routing policy specified.</span></span>|
|<span data-ttu-id="77757-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="77757-115">splitTunnel</span></span>|<span data-ttu-id="77757-116">1</span><span class="sxs-lookup"><span data-stu-id="77757-116">1</span></span>|<span data-ttu-id="77757-117">指定したアプリケーションのネットワーク トラフィックは、VPN を介してルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="77757-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="77757-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="77757-118">forceTunnel</span></span>|<span data-ttu-id="77757-119">2</span><span class="sxs-lookup"><span data-stu-id="77757-119">2</span></span>|<span data-ttu-id="77757-120">すべてのネットワーク トラフィックは、VPN を介してルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="77757-120">All network traffic will be routed through the VPN.</span></span>|





