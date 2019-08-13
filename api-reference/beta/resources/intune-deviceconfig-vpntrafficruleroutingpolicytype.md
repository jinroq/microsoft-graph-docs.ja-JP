---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックルールのルーティングポリシーを指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 529c42722d8ce3827bb9daa4c0f158cfd92d8383
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367520"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="f3b90-103">vpnTrafficRuleRoutingPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f3b90-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="f3b90-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3b90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3b90-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3b90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3b90-106">VPN トラフィックルールのルーティングポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3b90-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="f3b90-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3b90-107">Members</span></span>
|<span data-ttu-id="f3b90-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3b90-108">Member</span></span>|<span data-ttu-id="f3b90-109">値</span><span class="sxs-lookup"><span data-stu-id="f3b90-109">Value</span></span>|<span data-ttu-id="f3b90-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3b90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3b90-111">none</span><span class="sxs-lookup"><span data-stu-id="f3b90-111">none</span></span>|<span data-ttu-id="f3b90-112">.0</span><span class="sxs-lookup"><span data-stu-id="f3b90-112">0</span></span>|<span data-ttu-id="f3b90-113">ルーティングポリシーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="f3b90-113">No routing policy specified.</span></span>|
|<span data-ttu-id="f3b90-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="f3b90-114">splitTunnel</span></span>|<span data-ttu-id="f3b90-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f3b90-115">1</span></span>|<span data-ttu-id="f3b90-116">指定したアプリのネットワークトラフィックは、VPN 経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="f3b90-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="f3b90-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="f3b90-117">forceTunnel</span></span>|<span data-ttu-id="f3b90-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f3b90-118">2</span></span>|<span data-ttu-id="f3b90-119">すべてのネットワークトラフィックは、VPN 経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="f3b90-119">All network traffic will be routed through the VPN.</span></span>|



