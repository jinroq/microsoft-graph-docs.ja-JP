---
title: androidDeviceOwnerWiFiSecurityType 列挙型
description: Android デバイス所有者の wi-fi セキュリティの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b54a451ac3e4444d58ad6cdd66abba61d6d69fb4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334746"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a><span data-ttu-id="661bd-103">androidDeviceOwnerWiFiSecurityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="661bd-103">androidDeviceOwnerWiFiSecurityType enum type</span></span>

> <span data-ttu-id="661bd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="661bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="661bd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="661bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="661bd-106">Android デバイス所有者の wi-fi セキュリティの種類。</span><span class="sxs-lookup"><span data-stu-id="661bd-106">Wi-Fi Security Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="661bd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="661bd-107">Members</span></span>
|<span data-ttu-id="661bd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="661bd-108">Member</span></span>|<span data-ttu-id="661bd-109">値</span><span class="sxs-lookup"><span data-stu-id="661bd-109">Value</span></span>|<span data-ttu-id="661bd-110">説明</span><span class="sxs-lookup"><span data-stu-id="661bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="661bd-111">開か</span><span class="sxs-lookup"><span data-stu-id="661bd-111">open</span></span>|<span data-ttu-id="661bd-112">.0</span><span class="sxs-lookup"><span data-stu-id="661bd-112">0</span></span>|<span data-ttu-id="661bd-113">開く (認証なし)。</span><span class="sxs-lookup"><span data-stu-id="661bd-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="661bd-114">wep</span><span class="sxs-lookup"><span data-stu-id="661bd-114">wep</span></span>|<span data-ttu-id="661bd-115">1-d</span><span class="sxs-lookup"><span data-stu-id="661bd-115">1</span></span>|<span data-ttu-id="661bd-116">WEP 暗号化。</span><span class="sxs-lookup"><span data-stu-id="661bd-116">WEP Encryption.</span></span>|
|<span data-ttu-id="661bd-117">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="661bd-117">wpaPersonal</span></span>|<span data-ttu-id="661bd-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="661bd-118">2</span></span>|<span data-ttu-id="661bd-119">WPA-Personal/WPA2-個人用。</span><span class="sxs-lookup"><span data-stu-id="661bd-119">WPA-Personal/WPA2-Personal.</span></span>|
|<span data-ttu-id="661bd-120">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="661bd-120">wpaEnterprise</span></span>|<span data-ttu-id="661bd-121">2/4</span><span class="sxs-lookup"><span data-stu-id="661bd-121">4</span></span>|<span data-ttu-id="661bd-122">WPA-エンタープライズ/WPA2-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="661bd-122">WPA-Enterprise/WPA2-Enterprise.</span></span> <span data-ttu-id="661bd-123">エンタープライズオプションを構成するには、AndroidDeviceOwnerEnterpriseWifiConfiguration type を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="661bd-123">Must use AndroidDeviceOwnerEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|



