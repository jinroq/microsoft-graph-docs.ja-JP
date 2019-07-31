---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックルールのルーティングポリシーを指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5cbbba22017a40ae2f7db41e25f497c09156a2f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969374"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="dd002-103">vpnTrafficRuleRoutingPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="dd002-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="dd002-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd002-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd002-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dd002-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd002-106">VPN トラフィックルールのルーティングポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="dd002-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="dd002-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="dd002-107">Members</span></span>
|<span data-ttu-id="dd002-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="dd002-108">Member</span></span>|<span data-ttu-id="dd002-109">値</span><span class="sxs-lookup"><span data-stu-id="dd002-109">Value</span></span>|<span data-ttu-id="dd002-110">説明</span><span class="sxs-lookup"><span data-stu-id="dd002-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd002-111">none</span><span class="sxs-lookup"><span data-stu-id="dd002-111">none</span></span>|<span data-ttu-id="dd002-112">.0</span><span class="sxs-lookup"><span data-stu-id="dd002-112">0</span></span>|<span data-ttu-id="dd002-113">ルーティングポリシーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="dd002-113">No routing policy specified.</span></span>|
|<span data-ttu-id="dd002-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="dd002-114">splitTunnel</span></span>|<span data-ttu-id="dd002-115">1-d</span><span class="sxs-lookup"><span data-stu-id="dd002-115">1</span></span>|<span data-ttu-id="dd002-116">指定したアプリのネットワークトラフィックは、VPN 経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="dd002-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="dd002-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="dd002-117">forceTunnel</span></span>|<span data-ttu-id="dd002-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="dd002-118">2</span></span>|<span data-ttu-id="dd002-119">すべてのネットワークトラフィックは、VPN 経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="dd002-119">All network traffic will be routed through the VPN.</span></span>|





