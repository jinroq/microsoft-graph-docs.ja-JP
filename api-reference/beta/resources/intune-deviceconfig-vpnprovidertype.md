---
title: vpnprovidertype 列挙型
description: アプリごとの VPN のプロバイダーの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a62436f56a210bbb71606ebb8f2586e5b48f8d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163190"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="ac4cb-103">vpnprovidertype 列挙型</span><span class="sxs-lookup"><span data-stu-id="ac4cb-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="ac4cb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac4cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac4cb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ac4cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac4cb-106">アプリごとの VPN のプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="ac4cb-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="ac4cb-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ac4cb-107">Members</span></span>
|<span data-ttu-id="ac4cb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ac4cb-108">Member</span></span>|<span data-ttu-id="ac4cb-109">値</span><span class="sxs-lookup"><span data-stu-id="ac4cb-109">Value</span></span>|<span data-ttu-id="ac4cb-110">説明</span><span class="sxs-lookup"><span data-stu-id="ac4cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac4cb-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ac4cb-111">notConfigured</span></span>|<span data-ttu-id="ac4cb-112">.0</span><span class="sxs-lookup"><span data-stu-id="ac4cb-112">0</span></span>|<span data-ttu-id="ac4cb-113">トンネルトラフィックは明示的に構成されていません。</span><span class="sxs-lookup"><span data-stu-id="ac4cb-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="ac4cb-114">appproxy</span><span class="sxs-lookup"><span data-stu-id="ac4cb-114">appProxy</span></span>|<span data-ttu-id="ac4cb-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ac4cb-115">1</span></span>|<span data-ttu-id="ac4cb-116">アプリケーション層でのトンネルトラフィック。</span><span class="sxs-lookup"><span data-stu-id="ac4cb-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="ac4cb-117">packettunnel</span><span class="sxs-lookup"><span data-stu-id="ac4cb-117">packetTunnel</span></span>|<span data-ttu-id="ac4cb-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ac4cb-118">2</span></span>|<span data-ttu-id="ac4cb-119">IP 層でのトンネルトラフィック。</span><span class="sxs-lookup"><span data-stu-id="ac4cb-119">Tunnel traffic at the IP layer.</span></span>|




