---
title: vpnProviderType 列挙型
description: アプリケーションごとの vpn プロバイダーの種類。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2de8f78222ba0c945000b84f28039c2f6af58daa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407222"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="23fa0-103">vpnProviderType 列挙型</span><span class="sxs-lookup"><span data-stu-id="23fa0-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="23fa0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23fa0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23fa0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23fa0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23fa0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23fa0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23fa0-107">アプリケーションごとの vpn プロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="23fa0-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="23fa0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="23fa0-108">Members</span></span>
|<span data-ttu-id="23fa0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="23fa0-109">Member</span></span>|<span data-ttu-id="23fa0-110">値</span><span class="sxs-lookup"><span data-stu-id="23fa0-110">Value</span></span>|<span data-ttu-id="23fa0-111">説明</span><span class="sxs-lookup"><span data-stu-id="23fa0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23fa0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="23fa0-112">notConfigured</span></span>|<span data-ttu-id="23fa0-113">0</span><span class="sxs-lookup"><span data-stu-id="23fa0-113">0</span></span>|<span data-ttu-id="23fa0-114">トンネル トラフィックが明示的に構成されていません。</span><span class="sxs-lookup"><span data-stu-id="23fa0-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="23fa0-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="23fa0-115">appProxy</span></span>|<span data-ttu-id="23fa0-116">1</span><span class="sxs-lookup"><span data-stu-id="23fa0-116">1</span></span>|<span data-ttu-id="23fa0-117">アプリケーション レイヤーでトラフィックをトンネルします。</span><span class="sxs-lookup"><span data-stu-id="23fa0-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="23fa0-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="23fa0-118">packetTunnel</span></span>|<span data-ttu-id="23fa0-119">2</span><span class="sxs-lookup"><span data-stu-id="23fa0-119">2</span></span>|<span data-ttu-id="23fa0-120">IP 層でトラフィックをトンネリングします。</span><span class="sxs-lookup"><span data-stu-id="23fa0-120">Tunnel traffic at the IP layer.</span></span>|




