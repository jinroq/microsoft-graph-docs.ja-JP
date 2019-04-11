---
title: deviceThreatProtectionLevel 列挙型
description: デバイス脅威保護 API のデバイスの脅威保護レベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 311a2e9a8db68d41d3c4a55f9691446b4e96c2d3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796172"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="a1ca5-103">deviceThreatProtectionLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="a1ca5-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="a1ca5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1ca5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1ca5-106">デバイス脅威保護 API のデバイスの脅威保護レベル。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="a1ca5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1ca5-107">Members</span></span>
|<span data-ttu-id="a1ca5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1ca5-108">Member</span></span>|<span data-ttu-id="a1ca5-109">値</span><span class="sxs-lookup"><span data-stu-id="a1ca5-109">Value</span></span>|<span data-ttu-id="a1ca5-110">説明</span><span class="sxs-lookup"><span data-stu-id="a1ca5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ca5-111">無効</span><span class="sxs-lookup"><span data-stu-id="a1ca5-111">unavailable</span></span>|<span data-ttu-id="a1ca5-112">.0</span><span class="sxs-lookup"><span data-stu-id="a1ca5-112">0</span></span>|<span data-ttu-id="a1ca5-113">既定値です。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-113">Default Value.</span></span> <span data-ttu-id="a1ca5-114">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-114">Do not use.</span></span>|
|<span data-ttu-id="a1ca5-115">セキュリティ保護</span><span class="sxs-lookup"><span data-stu-id="a1ca5-115">secured</span></span>|<span data-ttu-id="a1ca5-116">1-d</span><span class="sxs-lookup"><span data-stu-id="a1ca5-116">1</span></span>|<span data-ttu-id="a1ca5-117">デバイスの脅威レベルの要件: セキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="a1ca5-118">これは最も安全なレベルで、デバイス上に脅威が何も検出されなかったことを表します。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="a1ca5-119">低さ</span><span class="sxs-lookup"><span data-stu-id="a1ca5-119">low</span></span>|<span data-ttu-id="a1ca5-120">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a1ca5-120">2</span></span>|<span data-ttu-id="a1ca5-121">デバイスの脅威保護レベルの要件: 低。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="a1ca5-122">Low は、デバイスまたはデバイスのデータに対するリスクを最小限に抑える脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="a1ca5-123">medium</span><span class="sxs-lookup"><span data-stu-id="a1ca5-123">medium</span></span>|<span data-ttu-id="a1ca5-124">1/3</span><span class="sxs-lookup"><span data-stu-id="a1ca5-124">3</span></span>|<span data-ttu-id="a1ca5-125">デバイスの脅威保護レベルの要件: 中。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="a1ca5-126">Medium は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="a1ca5-127">高額</span><span class="sxs-lookup"><span data-stu-id="a1ca5-127">high</span></span>|<span data-ttu-id="a1ca5-128">2/4</span><span class="sxs-lookup"><span data-stu-id="a1ca5-128">4</span></span>|<span data-ttu-id="a1ca5-129">デバイスの脅威保護レベルの要件: High。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="a1ca5-130">High は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="a1ca5-131">notSet</span><span class="sxs-lookup"><span data-stu-id="a1ca5-131">notSet</span></span>|<span data-ttu-id="a1ca5-132">個</span><span class="sxs-lookup"><span data-stu-id="a1ca5-132">10</span></span>|<span data-ttu-id="a1ca5-133">デバイスの脅威保護レベルの要件: 設定されていません。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="a1ca5-134">Not set は、デバイスが脅威保護レベルを満たすための要件がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="a1ca5-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





