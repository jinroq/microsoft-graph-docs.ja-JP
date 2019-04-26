---
title: wiFiSecurityType 列挙型
description: wi-fi セキュリティの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9144a5761691b0a50e40370b1f4d2d08967f2c28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554843"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="66d20-103">wiFiSecurityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="66d20-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="66d20-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66d20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d20-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66d20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d20-106">wi-fi セキュリティの種類。</span><span class="sxs-lookup"><span data-stu-id="66d20-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="66d20-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="66d20-107">Members</span></span>
|<span data-ttu-id="66d20-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="66d20-108">Member</span></span>|<span data-ttu-id="66d20-109">値</span><span class="sxs-lookup"><span data-stu-id="66d20-109">Value</span></span>|<span data-ttu-id="66d20-110">説明</span><span class="sxs-lookup"><span data-stu-id="66d20-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d20-111">開か</span><span class="sxs-lookup"><span data-stu-id="66d20-111">open</span></span>|<span data-ttu-id="66d20-112">.0</span><span class="sxs-lookup"><span data-stu-id="66d20-112">0</span></span>|<span data-ttu-id="66d20-113">開く (認証なし)。</span><span class="sxs-lookup"><span data-stu-id="66d20-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="66d20-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="66d20-114">wpaPersonal</span></span>|<span data-ttu-id="66d20-115">1 </span><span class="sxs-lookup"><span data-stu-id="66d20-115">1</span></span>|<span data-ttu-id="66d20-116">WPA-個人用。</span><span class="sxs-lookup"><span data-stu-id="66d20-116">WPA-Personal.</span></span>|
|<span data-ttu-id="66d20-117">wpaenterprise</span><span class="sxs-lookup"><span data-stu-id="66d20-117">wpaEnterprise</span></span>|<span data-ttu-id="66d20-118">2 </span><span class="sxs-lookup"><span data-stu-id="66d20-118">2</span></span>|<span data-ttu-id="66d20-119">WPA-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="66d20-119">WPA-Enterprise.</span></span> <span data-ttu-id="66d20-120">エンタープライズオプションを構成するには、IOSEnterpriseWifiConfiguration type を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="66d20-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="66d20-121">wep</span><span class="sxs-lookup"><span data-stu-id="66d20-121">wep</span></span>|<span data-ttu-id="66d20-122">3 </span><span class="sxs-lookup"><span data-stu-id="66d20-122">3</span></span>|<span data-ttu-id="66d20-123">WEP 暗号化。</span><span class="sxs-lookup"><span data-stu-id="66d20-123">WEP Encryption.</span></span>|
|<span data-ttu-id="66d20-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="66d20-124">wpa2Personal</span></span>|<span data-ttu-id="66d20-125">4 </span><span class="sxs-lookup"><span data-stu-id="66d20-125">4</span></span>|<span data-ttu-id="66d20-126">WPA2-個人用。</span><span class="sxs-lookup"><span data-stu-id="66d20-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="66d20-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="66d20-127">wpa2Enterprise</span></span>|<span data-ttu-id="66d20-128">5 </span><span class="sxs-lookup"><span data-stu-id="66d20-128">5</span></span>|<span data-ttu-id="66d20-129">WPA2-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="66d20-129">WPA2-Enterprise.</span></span> <span data-ttu-id="66d20-130">エンタープライズオプションを構成するには、WindowsWifiEnterpriseEAPConfiguration type を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="66d20-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





