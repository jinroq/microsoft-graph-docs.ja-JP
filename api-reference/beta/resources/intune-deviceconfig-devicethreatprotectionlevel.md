---
title: deviceThreatProtectionLevel 列挙型
description: デバイスの脅威保護 API のデバイスの脅威保護レベルです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38d4c17fc9883b23417a4c72ac7cc3c75512865c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948052"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="c8566-103">deviceThreatProtectionLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="c8566-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="c8566-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8566-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8566-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8566-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8566-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8566-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8566-107">デバイスの脅威保護 API のデバイスの脅威保護レベルです。</span><span class="sxs-lookup"><span data-stu-id="c8566-107">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="c8566-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c8566-108">Members</span></span>
|<span data-ttu-id="c8566-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c8566-109">Member</span></span>|<span data-ttu-id="c8566-110">値</span><span class="sxs-lookup"><span data-stu-id="c8566-110">Value</span></span>|<span data-ttu-id="c8566-111">説明</span><span class="sxs-lookup"><span data-stu-id="c8566-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8566-112">利用不可</span><span class="sxs-lookup"><span data-stu-id="c8566-112">unavailable</span></span>|<span data-ttu-id="c8566-113">0</span><span class="sxs-lookup"><span data-stu-id="c8566-113">0</span></span>|<span data-ttu-id="c8566-114">既定値です。</span><span class="sxs-lookup"><span data-stu-id="c8566-114">Default Value.</span></span> <span data-ttu-id="c8566-115">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="c8566-115">Do not use.</span></span>|
|<span data-ttu-id="c8566-116">セキュリティで保護</span><span class="sxs-lookup"><span data-stu-id="c8566-116">secured</span></span>|<span data-ttu-id="c8566-117">1</span><span class="sxs-lookup"><span data-stu-id="c8566-117">1</span></span>|<span data-ttu-id="c8566-118">デバイスの脅威のレベルの要件: セキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="c8566-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="c8566-119">これは、最も安全なレベルであり、デバイス上の脅威が見つかりませんだったことを表します。</span><span class="sxs-lookup"><span data-stu-id="c8566-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="c8566-120">低</span><span class="sxs-lookup"><span data-stu-id="c8566-120">low</span></span>|<span data-ttu-id="c8566-121">2</span><span class="sxs-lookup"><span data-stu-id="c8566-121">2</span></span>|<span data-ttu-id="c8566-122">デバイスの脅威保護に必要なレベル: 低。</span><span class="sxs-lookup"><span data-stu-id="c8566-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="c8566-123">低は、デバイスまたはデバイスのデータに最小限のリスクをもたらす脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="c8566-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="c8566-124">medium</span><span class="sxs-lookup"><span data-stu-id="c8566-124">medium</span></span>|<span data-ttu-id="c8566-125">3</span><span class="sxs-lookup"><span data-stu-id="c8566-125">3</span></span>|<span data-ttu-id="c8566-126">デバイスの脅威保護に必要なレベル: 中。</span><span class="sxs-lookup"><span data-stu-id="c8566-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="c8566-127">[中] では、中程度のデバイスまたはデバイスのデータへのリスクをポーズする脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="c8566-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="c8566-128">高</span><span class="sxs-lookup"><span data-stu-id="c8566-128">high</span></span>|<span data-ttu-id="c8566-129">4</span><span class="sxs-lookup"><span data-stu-id="c8566-129">4</span></span>|<span data-ttu-id="c8566-130">デバイスの脅威保護に必要なレベル: 高。</span><span class="sxs-lookup"><span data-stu-id="c8566-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="c8566-131">高では、デバイスまたはデバイスのデータに重大なリスクをもたらす脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="c8566-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="c8566-132">notSet</span><span class="sxs-lookup"><span data-stu-id="c8566-132">notSet</span></span>|<span data-ttu-id="c8566-133">10</span><span class="sxs-lookup"><span data-stu-id="c8566-133">10</span></span>|<span data-ttu-id="c8566-134">デバイスの脅威保護に必要なレベル: 設定されていません。</span><span class="sxs-lookup"><span data-stu-id="c8566-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="c8566-135">セットはない、脅威保護のレベルを満たすためにデバイスの要件がないことです。</span><span class="sxs-lookup"><span data-stu-id="c8566-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





