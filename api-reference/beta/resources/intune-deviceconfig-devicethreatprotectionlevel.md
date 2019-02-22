---
title: deviceThreatProtectionLevel 列挙型
description: デバイス脅威保護 API のデバイスの脅威保護レベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ecdf54051b1545b842cbc3c49359b9a77f12e2e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140244"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="ddfaa-103">deviceThreatProtectionLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="ddfaa-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="ddfaa-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddfaa-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddfaa-106">デバイス脅威保護 API のデバイスの脅威保護レベル。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="ddfaa-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ddfaa-107">Members</span></span>
|<span data-ttu-id="ddfaa-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ddfaa-108">Member</span></span>|<span data-ttu-id="ddfaa-109">値</span><span class="sxs-lookup"><span data-stu-id="ddfaa-109">Value</span></span>|<span data-ttu-id="ddfaa-110">説明</span><span class="sxs-lookup"><span data-stu-id="ddfaa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddfaa-111">無効</span><span class="sxs-lookup"><span data-stu-id="ddfaa-111">unavailable</span></span>|<span data-ttu-id="ddfaa-112">.0</span><span class="sxs-lookup"><span data-stu-id="ddfaa-112">0</span></span>|<span data-ttu-id="ddfaa-113">既定値です。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-113">Default Value.</span></span> <span data-ttu-id="ddfaa-114">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-114">Do not use.</span></span>|
|<span data-ttu-id="ddfaa-115">セキュリティ保護</span><span class="sxs-lookup"><span data-stu-id="ddfaa-115">secured</span></span>|<span data-ttu-id="ddfaa-116">1-d</span><span class="sxs-lookup"><span data-stu-id="ddfaa-116">1</span></span>|<span data-ttu-id="ddfaa-117">デバイスの脅威レベルの要件: セキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="ddfaa-118">これは最も安全なレベルで、デバイス上に脅威が何も検出されなかったことを表します。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="ddfaa-119">低さ</span><span class="sxs-lookup"><span data-stu-id="ddfaa-119">low</span></span>|<span data-ttu-id="ddfaa-120">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ddfaa-120">2</span></span>|<span data-ttu-id="ddfaa-121">デバイスの脅威保護レベルの要件: 低。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="ddfaa-122">Low は、デバイスまたはデバイスのデータに対するリスクを最小限に抑える脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="ddfaa-123">medium</span><span class="sxs-lookup"><span data-stu-id="ddfaa-123">medium</span></span>|<span data-ttu-id="ddfaa-124">1/3</span><span class="sxs-lookup"><span data-stu-id="ddfaa-124">3</span></span>|<span data-ttu-id="ddfaa-125">デバイスの脅威保護レベルの要件: 中。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="ddfaa-126">Medium は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="ddfaa-127">高額</span><span class="sxs-lookup"><span data-stu-id="ddfaa-127">high</span></span>|<span data-ttu-id="ddfaa-128">2/4</span><span class="sxs-lookup"><span data-stu-id="ddfaa-128">4</span></span>|<span data-ttu-id="ddfaa-129">デバイスの脅威保護レベルの要件: High。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="ddfaa-130">High は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="ddfaa-131">notSet</span><span class="sxs-lookup"><span data-stu-id="ddfaa-131">notSet</span></span>|<span data-ttu-id="ddfaa-132">個</span><span class="sxs-lookup"><span data-stu-id="ddfaa-132">10</span></span>|<span data-ttu-id="ddfaa-133">デバイスの脅威保護レベルの要件: 設定されていません。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="ddfaa-134">Not set は、デバイスが脅威保護レベルを満たすための要件がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="ddfaa-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




