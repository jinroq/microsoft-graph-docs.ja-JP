---
title: deviceThreatProtectionLevel 列挙型
description: デバイス脅威保護 API のデバイスの脅威保護レベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1af0231e15cfa815d3fd2e154adf180f3e0c0c43
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253296"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="33c9a-103">deviceThreatProtectionLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="33c9a-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="33c9a-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33c9a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33c9a-105">デバイス脅威保護 API のデバイスの脅威保護レベル。</span><span class="sxs-lookup"><span data-stu-id="33c9a-105">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="33c9a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="33c9a-106">Members</span></span>
|<span data-ttu-id="33c9a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="33c9a-107">Member</span></span>|<span data-ttu-id="33c9a-108">値</span><span class="sxs-lookup"><span data-stu-id="33c9a-108">Value</span></span>|<span data-ttu-id="33c9a-109">説明</span><span class="sxs-lookup"><span data-stu-id="33c9a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33c9a-110">無効</span><span class="sxs-lookup"><span data-stu-id="33c9a-110">unavailable</span></span>|<span data-ttu-id="33c9a-111">.0</span><span class="sxs-lookup"><span data-stu-id="33c9a-111">0</span></span>|<span data-ttu-id="33c9a-112">既定値です。</span><span class="sxs-lookup"><span data-stu-id="33c9a-112">Default Value.</span></span> <span data-ttu-id="33c9a-113">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="33c9a-113">Do not use.</span></span>|
|<span data-ttu-id="33c9a-114">セキュリティ保護</span><span class="sxs-lookup"><span data-stu-id="33c9a-114">secured</span></span>|<span data-ttu-id="33c9a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="33c9a-115">1</span></span>|<span data-ttu-id="33c9a-116">デバイスの脅威レベルの要件: セキュリティで保護されています。</span><span class="sxs-lookup"><span data-stu-id="33c9a-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="33c9a-117">これは最も安全なレベルで、デバイス上に脅威が何も検出されなかったことを表します。</span><span class="sxs-lookup"><span data-stu-id="33c9a-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="33c9a-118">低さ</span><span class="sxs-lookup"><span data-stu-id="33c9a-118">low</span></span>|<span data-ttu-id="33c9a-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="33c9a-119">2</span></span>|<span data-ttu-id="33c9a-120">デバイスの脅威保護レベルの要件: 低。</span><span class="sxs-lookup"><span data-stu-id="33c9a-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="33c9a-121">Low は、デバイスまたはデバイスのデータに対するリスクを最小限に抑える脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="33c9a-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="33c9a-122">medium</span><span class="sxs-lookup"><span data-stu-id="33c9a-122">medium</span></span>|<span data-ttu-id="33c9a-123">1/3</span><span class="sxs-lookup"><span data-stu-id="33c9a-123">3</span></span>|<span data-ttu-id="33c9a-124">デバイスの脅威保護レベルの要件: 中。</span><span class="sxs-lookup"><span data-stu-id="33c9a-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="33c9a-125">Medium は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="33c9a-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="33c9a-126">高額</span><span class="sxs-lookup"><span data-stu-id="33c9a-126">high</span></span>|<span data-ttu-id="33c9a-127">2/4</span><span class="sxs-lookup"><span data-stu-id="33c9a-127">4</span></span>|<span data-ttu-id="33c9a-128">デバイスの脅威保護レベルの要件: High。</span><span class="sxs-lookup"><span data-stu-id="33c9a-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="33c9a-129">High は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="33c9a-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="33c9a-130">notSet</span><span class="sxs-lookup"><span data-stu-id="33c9a-130">notSet</span></span>|<span data-ttu-id="33c9a-131">個</span><span class="sxs-lookup"><span data-stu-id="33c9a-131">10</span></span>|<span data-ttu-id="33c9a-132">デバイスの脅威保護レベルの要件: 設定されていません。</span><span class="sxs-lookup"><span data-stu-id="33c9a-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="33c9a-133">Not set は、デバイスが脅威保護レベルを満たすための要件がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="33c9a-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



