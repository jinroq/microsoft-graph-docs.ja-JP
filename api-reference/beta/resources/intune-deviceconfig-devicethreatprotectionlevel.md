---
title: deviceThreatProtectionLevel 列挙型
description: デバイスの脅威保護 API のデバイスの脅威保護レベルです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4c9bbc599d424b91d07339a7a7cdad90b84c262
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411233"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="da579-103">deviceThreatProtectionLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="da579-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="da579-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da579-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da579-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da579-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da579-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da579-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da579-107">デバイスの脅威保護 API のデバイスの脅威保護レベルです。</span><span class="sxs-lookup"><span data-stu-id="da579-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="da579-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="da579-108">Members</span></span>
|<span data-ttu-id="da579-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="da579-109">Member</span></span>|<span data-ttu-id="da579-110">値</span><span class="sxs-lookup"><span data-stu-id="da579-110">Value</span></span>|<span data-ttu-id="da579-111">説明</span><span class="sxs-lookup"><span data-stu-id="da579-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da579-112">利用不可</span><span class="sxs-lookup"><span data-stu-id="da579-112">unavailable</span></span>|<span data-ttu-id="da579-113">0</span><span class="sxs-lookup"><span data-stu-id="da579-113">0</span></span>|<span data-ttu-id="da579-114">既定値です。</span><span class="sxs-lookup"><span data-stu-id="da579-114">Default Value.</span></span> <span data-ttu-id="da579-115">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="da579-115">Do not use.</span></span>|
|<span data-ttu-id="da579-116">セキュリティで保護</span><span class="sxs-lookup"><span data-stu-id="da579-116">secured</span></span>|<span data-ttu-id="da579-117">1</span><span class="sxs-lookup"><span data-stu-id="da579-117">1</span></span>|<span data-ttu-id="da579-118">デバイスの脅威のレベルの要件: セキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="da579-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="da579-119">これは、最も安全なレベルであり、デバイス上の脅威が見つかりませんだったことを表します。</span><span class="sxs-lookup"><span data-stu-id="da579-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="da579-120">低</span><span class="sxs-lookup"><span data-stu-id="da579-120">low</span></span>|<span data-ttu-id="da579-121">2</span><span class="sxs-lookup"><span data-stu-id="da579-121">2</span></span>|<span data-ttu-id="da579-122">デバイスの脅威保護に必要なレベル: 低。</span><span class="sxs-lookup"><span data-stu-id="da579-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="da579-123">低は、デバイスまたはデバイスのデータに最小限のリスクをもたらす脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="da579-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="da579-124">medium</span><span class="sxs-lookup"><span data-stu-id="da579-124">medium</span></span>|<span data-ttu-id="da579-125">3</span><span class="sxs-lookup"><span data-stu-id="da579-125">3</span></span>|<span data-ttu-id="da579-126">デバイスの脅威保護に必要なレベル: 中。</span><span class="sxs-lookup"><span data-stu-id="da579-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="da579-127">[中] では、中程度のデバイスまたはデバイスのデータへのリスクをポーズする脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="da579-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="da579-128">高</span><span class="sxs-lookup"><span data-stu-id="da579-128">high</span></span>|<span data-ttu-id="da579-129">4</span><span class="sxs-lookup"><span data-stu-id="da579-129">4</span></span>|<span data-ttu-id="da579-130">デバイスの脅威保護に必要なレベル: 高。</span><span class="sxs-lookup"><span data-stu-id="da579-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="da579-131">高では、デバイスまたはデバイスのデータに重大なリスクをもたらす脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="da579-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="da579-132">notSet</span><span class="sxs-lookup"><span data-stu-id="da579-132">notSet</span></span>|<span data-ttu-id="da579-133">10</span><span class="sxs-lookup"><span data-stu-id="da579-133">10</span></span>|<span data-ttu-id="da579-134">デバイスの脅威保護に必要なレベル: 設定されていません。</span><span class="sxs-lookup"><span data-stu-id="da579-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="da579-135">セットはない、脅威保護のレベルを満たすためにデバイスの要件がないことです。</span><span class="sxs-lookup"><span data-stu-id="da579-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




