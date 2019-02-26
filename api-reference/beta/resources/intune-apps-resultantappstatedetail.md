---
title: resultの appstatedetail 列挙型
description: 列挙アプリケーションが特定のインストール状態を持っている理由に関する追加の詳細を示しています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d6b7e6a665229d02033cd1c0c25469a83dfc37d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167215"
---
# <a name="resultantappstatedetail-enum-type"></a><span data-ttu-id="46eec-103">resultの appstatedetail 列挙型</span><span class="sxs-lookup"><span data-stu-id="46eec-103">resultantAppStateDetail enum type</span></span>

> <span data-ttu-id="46eec-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46eec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46eec-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="46eec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46eec-106">列挙アプリケーションが特定のインストール状態を持っている理由に関する追加の詳細を示しています。</span><span class="sxs-lookup"><span data-stu-id="46eec-106">Enum indicating additional details regarding why an application has a particular install state.</span></span>

## <a name="members"></a><span data-ttu-id="46eec-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="46eec-107">Members</span></span>
|<span data-ttu-id="46eec-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="46eec-108">Member</span></span>|<span data-ttu-id="46eec-109">値</span><span class="sxs-lookup"><span data-stu-id="46eec-109">Value</span></span>|<span data-ttu-id="46eec-110">説明</span><span class="sxs-lookup"><span data-stu-id="46eec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46eec-111">noadditionaldetails</span><span class="sxs-lookup"><span data-stu-id="46eec-111">noAdditionalDetails</span></span>|<span data-ttu-id="46eec-112">.0</span><span class="sxs-lookup"><span data-stu-id="46eec-112">0</span></span>|<span data-ttu-id="46eec-113">追加の詳細情報は利用できません。</span><span class="sxs-lookup"><span data-stu-id="46eec-113">No additional details are available.</span></span>|
|<span data-ttu-id="46eec-114">参照 installerrorcode</span><span class="sxs-lookup"><span data-stu-id="46eec-114">seeInstallErrorCode</span></span>|<span data-ttu-id="46eec-115">2000</span><span class="sxs-lookup"><span data-stu-id="46eec-115">2000</span></span>|<span data-ttu-id="46eec-116">アプリケーションをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="46eec-116">Application failed to install.</span></span> <span data-ttu-id="46eec-117">詳細については、「エラーコードプロパティ」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46eec-117">See error code property for more details.</span></span>|
|<span data-ttu-id="46eec-118">未確認のエラーを参照</span><span class="sxs-lookup"><span data-stu-id="46eec-118">seeUninstallErrorCode</span></span>|<span data-ttu-id="46eec-119">4000</span><span class="sxs-lookup"><span data-stu-id="46eec-119">4000</span></span>|<span data-ttu-id="46eec-120">アプリケーションをアンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="46eec-120">Application failed to uninstall.</span></span> <span data-ttu-id="46eec-121">詳細については、「エラーコードプロパティ」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46eec-121">See error code property for more details.</span></span>|
|<span data-ttu-id="46eec-122">pendingreboot</span><span class="sxs-lookup"><span data-stu-id="46eec-122">pendingReboot</span></span>|<span data-ttu-id="46eec-123">5000</span><span class="sxs-lookup"><span data-stu-id="46eec-123">5000</span></span>|<span data-ttu-id="46eec-124">アプリケーションのインストールを完了するには、デバイスを再起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46eec-124">Device must be rebooted to complete installation of the application.</span></span>|
|<span data-ttu-id="46eec-125">platformnotapplicable</span><span class="sxs-lookup"><span data-stu-id="46eec-125">platformNotApplicable</span></span>|<span data-ttu-id="46eec-126">-1006</span><span class="sxs-lookup"><span data-stu-id="46eec-126">-1006</span></span>|<span data-ttu-id="46eec-127">アプリケーションはこのプラットフォームには適用できません。</span><span class="sxs-lookup"><span data-stu-id="46eec-127">Application is not applicable to this platform.</span></span> <span data-ttu-id="46eec-128">(IOS を対象とした Android アプリなど)</span><span class="sxs-lookup"><span data-stu-id="46eec-128">(e.g. Android app targeted to IOS)</span></span>|
|<span data-ttu-id="46eec-129">minimumcpuspeednotmet れている</span><span class="sxs-lookup"><span data-stu-id="46eec-129">minimumCpuSpeedNotMet</span></span>|<span data-ttu-id="46eec-130">-1005</span><span class="sxs-lookup"><span data-stu-id="46eec-130">-1005</span></span>|<span data-ttu-id="46eec-131">ターゲットデバイスの CPU 速度が構成されている最小値を下回っています。</span><span class="sxs-lookup"><span data-stu-id="46eec-131">CPU speed on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="46eec-132">minimumlogicalprocessorcountnotmet れた</span><span class="sxs-lookup"><span data-stu-id="46eec-132">minimumLogicalProcessorCountNotMet</span></span>|<span data-ttu-id="46eec-133">-1004</span><span class="sxs-lookup"><span data-stu-id="46eec-133">-1004</span></span>|<span data-ttu-id="46eec-134">ターゲットデバイス上の論理プロセッサ数が構成されている最小値を下回っています。</span><span class="sxs-lookup"><span data-stu-id="46eec-134">Count of logical processors on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="46eec-135">minimumphysicalmemorynotmet</span><span class="sxs-lookup"><span data-stu-id="46eec-135">minimumPhysicalMemoryNotMet</span></span>|<span data-ttu-id="46eec-136">-1003</span><span class="sxs-lookup"><span data-stu-id="46eec-136">-1003</span></span>|<span data-ttu-id="46eec-137">ターゲットデバイスの RAM の容量が構成されている最小値を下回っています。</span><span class="sxs-lookup"><span data-stu-id="46eec-137">Amount of RAM on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="46eec-138">minimumOsVersionNotMet</span><span class="sxs-lookup"><span data-stu-id="46eec-138">minimumOsVersionNotMet</span></span>|<span data-ttu-id="46eec-139">-1002</span><span class="sxs-lookup"><span data-stu-id="46eec-139">-1002</span></span>|<span data-ttu-id="46eec-140">ターゲットデバイスの OS のバージョンが、構成されている最小値を下回っています。</span><span class="sxs-lookup"><span data-stu-id="46eec-140">OS version on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="46eec-141">minimumdiskん enot満たさ</span><span class="sxs-lookup"><span data-stu-id="46eec-141">minimumDiskSpaceNotMet</span></span>|<span data-ttu-id="46eec-142">-1001</span><span class="sxs-lookup"><span data-stu-id="46eec-142">-1001</span></span>|<span data-ttu-id="46eec-143">ターゲットデバイスの使用可能なディスク領域が構成されている最小値を下回っています。</span><span class="sxs-lookup"><span data-stu-id="46eec-143">Available disk space on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="46eec-144">プロセッサアーキテクチャ (該当する場合)</span><span class="sxs-lookup"><span data-stu-id="46eec-144">processorArchitectureNotApplicable</span></span>|<span data-ttu-id="46eec-145">-1000</span><span class="sxs-lookup"><span data-stu-id="46eec-145">-1000</span></span>|<span data-ttu-id="46eec-146">デバイスアーキテクチャ (x86/amd64 など) は、アプリケーションには適用されません。</span><span class="sxs-lookup"><span data-stu-id="46eec-146">Device architecture (e.g. x86/amd64) is not applicable for the application.</span></span>|




