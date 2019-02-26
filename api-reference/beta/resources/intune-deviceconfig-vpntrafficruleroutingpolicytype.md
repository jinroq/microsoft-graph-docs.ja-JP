---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックルールのルーティングポリシーを指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a7c6121b9adc47d116a7b3321ca150a8d42449a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157345"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="e9376-103">vpnTrafficRuleRoutingPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e9376-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="e9376-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9376-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9376-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9376-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9376-106">VPN トラフィックルールのルーティングポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9376-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="e9376-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e9376-107">Members</span></span>
|<span data-ttu-id="e9376-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e9376-108">Member</span></span>|<span data-ttu-id="e9376-109">値</span><span class="sxs-lookup"><span data-stu-id="e9376-109">Value</span></span>|<span data-ttu-id="e9376-110">説明</span><span class="sxs-lookup"><span data-stu-id="e9376-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9376-111">none</span><span class="sxs-lookup"><span data-stu-id="e9376-111">none</span></span>|<span data-ttu-id="e9376-112">.0</span><span class="sxs-lookup"><span data-stu-id="e9376-112">0</span></span>|<span data-ttu-id="e9376-113">ルーティングポリシーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="e9376-113">No routing policy specified.</span></span>|
|<span data-ttu-id="e9376-114">splittunnel</span><span class="sxs-lookup"><span data-stu-id="e9376-114">splitTunnel</span></span>|<span data-ttu-id="e9376-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e9376-115">1</span></span>|<span data-ttu-id="e9376-116">指定したアプリのネットワークトラフィックは、VPN 経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="e9376-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="e9376-117">forcetunnel</span><span class="sxs-lookup"><span data-stu-id="e9376-117">forceTunnel</span></span>|<span data-ttu-id="e9376-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e9376-118">2</span></span>|<span data-ttu-id="e9376-119">すべてのネットワークトラフィックは、VPN 経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="e9376-119">All network traffic will be routed through the VPN.</span></span>|




