---
title: wiFiSecurityType 列挙型
description: wi-fi セキュリティの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c16265ecf9b4fa56536838dde1f4f1f757d8b1f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159046"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="2fee4-103">wiFiSecurityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="2fee4-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="2fee4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fee4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fee4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2fee4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fee4-106">wi-fi セキュリティの種類。</span><span class="sxs-lookup"><span data-stu-id="2fee4-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="2fee4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2fee4-107">Members</span></span>
|<span data-ttu-id="2fee4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2fee4-108">Member</span></span>|<span data-ttu-id="2fee4-109">値</span><span class="sxs-lookup"><span data-stu-id="2fee4-109">Value</span></span>|<span data-ttu-id="2fee4-110">説明</span><span class="sxs-lookup"><span data-stu-id="2fee4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fee4-111">開か</span><span class="sxs-lookup"><span data-stu-id="2fee4-111">open</span></span>|<span data-ttu-id="2fee4-112">.0</span><span class="sxs-lookup"><span data-stu-id="2fee4-112">0</span></span>|<span data-ttu-id="2fee4-113">開く (認証なし)。</span><span class="sxs-lookup"><span data-stu-id="2fee4-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="2fee4-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="2fee4-114">wpaPersonal</span></span>|<span data-ttu-id="2fee4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="2fee4-115">1</span></span>|<span data-ttu-id="2fee4-116">WPA-個人用。</span><span class="sxs-lookup"><span data-stu-id="2fee4-116">WPA-Personal.</span></span>|
|<span data-ttu-id="2fee4-117">wpaenterprise</span><span class="sxs-lookup"><span data-stu-id="2fee4-117">wpaEnterprise</span></span>|<span data-ttu-id="2fee4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="2fee4-118">2</span></span>|<span data-ttu-id="2fee4-119">WPA-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="2fee4-119">WPA-Enterprise.</span></span> <span data-ttu-id="2fee4-120">エンタープライズオプションを構成するには、IOSEnterpriseWifiConfiguration type を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fee4-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="2fee4-121">wep</span><span class="sxs-lookup"><span data-stu-id="2fee4-121">wep</span></span>|<span data-ttu-id="2fee4-122">1/3</span><span class="sxs-lookup"><span data-stu-id="2fee4-122">3</span></span>|<span data-ttu-id="2fee4-123">WEP 暗号化。</span><span class="sxs-lookup"><span data-stu-id="2fee4-123">WEP Encryption.</span></span>|
|<span data-ttu-id="2fee4-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="2fee4-124">wpa2Personal</span></span>|<span data-ttu-id="2fee4-125">2/4</span><span class="sxs-lookup"><span data-stu-id="2fee4-125">4</span></span>|<span data-ttu-id="2fee4-126">WPA2-個人用。</span><span class="sxs-lookup"><span data-stu-id="2fee4-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="2fee4-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="2fee4-127">wpa2Enterprise</span></span>|<span data-ttu-id="2fee4-128">5</span><span class="sxs-lookup"><span data-stu-id="2fee4-128">5</span></span>|<span data-ttu-id="2fee4-129">WPA2-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="2fee4-129">WPA2-Enterprise.</span></span> <span data-ttu-id="2fee4-130">エンタープライズオプションを構成するには、WindowsWifiEnterpriseEAPConfiguration type を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fee4-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




