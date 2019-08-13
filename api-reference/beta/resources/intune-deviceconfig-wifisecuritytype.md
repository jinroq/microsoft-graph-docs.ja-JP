---
title: wiFiSecurityType 列挙型
description: Wi-fi セキュリティの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8bfe6184b2427584c54094636ef7c71f857ec1f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369403"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="7df2b-103">wiFiSecurityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7df2b-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="7df2b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7df2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7df2b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7df2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7df2b-106">Wi-fi セキュリティの種類。</span><span class="sxs-lookup"><span data-stu-id="7df2b-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="7df2b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7df2b-107">Members</span></span>
|<span data-ttu-id="7df2b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7df2b-108">Member</span></span>|<span data-ttu-id="7df2b-109">値</span><span class="sxs-lookup"><span data-stu-id="7df2b-109">Value</span></span>|<span data-ttu-id="7df2b-110">説明</span><span class="sxs-lookup"><span data-stu-id="7df2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df2b-111">開か</span><span class="sxs-lookup"><span data-stu-id="7df2b-111">open</span></span>|<span data-ttu-id="7df2b-112">.0</span><span class="sxs-lookup"><span data-stu-id="7df2b-112">0</span></span>|<span data-ttu-id="7df2b-113">開く (認証なし)。</span><span class="sxs-lookup"><span data-stu-id="7df2b-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="7df2b-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="7df2b-114">wpaPersonal</span></span>|<span data-ttu-id="7df2b-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7df2b-115">1</span></span>|<span data-ttu-id="7df2b-116">WPA-個人用。</span><span class="sxs-lookup"><span data-stu-id="7df2b-116">WPA-Personal.</span></span>|
|<span data-ttu-id="7df2b-117">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="7df2b-117">wpaEnterprise</span></span>|<span data-ttu-id="7df2b-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7df2b-118">2</span></span>|<span data-ttu-id="7df2b-119">WPA-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="7df2b-119">WPA-Enterprise.</span></span> <span data-ttu-id="7df2b-120">エンタープライズオプションを構成するには、IOSEnterpriseWifiConfiguration type を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7df2b-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="7df2b-121">wep</span><span class="sxs-lookup"><span data-stu-id="7df2b-121">wep</span></span>|<span data-ttu-id="7df2b-122">1/3</span><span class="sxs-lookup"><span data-stu-id="7df2b-122">3</span></span>|<span data-ttu-id="7df2b-123">WEP 暗号化。</span><span class="sxs-lookup"><span data-stu-id="7df2b-123">WEP Encryption.</span></span>|
|<span data-ttu-id="7df2b-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="7df2b-124">wpa2Personal</span></span>|<span data-ttu-id="7df2b-125">2/4</span><span class="sxs-lookup"><span data-stu-id="7df2b-125">4</span></span>|<span data-ttu-id="7df2b-126">WPA2-個人用。</span><span class="sxs-lookup"><span data-stu-id="7df2b-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="7df2b-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="7df2b-127">wpa2Enterprise</span></span>|<span data-ttu-id="7df2b-128">5</span><span class="sxs-lookup"><span data-stu-id="7df2b-128">5</span></span>|<span data-ttu-id="7df2b-129">WPA2-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="7df2b-129">WPA2-Enterprise.</span></span> <span data-ttu-id="7df2b-130">エンタープライズオプションを構成するには、WindowsWifiEnterpriseEAPConfiguration type を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7df2b-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



