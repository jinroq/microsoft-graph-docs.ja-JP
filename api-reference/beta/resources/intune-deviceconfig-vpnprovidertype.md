---
title: vpnProviderType 列挙型
description: アプリごとの VPN のプロバイダーの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ea4dee71a18a6ddca4519d8b421d2097fc7907b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367646"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="a75d1-103">vpnProviderType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a75d1-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="a75d1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a75d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a75d1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a75d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a75d1-106">アプリごとの VPN のプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="a75d1-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="a75d1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a75d1-107">Members</span></span>
|<span data-ttu-id="a75d1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a75d1-108">Member</span></span>|<span data-ttu-id="a75d1-109">値</span><span class="sxs-lookup"><span data-stu-id="a75d1-109">Value</span></span>|<span data-ttu-id="a75d1-110">説明</span><span class="sxs-lookup"><span data-stu-id="a75d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a75d1-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a75d1-111">notConfigured</span></span>|<span data-ttu-id="a75d1-112">.0</span><span class="sxs-lookup"><span data-stu-id="a75d1-112">0</span></span>|<span data-ttu-id="a75d1-113">トンネルトラフィックは明示的に構成されていません。</span><span class="sxs-lookup"><span data-stu-id="a75d1-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="a75d1-114">appProxy</span><span class="sxs-lookup"><span data-stu-id="a75d1-114">appProxy</span></span>|<span data-ttu-id="a75d1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a75d1-115">1</span></span>|<span data-ttu-id="a75d1-116">アプリケーション層でのトンネルトラフィック。</span><span class="sxs-lookup"><span data-stu-id="a75d1-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="a75d1-117">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="a75d1-117">packetTunnel</span></span>|<span data-ttu-id="a75d1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a75d1-118">2</span></span>|<span data-ttu-id="a75d1-119">IP 層でのトンネルトラフィック。</span><span class="sxs-lookup"><span data-stu-id="a75d1-119">Tunnel traffic at the IP layer.</span></span>|



