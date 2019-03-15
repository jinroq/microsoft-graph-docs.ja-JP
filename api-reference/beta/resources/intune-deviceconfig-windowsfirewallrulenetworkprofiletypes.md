---
title: windowsFirewallRuleNetworkProfileTypes 列挙型
description: ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9aad571c5563427343ebd6686073f98b7ac703cb
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631571"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="cf54d-103">windowsFirewallRuleNetworkProfileTypes 列挙型</span><span class="sxs-lookup"><span data-stu-id="cf54d-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="cf54d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf54d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf54d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf54d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf54d-106">ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。</span><span class="sxs-lookup"><span data-stu-id="cf54d-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="cf54d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="cf54d-107">Members</span></span>
|<span data-ttu-id="cf54d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="cf54d-108">Member</span></span>|<span data-ttu-id="cf54d-109">値</span><span class="sxs-lookup"><span data-stu-id="cf54d-109">Value</span></span>|<span data-ttu-id="cf54d-110">説明</span><span class="sxs-lookup"><span data-stu-id="cf54d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf54d-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cf54d-111">notConfigured</span></span>|<span data-ttu-id="cf54d-112">.0</span><span class="sxs-lookup"><span data-stu-id="cf54d-112">0</span></span>|<span data-ttu-id="cf54d-113">フラグは設定しません。</span><span class="sxs-lookup"><span data-stu-id="cf54d-113">No flags set.</span></span>|
|<span data-ttu-id="cf54d-114">domain</span><span class="sxs-lookup"><span data-stu-id="cf54d-114">domain</span></span>|<span data-ttu-id="cf54d-115">1</span><span class="sxs-lookup"><span data-stu-id="cf54d-115">1</span></span>|<span data-ttu-id="cf54d-116">ドメインに接続されているネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="cf54d-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="cf54d-117">機密性</span><span class="sxs-lookup"><span data-stu-id="cf54d-117">private</span></span>|<span data-ttu-id="cf54d-118">2</span><span class="sxs-lookup"><span data-stu-id="cf54d-118">2</span></span>|<span data-ttu-id="cf54d-119">プライベートネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="cf54d-119">The profile for private networks.</span></span>|
|<span data-ttu-id="cf54d-120">public</span><span class="sxs-lookup"><span data-stu-id="cf54d-120">public</span></span>|<span data-ttu-id="cf54d-121">2/4</span><span class="sxs-lookup"><span data-stu-id="cf54d-121">4</span></span>|<span data-ttu-id="cf54d-122">パブリックネットワークのプロファイル。</span><span class="sxs-lookup"><span data-stu-id="cf54d-122">The profile for public networks.</span></span>|




