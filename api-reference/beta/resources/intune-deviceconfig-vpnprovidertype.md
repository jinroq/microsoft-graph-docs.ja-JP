---
title: vpnprovidertype 列挙型
description: アプリごとの VPN のプロバイダーの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e47f4d20cb843b62928c6c66e468d00f5a4f743
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561916"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="65500-103">vpnprovidertype 列挙型</span><span class="sxs-lookup"><span data-stu-id="65500-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="65500-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65500-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65500-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65500-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65500-106">アプリごとの VPN のプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="65500-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="65500-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="65500-107">Members</span></span>
|<span data-ttu-id="65500-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="65500-108">Member</span></span>|<span data-ttu-id="65500-109">値</span><span class="sxs-lookup"><span data-stu-id="65500-109">Value</span></span>|<span data-ttu-id="65500-110">説明</span><span class="sxs-lookup"><span data-stu-id="65500-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65500-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="65500-111">notConfigured</span></span>|<span data-ttu-id="65500-112">.0</span><span class="sxs-lookup"><span data-stu-id="65500-112">0</span></span>|<span data-ttu-id="65500-113">トンネルトラフィックは明示的に構成されていません。</span><span class="sxs-lookup"><span data-stu-id="65500-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="65500-114">appproxy</span><span class="sxs-lookup"><span data-stu-id="65500-114">appProxy</span></span>|<span data-ttu-id="65500-115">1 </span><span class="sxs-lookup"><span data-stu-id="65500-115">1</span></span>|<span data-ttu-id="65500-116">アプリケーション層でのトンネルトラフィック。</span><span class="sxs-lookup"><span data-stu-id="65500-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="65500-117">packettunnel</span><span class="sxs-lookup"><span data-stu-id="65500-117">packetTunnel</span></span>|<span data-ttu-id="65500-118">2 </span><span class="sxs-lookup"><span data-stu-id="65500-118">2</span></span>|<span data-ttu-id="65500-119">IP 層でのトンネルトラフィック。</span><span class="sxs-lookup"><span data-stu-id="65500-119">Tunnel traffic at the IP layer.</span></span>|





