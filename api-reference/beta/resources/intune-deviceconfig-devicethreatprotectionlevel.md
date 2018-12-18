---
title: deviceThreatProtectionLevel 列挙型
description: デバイスの脅威保護 API のデバイスの脅威保護レベルです。
author: tfitzmac
ms.openlocfilehash: 8fdb336b60ad5f17bd5fcfb730c59238dbba55a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336009"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="48b14-103">deviceThreatProtectionLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="48b14-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="48b14-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="48b14-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48b14-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48b14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48b14-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="48b14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48b14-107">デバイスの脅威保護 API のデバイスの脅威保護レベルです。</span><span class="sxs-lookup"><span data-stu-id="48b14-107">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="48b14-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="48b14-108">Members</span></span>
|<span data-ttu-id="48b14-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="48b14-109">Member</span></span>|<span data-ttu-id="48b14-110">値</span><span class="sxs-lookup"><span data-stu-id="48b14-110">Value</span></span>|<span data-ttu-id="48b14-111">説明</span><span class="sxs-lookup"><span data-stu-id="48b14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48b14-112">利用不可</span><span class="sxs-lookup"><span data-stu-id="48b14-112">unavailable</span></span>|<span data-ttu-id="48b14-113">0</span><span class="sxs-lookup"><span data-stu-id="48b14-113">0</span></span>|<span data-ttu-id="48b14-114">既定値です。</span><span class="sxs-lookup"><span data-stu-id="48b14-114">Default Value.</span></span> <span data-ttu-id="48b14-115">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="48b14-115">Do not use.</span></span>|
|<span data-ttu-id="48b14-116">セキュリティで保護</span><span class="sxs-lookup"><span data-stu-id="48b14-116">secured</span></span>|<span data-ttu-id="48b14-117">1</span><span class="sxs-lookup"><span data-stu-id="48b14-117">1</span></span>|<span data-ttu-id="48b14-118">デバイスの脅威のレベルの要件: セキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="48b14-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="48b14-119">これは、最も安全なレベルであり、デバイス上の脅威が見つかりませんだったことを表します。</span><span class="sxs-lookup"><span data-stu-id="48b14-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="48b14-120">低</span><span class="sxs-lookup"><span data-stu-id="48b14-120">low</span></span>|<span data-ttu-id="48b14-121">2</span><span class="sxs-lookup"><span data-stu-id="48b14-121">2</span></span>|<span data-ttu-id="48b14-122">デバイスの脅威保護に必要なレベル: 低。</span><span class="sxs-lookup"><span data-stu-id="48b14-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="48b14-123">低は、デバイスまたはデバイスのデータに最小限のリスクをもたらす脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="48b14-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="48b14-124">medium</span><span class="sxs-lookup"><span data-stu-id="48b14-124">medium</span></span>|<span data-ttu-id="48b14-125">3</span><span class="sxs-lookup"><span data-stu-id="48b14-125">3</span></span>|<span data-ttu-id="48b14-126">デバイスの脅威保護に必要なレベル: 中。</span><span class="sxs-lookup"><span data-stu-id="48b14-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="48b14-127">[中] では、中程度のデバイスまたはデバイスのデータへのリスクをポーズする脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="48b14-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="48b14-128">高</span><span class="sxs-lookup"><span data-stu-id="48b14-128">high</span></span>|<span data-ttu-id="48b14-129">4</span><span class="sxs-lookup"><span data-stu-id="48b14-129">4</span></span>|<span data-ttu-id="48b14-130">デバイスの脅威保護に必要なレベル: 高。</span><span class="sxs-lookup"><span data-stu-id="48b14-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="48b14-131">高では、デバイスまたはデバイスのデータに重大なリスクをもたらす脅威の重大度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="48b14-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="48b14-132">notSet</span><span class="sxs-lookup"><span data-stu-id="48b14-132">notSet</span></span>|<span data-ttu-id="48b14-133">10</span><span class="sxs-lookup"><span data-stu-id="48b14-133">10</span></span>|<span data-ttu-id="48b14-134">デバイスの脅威保護に必要なレベル: 設定されていません。</span><span class="sxs-lookup"><span data-stu-id="48b14-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="48b14-135">セットはない、脅威保護のレベルを満たすためにデバイスの要件がないことです。</span><span class="sxs-lookup"><span data-stu-id="48b14-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





