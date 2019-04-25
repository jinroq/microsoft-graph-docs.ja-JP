---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックルールのルーティングポリシーを指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 360a7ea9ab46a9d482fd8e41c2d2a64041453e88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555018"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="ae45b-103">vpnTrafficRuleRoutingPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ae45b-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="ae45b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae45b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae45b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae45b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae45b-106">VPN トラフィックルールのルーティングポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae45b-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="ae45b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae45b-107">Members</span></span>
|<span data-ttu-id="ae45b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae45b-108">Member</span></span>|<span data-ttu-id="ae45b-109">値</span><span class="sxs-lookup"><span data-stu-id="ae45b-109">Value</span></span>|<span data-ttu-id="ae45b-110">説明</span><span class="sxs-lookup"><span data-stu-id="ae45b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae45b-111">なし</span><span class="sxs-lookup"><span data-stu-id="ae45b-111">none</span></span>|<span data-ttu-id="ae45b-112">.0</span><span class="sxs-lookup"><span data-stu-id="ae45b-112">0</span></span>|<span data-ttu-id="ae45b-113">ルーティングポリシーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="ae45b-113">No routing policy specified.</span></span>|
|<span data-ttu-id="ae45b-114">splittunnel</span><span class="sxs-lookup"><span data-stu-id="ae45b-114">splitTunnel</span></span>|<span data-ttu-id="ae45b-115">1 </span><span class="sxs-lookup"><span data-stu-id="ae45b-115">1</span></span>|<span data-ttu-id="ae45b-116">指定したアプリのネットワークトラフィックは、VPN 経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="ae45b-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="ae45b-117">forcetunnel</span><span class="sxs-lookup"><span data-stu-id="ae45b-117">forceTunnel</span></span>|<span data-ttu-id="ae45b-118">2 </span><span class="sxs-lookup"><span data-stu-id="ae45b-118">2</span></span>|<span data-ttu-id="ae45b-119">すべてのネットワークトラフィックは、VPN 経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="ae45b-119">All network traffic will be routed through the VPN.</span></span>|





