---
title: vpnProviderType 列挙型
description: アプリケーションごとの vpn プロバイダーの種類。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea3e3fcac5fc84270fcdb63b6ab673cb9f55aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861286"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="fc065-103">vpnProviderType 列挙型</span><span class="sxs-lookup"><span data-stu-id="fc065-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="fc065-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fc065-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc065-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc065-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc065-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc065-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc065-107">アプリケーションごとの vpn プロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="fc065-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="fc065-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fc065-108">Members</span></span>
|<span data-ttu-id="fc065-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="fc065-109">Member</span></span>|<span data-ttu-id="fc065-110">値</span><span class="sxs-lookup"><span data-stu-id="fc065-110">Value</span></span>|<span data-ttu-id="fc065-111">説明</span><span class="sxs-lookup"><span data-stu-id="fc065-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc065-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fc065-112">notConfigured</span></span>|<span data-ttu-id="fc065-113">0</span><span class="sxs-lookup"><span data-stu-id="fc065-113">0</span></span>|<span data-ttu-id="fc065-114">トンネル トラフィックが明示的に構成されていません。</span><span class="sxs-lookup"><span data-stu-id="fc065-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="fc065-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="fc065-115">appProxy</span></span>|<span data-ttu-id="fc065-116">1</span><span class="sxs-lookup"><span data-stu-id="fc065-116">1</span></span>|<span data-ttu-id="fc065-117">アプリケーション レイヤーでトラフィックをトンネルします。</span><span class="sxs-lookup"><span data-stu-id="fc065-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="fc065-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="fc065-118">packetTunnel</span></span>|<span data-ttu-id="fc065-119">2</span><span class="sxs-lookup"><span data-stu-id="fc065-119">2</span></span>|<span data-ttu-id="fc065-120">IP 層でトラフィックをトンネリングします。</span><span class="sxs-lookup"><span data-stu-id="fc065-120">Tunnel traffic at the IP layer.</span></span>|





