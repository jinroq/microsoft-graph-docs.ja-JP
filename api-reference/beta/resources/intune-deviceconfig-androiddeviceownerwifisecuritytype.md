---
title: androidDeviceOwnerWiFiSecurityType 列挙型
description: Android デバイス所有者の wi-fi セキュリティの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 19d96ae6c56d0d37e857d6e9e1f0786f225e25e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971467"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a><span data-ttu-id="65022-103">androidDeviceOwnerWiFiSecurityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="65022-103">androidDeviceOwnerWiFiSecurityType enum type</span></span>

> <span data-ttu-id="65022-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65022-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65022-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65022-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65022-106">Android デバイス所有者の wi-fi セキュリティの種類。</span><span class="sxs-lookup"><span data-stu-id="65022-106">Wi-Fi Security Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="65022-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="65022-107">Members</span></span>
|<span data-ttu-id="65022-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="65022-108">Member</span></span>|<span data-ttu-id="65022-109">値</span><span class="sxs-lookup"><span data-stu-id="65022-109">Value</span></span>|<span data-ttu-id="65022-110">説明</span><span class="sxs-lookup"><span data-stu-id="65022-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65022-111">開か</span><span class="sxs-lookup"><span data-stu-id="65022-111">open</span></span>|<span data-ttu-id="65022-112">.0</span><span class="sxs-lookup"><span data-stu-id="65022-112">0</span></span>|<span data-ttu-id="65022-113">開く (認証なし)。</span><span class="sxs-lookup"><span data-stu-id="65022-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="65022-114">wep</span><span class="sxs-lookup"><span data-stu-id="65022-114">wep</span></span>|<span data-ttu-id="65022-115">1-d</span><span class="sxs-lookup"><span data-stu-id="65022-115">1</span></span>|<span data-ttu-id="65022-116">WEP 暗号化。</span><span class="sxs-lookup"><span data-stu-id="65022-116">WEP Encryption.</span></span>|
|<span data-ttu-id="65022-117">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="65022-117">wpaPersonal</span></span>|<span data-ttu-id="65022-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="65022-118">2</span></span>|<span data-ttu-id="65022-119">WPA-Personal/WPA2-個人用。</span><span class="sxs-lookup"><span data-stu-id="65022-119">WPA-Personal/WPA2-Personal.</span></span>|
|<span data-ttu-id="65022-120">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="65022-120">wpaEnterprise</span></span>|<span data-ttu-id="65022-121">2/4</span><span class="sxs-lookup"><span data-stu-id="65022-121">4</span></span>|<span data-ttu-id="65022-122">WPA-エンタープライズ/WPA2-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="65022-122">WPA-Enterprise/WPA2-Enterprise.</span></span> <span data-ttu-id="65022-123">エンタープライズオプションを構成するには、AndroidDeviceOwnerEnterpriseWifiConfiguration type を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="65022-123">Must use AndroidDeviceOwnerEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|





