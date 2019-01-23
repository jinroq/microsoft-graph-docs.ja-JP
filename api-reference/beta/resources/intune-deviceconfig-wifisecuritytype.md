---
title: wiFiSecurityType 列挙型
description: Wi-fi セキュリティの種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422132"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="5ed55-103">wiFiSecurityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5ed55-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="5ed55-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ed55-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5ed55-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ed55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ed55-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ed55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ed55-107">Wi-fi セキュリティの種類です。</span><span class="sxs-lookup"><span data-stu-id="5ed55-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="5ed55-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ed55-108">Members</span></span>
|<span data-ttu-id="5ed55-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ed55-109">Member</span></span>|<span data-ttu-id="5ed55-110">値</span><span class="sxs-lookup"><span data-stu-id="5ed55-110">Value</span></span>|<span data-ttu-id="5ed55-111">説明</span><span class="sxs-lookup"><span data-stu-id="5ed55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed55-112">開く</span><span class="sxs-lookup"><span data-stu-id="5ed55-112">open</span></span>|<span data-ttu-id="5ed55-113">0</span><span class="sxs-lookup"><span data-stu-id="5ed55-113">0</span></span>|<span data-ttu-id="5ed55-114">(認証なし) を開きます。</span><span class="sxs-lookup"><span data-stu-id="5ed55-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="5ed55-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="5ed55-115">wpaPersonal</span></span>|<span data-ttu-id="5ed55-116">1</span><span class="sxs-lookup"><span data-stu-id="5ed55-116">1</span></span>|<span data-ttu-id="5ed55-117">WPA-パーソナルです。</span><span class="sxs-lookup"><span data-stu-id="5ed55-117">WPA-Personal.</span></span>|
|<span data-ttu-id="5ed55-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="5ed55-118">wpaEnterprise</span></span>|<span data-ttu-id="5ed55-119">2</span><span class="sxs-lookup"><span data-stu-id="5ed55-119">2</span></span>|<span data-ttu-id="5ed55-120">WPA-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="5ed55-120">WPA-Enterprise.</span></span> <span data-ttu-id="5ed55-121">エンタープライズ オプションを構成するのには IOSEnterpriseWifiConfiguration 型を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ed55-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="5ed55-122">wep</span><span class="sxs-lookup"><span data-stu-id="5ed55-122">wep</span></span>|<span data-ttu-id="5ed55-123">3</span><span class="sxs-lookup"><span data-stu-id="5ed55-123">3</span></span>|<span data-ttu-id="5ed55-124">WEP 暗号化します。</span><span class="sxs-lookup"><span data-stu-id="5ed55-124">WEP Encryption.</span></span>|
|<span data-ttu-id="5ed55-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="5ed55-125">wpa2Personal</span></span>|<span data-ttu-id="5ed55-126">4</span><span class="sxs-lookup"><span data-stu-id="5ed55-126">4</span></span>|<span data-ttu-id="5ed55-127">WPA2-パーソナルです。</span><span class="sxs-lookup"><span data-stu-id="5ed55-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="5ed55-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="5ed55-128">wpa2Enterprise</span></span>|<span data-ttu-id="5ed55-129">5</span><span class="sxs-lookup"><span data-stu-id="5ed55-129">5</span></span>|<span data-ttu-id="5ed55-130">WPA2-エンタープライズ。</span><span class="sxs-lookup"><span data-stu-id="5ed55-130">WPA2-Enterprise.</span></span> <span data-ttu-id="5ed55-131">エンタープライズ オプションを構成するのには WindowsWifiEnterpriseEAPConfiguration 型を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ed55-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




