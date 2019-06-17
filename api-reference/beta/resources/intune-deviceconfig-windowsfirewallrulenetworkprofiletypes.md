---
title: windowsFirewallRuleNetworkProfileTypes 列挙型
description: ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dd5ac398700338cb4e26d435fae042773c03f8a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994098"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="be055-103">windowsFirewallRuleNetworkProfileTypes 列挙型</span><span class="sxs-lookup"><span data-stu-id="be055-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="be055-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be055-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be055-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="be055-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be055-106">ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。</span><span class="sxs-lookup"><span data-stu-id="be055-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="be055-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="be055-107">Members</span></span>
|<span data-ttu-id="be055-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="be055-108">Member</span></span>|<span data-ttu-id="be055-109">値</span><span class="sxs-lookup"><span data-stu-id="be055-109">Value</span></span>|<span data-ttu-id="be055-110">説明</span><span class="sxs-lookup"><span data-stu-id="be055-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be055-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="be055-111">notConfigured</span></span>|<span data-ttu-id="be055-112">.0</span><span class="sxs-lookup"><span data-stu-id="be055-112">0</span></span>|<span data-ttu-id="be055-113">フラグは設定しません。</span><span class="sxs-lookup"><span data-stu-id="be055-113">No flags set.</span></span>|
|<span data-ttu-id="be055-114">domain</span><span class="sxs-lookup"><span data-stu-id="be055-114">domain</span></span>|<span data-ttu-id="be055-115">1-d</span><span class="sxs-lookup"><span data-stu-id="be055-115">1</span></span>|<span data-ttu-id="be055-116">ドメインに接続されているネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="be055-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="be055-117">機密性</span><span class="sxs-lookup"><span data-stu-id="be055-117">private</span></span>|<span data-ttu-id="be055-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="be055-118">2</span></span>|<span data-ttu-id="be055-119">プライベートネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="be055-119">The profile for private networks.</span></span>|
|<span data-ttu-id="be055-120">public</span><span class="sxs-lookup"><span data-stu-id="be055-120">public</span></span>|<span data-ttu-id="be055-121">2/4</span><span class="sxs-lookup"><span data-stu-id="be055-121">4</span></span>|<span data-ttu-id="be055-122">パブリックネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="be055-122">The profile for public networks.</span></span>|





