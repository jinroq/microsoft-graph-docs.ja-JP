---
title: manageddevicepartnerreportedhealthstate 列挙型
description: デバイス正常性 API の利用可能な状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04ed30c087bb9f607f1579819d09def103658ca3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521272"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="5b606-103">manageddevicepartnerreportedhealthstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="5b606-103">managedDevicePartnerReportedHealthState enum type</span></span>

> <span data-ttu-id="5b606-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b606-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b606-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b606-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b606-106">デバイス正常性 API の利用可能な状態</span><span class="sxs-lookup"><span data-stu-id="5b606-106">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="5b606-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5b606-107">Members</span></span>
|<span data-ttu-id="5b606-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5b606-108">Member</span></span>|<span data-ttu-id="5b606-109">値</span><span class="sxs-lookup"><span data-stu-id="5b606-109">Value</span></span>|<span data-ttu-id="5b606-110">説明</span><span class="sxs-lookup"><span data-stu-id="5b606-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b606-111">不明</span><span class="sxs-lookup"><span data-stu-id="5b606-111">unknown</span></span>|<span data-ttu-id="5b606-112">.0</span><span class="sxs-lookup"><span data-stu-id="5b606-112">0</span></span>|<span data-ttu-id="5b606-113">デバイス正常性状態はまだ報告されていません</span><span class="sxs-lookup"><span data-stu-id="5b606-113">Device health state is not yet reported</span></span>|
|<span data-ttu-id="5b606-114">アクティブ化</span><span class="sxs-lookup"><span data-stu-id="5b606-114">activated</span></span>|<span data-ttu-id="5b606-115">1 </span><span class="sxs-lookup"><span data-stu-id="5b606-115">1</span></span>|<span data-ttu-id="5b606-116">デバイスは、モバイル脅威防衛パートナーによってアクティブ化されていますが、正常性を報告していません。</span><span class="sxs-lookup"><span data-stu-id="5b606-116">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="5b606-117">不可</span><span class="sxs-lookup"><span data-stu-id="5b606-117">deactivated</span></span>|<span data-ttu-id="5b606-118">2 </span><span class="sxs-lookup"><span data-stu-id="5b606-118">2</span></span>|<span data-ttu-id="5b606-119">モバイル脅威防御パートナーによってデバイスが非アクティブ化されました。</span><span class="sxs-lookup"><span data-stu-id="5b606-119">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="5b606-120">デバイスの正常性が不明です。</span><span class="sxs-lookup"><span data-stu-id="5b606-120">The device health is not known.</span></span>|
|<span data-ttu-id="5b606-121">セキュリティ保護</span><span class="sxs-lookup"><span data-stu-id="5b606-121">secured</span></span>|<span data-ttu-id="5b606-122">3 </span><span class="sxs-lookup"><span data-stu-id="5b606-122">3</span></span>|<span data-ttu-id="5b606-123">モバイル脅威防御パートナーによって、デバイスはセキュリティで保護されていると見なされます。</span><span class="sxs-lookup"><span data-stu-id="5b606-123">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="5b606-124">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="5b606-124">lowSeverity</span></span>|<span data-ttu-id="5b606-125">4 </span><span class="sxs-lookup"><span data-stu-id="5b606-125">4</span></span>|<span data-ttu-id="5b606-126">モバイル脅威防御パートナーによって、デバイスの脅威は低いと見なされます。</span><span class="sxs-lookup"><span data-stu-id="5b606-126">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="5b606-127">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="5b606-127">mediumSeverity</span></span>|<span data-ttu-id="5b606-128">5 </span><span class="sxs-lookup"><span data-stu-id="5b606-128">5</span></span>|<span data-ttu-id="5b606-129">モバイル脅威防御パートナーによって、デバイスは中程度の脅威と見なされます。</span><span class="sxs-lookup"><span data-stu-id="5b606-129">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="5b606-130">highSeverity</span><span class="sxs-lookup"><span data-stu-id="5b606-130">highSeverity</span></span>|<span data-ttu-id="5b606-131">6 </span><span class="sxs-lookup"><span data-stu-id="5b606-131">6</span></span>|<span data-ttu-id="5b606-132">モバイル脅威防御パートナーによって、デバイスが高い脅威と見なされます。</span><span class="sxs-lookup"><span data-stu-id="5b606-132">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="5b606-133">なかっ</span><span class="sxs-lookup"><span data-stu-id="5b606-133">unresponsive</span></span>|<span data-ttu-id="5b606-134">7 </span><span class="sxs-lookup"><span data-stu-id="5b606-134">7</span></span>|<span data-ttu-id="5b606-135">モバイル脅威防御パートナーによってデバイスが応答しないと見なされます。</span><span class="sxs-lookup"><span data-stu-id="5b606-135">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="5b606-136">デバイスの正常性が不明です。</span><span class="sxs-lookup"><span data-stu-id="5b606-136">The device health is not known.</span></span>|
|<span data-ttu-id="5b606-137">セキュリティ</span><span class="sxs-lookup"><span data-stu-id="5b606-137">compromised</span></span>|<span data-ttu-id="5b606-138">8 </span><span class="sxs-lookup"><span data-stu-id="5b606-138">8</span></span>|<span data-ttu-id="5b606-139">脅威の防御パートナーによってデバイスが侵害されたと見なされます。</span><span class="sxs-lookup"><span data-stu-id="5b606-139">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="5b606-140">これは、デバイスのアクティブな脅威またはリスクが、エンドユーザーによって簡単に修復できず、ユーザーが IT 管理者に連絡する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="5b606-140">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="5b606-141">誤った</span><span class="sxs-lookup"><span data-stu-id="5b606-141">misconfigured</span></span>|<span data-ttu-id="5b606-142">9 </span><span class="sxs-lookup"><span data-stu-id="5b606-142">9</span></span>|<span data-ttu-id="5b606-143">脅威の防御パートナーとの間でデバイスが正しく構成されていないと考えられます。</span><span class="sxs-lookup"><span data-stu-id="5b606-143">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="5b606-144">これは、脅威またはリスク分析が正常に機能するために必要なプロファイルまたは構成がデバイスにないことを意味します。そのため、脅威またはリスク分析を完了できません。</span><span class="sxs-lookup"><span data-stu-id="5b606-144">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|





