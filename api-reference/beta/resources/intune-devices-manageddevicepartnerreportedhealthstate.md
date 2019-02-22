---
title: manageddevicepartnerreportedhealthstate 列挙型
description: デバイス正常性 API の利用可能な状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60a3071094e2667b896401c6df29977f9923884c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143772"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="36a63-103">manageddevicepartnerreportedhealthstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="36a63-103">managedDevicePartnerReportedHealthState enum type</span></span>

> <span data-ttu-id="36a63-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36a63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36a63-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36a63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a63-106">デバイス正常性 API の利用可能な状態</span><span class="sxs-lookup"><span data-stu-id="36a63-106">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="36a63-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="36a63-107">Members</span></span>
|<span data-ttu-id="36a63-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="36a63-108">Member</span></span>|<span data-ttu-id="36a63-109">値</span><span class="sxs-lookup"><span data-stu-id="36a63-109">Value</span></span>|<span data-ttu-id="36a63-110">説明</span><span class="sxs-lookup"><span data-stu-id="36a63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36a63-111">不明</span><span class="sxs-lookup"><span data-stu-id="36a63-111">unknown</span></span>|<span data-ttu-id="36a63-112">.0</span><span class="sxs-lookup"><span data-stu-id="36a63-112">0</span></span>|<span data-ttu-id="36a63-113">デバイス正常性状態はまだ報告されていません</span><span class="sxs-lookup"><span data-stu-id="36a63-113">Device health state is not yet reported</span></span>|
|<span data-ttu-id="36a63-114">アクティブ化</span><span class="sxs-lookup"><span data-stu-id="36a63-114">activated</span></span>|<span data-ttu-id="36a63-115">1-d</span><span class="sxs-lookup"><span data-stu-id="36a63-115">1</span></span>|<span data-ttu-id="36a63-116">デバイスは、モバイル脅威防衛パートナーによってアクティブ化されていますが、正常性を報告していません。</span><span class="sxs-lookup"><span data-stu-id="36a63-116">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="36a63-117">不可</span><span class="sxs-lookup"><span data-stu-id="36a63-117">deactivated</span></span>|<span data-ttu-id="36a63-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="36a63-118">2</span></span>|<span data-ttu-id="36a63-119">モバイル脅威防御パートナーによってデバイスが非アクティブ化されました。</span><span class="sxs-lookup"><span data-stu-id="36a63-119">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="36a63-120">デバイスの正常性が不明です。</span><span class="sxs-lookup"><span data-stu-id="36a63-120">The device health is not known.</span></span>|
|<span data-ttu-id="36a63-121">セキュリティ保護</span><span class="sxs-lookup"><span data-stu-id="36a63-121">secured</span></span>|<span data-ttu-id="36a63-122">1/3</span><span class="sxs-lookup"><span data-stu-id="36a63-122">3</span></span>|<span data-ttu-id="36a63-123">モバイル脅威防御パートナーによって、デバイスはセキュリティで保護されていると見なされます。</span><span class="sxs-lookup"><span data-stu-id="36a63-123">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="36a63-124">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="36a63-124">lowSeverity</span></span>|<span data-ttu-id="36a63-125">2/4</span><span class="sxs-lookup"><span data-stu-id="36a63-125">4</span></span>|<span data-ttu-id="36a63-126">モバイル脅威防御パートナーによって、デバイスの脅威は低いと見なされます。</span><span class="sxs-lookup"><span data-stu-id="36a63-126">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="36a63-127">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="36a63-127">mediumSeverity</span></span>|<span data-ttu-id="36a63-128">5</span><span class="sxs-lookup"><span data-stu-id="36a63-128">5</span></span>|<span data-ttu-id="36a63-129">モバイル脅威防御パートナーによって、デバイスは中程度の脅威と見なされます。</span><span class="sxs-lookup"><span data-stu-id="36a63-129">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="36a63-130">highSeverity</span><span class="sxs-lookup"><span data-stu-id="36a63-130">highSeverity</span></span>|<span data-ttu-id="36a63-131">シックス</span><span class="sxs-lookup"><span data-stu-id="36a63-131">6</span></span>|<span data-ttu-id="36a63-132">モバイル脅威防御パートナーによって、デバイスが高い脅威と見なされます。</span><span class="sxs-lookup"><span data-stu-id="36a63-132">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="36a63-133">なかっ</span><span class="sxs-lookup"><span data-stu-id="36a63-133">unresponsive</span></span>|<span data-ttu-id="36a63-134">7</span><span class="sxs-lookup"><span data-stu-id="36a63-134">7</span></span>|<span data-ttu-id="36a63-135">モバイル脅威防御パートナーによってデバイスが応答しないと見なされます。</span><span class="sxs-lookup"><span data-stu-id="36a63-135">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="36a63-136">デバイスの正常性が不明です。</span><span class="sxs-lookup"><span data-stu-id="36a63-136">The device health is not known.</span></span>|
|<span data-ttu-id="36a63-137">セキュリティ</span><span class="sxs-lookup"><span data-stu-id="36a63-137">compromised</span></span>|<span data-ttu-id="36a63-138">~</span><span class="sxs-lookup"><span data-stu-id="36a63-138">8</span></span>|<span data-ttu-id="36a63-139">脅威の防御パートナーによってデバイスが侵害されたと見なされます。</span><span class="sxs-lookup"><span data-stu-id="36a63-139">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="36a63-140">これは、デバイスのアクティブな脅威またはリスクが、エンドユーザーによって簡単に修復できず、ユーザーが IT 管理者に連絡する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="36a63-140">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="36a63-141">誤った</span><span class="sxs-lookup"><span data-stu-id="36a63-141">misconfigured</span></span>|<span data-ttu-id="36a63-142">i-9</span><span class="sxs-lookup"><span data-stu-id="36a63-142">9</span></span>|<span data-ttu-id="36a63-143">脅威の防御パートナーとの間でデバイスが正しく構成されていないと考えられます。</span><span class="sxs-lookup"><span data-stu-id="36a63-143">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="36a63-144">これは、脅威またはリスク分析が正常に機能するために必要なプロファイルまたは構成がデバイスにないことを意味します。そのため、脅威またはリスク分析を完了できません。</span><span class="sxs-lookup"><span data-stu-id="36a63-144">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|




