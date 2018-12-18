---
title: wiFiSecurityType 列挙型
description: Wi-fi セキュリティの種類です。
author: tfitzmac
ms.openlocfilehash: 291bc3660971a90ea113959368542e715a86b570
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329191"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="5b289-103">wiFiSecurityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5b289-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="5b289-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b289-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b289-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b289-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b289-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b289-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b289-107">Wi-fi セキュリティの種類です。</span><span class="sxs-lookup"><span data-stu-id="5b289-107">Wi-Fi Security Types.</span></span>
## <a name="members"></a><span data-ttu-id="5b289-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5b289-108">Members</span></span>
|<span data-ttu-id="5b289-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5b289-109">Member</span></span>|<span data-ttu-id="5b289-110">値</span><span class="sxs-lookup"><span data-stu-id="5b289-110">Value</span></span>|<span data-ttu-id="5b289-111">説明</span><span class="sxs-lookup"><span data-stu-id="5b289-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b289-112">開く</span><span class="sxs-lookup"><span data-stu-id="5b289-112">open</span></span>|<span data-ttu-id="5b289-113">0</span><span class="sxs-lookup"><span data-stu-id="5b289-113">0</span></span>|<span data-ttu-id="5b289-114">(認証なし) を開きます。</span><span class="sxs-lookup"><span data-stu-id="5b289-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="5b289-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="5b289-115">wpaPersonal</span></span>|<span data-ttu-id="5b289-116">1</span><span class="sxs-lookup"><span data-stu-id="5b289-116">1</span></span>|<span data-ttu-id="5b289-117">WPA-パーソナルです。</span><span class="sxs-lookup"><span data-stu-id="5b289-117">WPA-Personal.</span></span>|
|<span data-ttu-id="5b289-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="5b289-118">wpaEnterprise</span></span>|<span data-ttu-id="5b289-119">2</span><span class="sxs-lookup"><span data-stu-id="5b289-119">2</span></span>|<span data-ttu-id="5b289-120">WPA-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="5b289-120">WPA-Enterprise.</span></span> <span data-ttu-id="5b289-121">エンタープライズ オプションを構成するのには IOSEnterpriseWifiConfiguration 型を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b289-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="5b289-122">wep</span><span class="sxs-lookup"><span data-stu-id="5b289-122">wep</span></span>|<span data-ttu-id="5b289-123">3</span><span class="sxs-lookup"><span data-stu-id="5b289-123">3</span></span>|<span data-ttu-id="5b289-124">WEP 暗号化します。</span><span class="sxs-lookup"><span data-stu-id="5b289-124">WEP Encryption.</span></span>|
|<span data-ttu-id="5b289-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="5b289-125">wpa2Personal</span></span>|<span data-ttu-id="5b289-126">4</span><span class="sxs-lookup"><span data-stu-id="5b289-126">4</span></span>|<span data-ttu-id="5b289-127">WPA2-パーソナルです。</span><span class="sxs-lookup"><span data-stu-id="5b289-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="5b289-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="5b289-128">wpa2Enterprise</span></span>|<span data-ttu-id="5b289-129">5</span><span class="sxs-lookup"><span data-stu-id="5b289-129">5</span></span>|<span data-ttu-id="5b289-130">WPA2-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="5b289-130">WPA2-Enterprise.</span></span> <span data-ttu-id="5b289-131">エンタープライズ オプションを構成するのには WindowsWifiEnterpriseEAPConfiguration 型を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b289-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





