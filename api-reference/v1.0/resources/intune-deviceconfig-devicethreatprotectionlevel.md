---
title: deviceThreatProtectionLevel 列挙型
description: デバイスの脅威保護 API のデバイスの脅威保護レベルです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa287d9259ed88f1b2240fd9bbdcaf77bcf9170e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850583"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="9e48f-103">deviceThreatProtectionLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="9e48f-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="9e48f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e48f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e48f-105">デバイスの脅威保護 API のデバイスの脅威保護レベルです。</span><span class="sxs-lookup"><span data-stu-id="9e48f-105">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="9e48f-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e48f-106">Members</span></span>
|<span data-ttu-id="9e48f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e48f-107">Member</span></span>|<span data-ttu-id="9e48f-108">値</span><span class="sxs-lookup"><span data-stu-id="9e48f-108">Value</span></span>|<span data-ttu-id="9e48f-109">説明</span><span class="sxs-lookup"><span data-stu-id="9e48f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e48f-110">利用不可</span><span class="sxs-lookup"><span data-stu-id="9e48f-110">unavailable</span></span>|<span data-ttu-id="9e48f-111">0</span><span class="sxs-lookup"><span data-stu-id="9e48f-111">0</span></span>|<span data-ttu-id="9e48f-112">既定値です。</span><span class="sxs-lookup"><span data-stu-id="9e48f-112">Default Value.</span></span> <span data-ttu-id="9e48f-113">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="9e48f-113">Do not use.</span></span>|
|<span data-ttu-id="9e48f-114">セキュリティで保護</span><span class="sxs-lookup"><span data-stu-id="9e48f-114">secured</span></span>|<span data-ttu-id="9e48f-115">1</span><span class="sxs-lookup"><span data-stu-id="9e48f-115">1</span></span>|<span data-ttu-id="9e48f-116">デバイスの脅威のレベルの要件: セキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="9e48f-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="9e48f-117">これは、最も安全なレベルであり、デバイス上の脅威が見つかりませんだったことを表します。</span><span class="sxs-lookup"><span data-stu-id="9e48f-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="9e48f-118">低</span><span class="sxs-lookup"><span data-stu-id="9e48f-118">low</span></span>|<span data-ttu-id="9e48f-119">2</span><span class="sxs-lookup"><span data-stu-id="9e48f-119">2</span></span>|<span data-ttu-id="9e48f-120">デバイスの脅威保護に必要なレベル: 低。</span><span class="sxs-lookup"><span data-stu-id="9e48f-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="9e48f-121">低は、デバイスまたはデバイスのデータに最小限のリスクをもたらす脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="9e48f-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="9e48f-122">medium</span><span class="sxs-lookup"><span data-stu-id="9e48f-122">medium</span></span>|<span data-ttu-id="9e48f-123">3</span><span class="sxs-lookup"><span data-stu-id="9e48f-123">3</span></span>|<span data-ttu-id="9e48f-124">デバイスの脅威保護に必要なレベル: 中。</span><span class="sxs-lookup"><span data-stu-id="9e48f-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="9e48f-125">[中] では、中程度のデバイスまたはデバイスのデータへのリスクをポーズする脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="9e48f-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="9e48f-126">高</span><span class="sxs-lookup"><span data-stu-id="9e48f-126">high</span></span>|<span data-ttu-id="9e48f-127">4</span><span class="sxs-lookup"><span data-stu-id="9e48f-127">4</span></span>|<span data-ttu-id="9e48f-128">デバイスの脅威保護に必要なレベル: 高。</span><span class="sxs-lookup"><span data-stu-id="9e48f-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="9e48f-129">高では、デバイスまたはデバイスのデータに重大なリスクをもたらす脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="9e48f-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="9e48f-130">notSet</span><span class="sxs-lookup"><span data-stu-id="9e48f-130">notSet</span></span>|<span data-ttu-id="9e48f-131">10</span><span class="sxs-lookup"><span data-stu-id="9e48f-131">10</span></span>|<span data-ttu-id="9e48f-132">デバイスの脅威保護に必要なレベル: 設定されていません。</span><span class="sxs-lookup"><span data-stu-id="9e48f-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="9e48f-133">セットはない、脅威保護のレベルを満たすためにデバイスの要件がないことです。</span><span class="sxs-lookup"><span data-stu-id="9e48f-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



