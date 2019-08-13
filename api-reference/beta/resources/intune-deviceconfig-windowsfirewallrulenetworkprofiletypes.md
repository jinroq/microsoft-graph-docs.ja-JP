---
title: windowsFirewallRuleNetworkProfileTypes 列挙型
description: ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c7e0f50a830134cea6b4bfc15c6e68b49b86d0a2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371083"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="55bf7-103">windowsFirewallRuleNetworkProfileTypes 列挙型</span><span class="sxs-lookup"><span data-stu-id="55bf7-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="55bf7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55bf7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55bf7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="55bf7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55bf7-106">ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。</span><span class="sxs-lookup"><span data-stu-id="55bf7-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="55bf7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="55bf7-107">Members</span></span>
|<span data-ttu-id="55bf7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="55bf7-108">Member</span></span>|<span data-ttu-id="55bf7-109">値</span><span class="sxs-lookup"><span data-stu-id="55bf7-109">Value</span></span>|<span data-ttu-id="55bf7-110">説明</span><span class="sxs-lookup"><span data-stu-id="55bf7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55bf7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="55bf7-111">notConfigured</span></span>|<span data-ttu-id="55bf7-112">.0</span><span class="sxs-lookup"><span data-stu-id="55bf7-112">0</span></span>|<span data-ttu-id="55bf7-113">フラグは設定しません。</span><span class="sxs-lookup"><span data-stu-id="55bf7-113">No flags set.</span></span>|
|<span data-ttu-id="55bf7-114">domain</span><span class="sxs-lookup"><span data-stu-id="55bf7-114">domain</span></span>|<span data-ttu-id="55bf7-115">1-d</span><span class="sxs-lookup"><span data-stu-id="55bf7-115">1</span></span>|<span data-ttu-id="55bf7-116">ドメインに接続されているネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="55bf7-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="55bf7-117">機密性</span><span class="sxs-lookup"><span data-stu-id="55bf7-117">private</span></span>|<span data-ttu-id="55bf7-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="55bf7-118">2</span></span>|<span data-ttu-id="55bf7-119">プライベートネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="55bf7-119">The profile for private networks.</span></span>|
|<span data-ttu-id="55bf7-120">public</span><span class="sxs-lookup"><span data-stu-id="55bf7-120">public</span></span>|<span data-ttu-id="55bf7-121">2/4</span><span class="sxs-lookup"><span data-stu-id="55bf7-121">4</span></span>|<span data-ttu-id="55bf7-122">パブリックネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="55bf7-122">The profile for public networks.</span></span>|



