---
title: vpnProviderType 列挙型
description: アプリごとの VPN のプロバイダーの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 43e9c146fc30e9dfaadef45b42e45dcf0787f13f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969465"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="39c49-103">vpnProviderType 列挙型</span><span class="sxs-lookup"><span data-stu-id="39c49-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="39c49-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39c49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39c49-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="39c49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39c49-106">アプリごとの VPN のプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="39c49-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="39c49-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="39c49-107">Members</span></span>
|<span data-ttu-id="39c49-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="39c49-108">Member</span></span>|<span data-ttu-id="39c49-109">値</span><span class="sxs-lookup"><span data-stu-id="39c49-109">Value</span></span>|<span data-ttu-id="39c49-110">説明</span><span class="sxs-lookup"><span data-stu-id="39c49-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39c49-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="39c49-111">notConfigured</span></span>|<span data-ttu-id="39c49-112">.0</span><span class="sxs-lookup"><span data-stu-id="39c49-112">0</span></span>|<span data-ttu-id="39c49-113">トンネルトラフィックは明示的に構成されていません。</span><span class="sxs-lookup"><span data-stu-id="39c49-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="39c49-114">appProxy</span><span class="sxs-lookup"><span data-stu-id="39c49-114">appProxy</span></span>|<span data-ttu-id="39c49-115">1-d</span><span class="sxs-lookup"><span data-stu-id="39c49-115">1</span></span>|<span data-ttu-id="39c49-116">アプリケーション層でのトンネルトラフィック。</span><span class="sxs-lookup"><span data-stu-id="39c49-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="39c49-117">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="39c49-117">packetTunnel</span></span>|<span data-ttu-id="39c49-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="39c49-118">2</span></span>|<span data-ttu-id="39c49-119">IP 層でのトンネルトラフィック。</span><span class="sxs-lookup"><span data-stu-id="39c49-119">Tunnel traffic at the IP layer.</span></span>|





