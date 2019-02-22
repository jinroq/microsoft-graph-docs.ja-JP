---
title: managementagenttype 列挙型
description: 管理エージェントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb948626035bed2dac7ee18d103aa083bd0f2aeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172542"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="16c49-103">managementagenttype 列挙型</span><span class="sxs-lookup"><span data-stu-id="16c49-103">managementAgentType enum type</span></span>

> <span data-ttu-id="16c49-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16c49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16c49-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="16c49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16c49-106">管理エージェントの種類。</span><span class="sxs-lookup"><span data-stu-id="16c49-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="16c49-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="16c49-107">Members</span></span>
|<span data-ttu-id="16c49-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="16c49-108">Member</span></span>|<span data-ttu-id="16c49-109">値</span><span class="sxs-lookup"><span data-stu-id="16c49-109">Value</span></span>|<span data-ttu-id="16c49-110">説明</span><span class="sxs-lookup"><span data-stu-id="16c49-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16c49-111">eas</span><span class="sxs-lookup"><span data-stu-id="16c49-111">eas</span></span>|<span data-ttu-id="16c49-112">1-d</span><span class="sxs-lookup"><span data-stu-id="16c49-112">1</span></span>|<span data-ttu-id="16c49-113">デバイスは、Exchange server によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="16c49-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="16c49-114">mdm.exe</span><span class="sxs-lookup"><span data-stu-id="16c49-114">mdm</span></span>|<span data-ttu-id="16c49-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="16c49-115">2</span></span>|<span data-ttu-id="16c49-116">デバイスは Intune MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="16c49-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="16c49-117">easmdm</span><span class="sxs-lookup"><span data-stu-id="16c49-117">easMdm</span></span>|<span data-ttu-id="16c49-118">1/3</span><span class="sxs-lookup"><span data-stu-id="16c49-118">3</span></span>|<span data-ttu-id="16c49-119">デバイスは、Exchange server と Intune MDM の両方によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="16c49-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="16c49-120">intアンの場合</span><span class="sxs-lookup"><span data-stu-id="16c49-120">intuneClient</span></span>|<span data-ttu-id="16c49-121">2/4</span><span class="sxs-lookup"><span data-stu-id="16c49-121">4</span></span>|<span data-ttu-id="16c49-122">Intune クライアント管理。</span><span class="sxs-lookup"><span data-stu-id="16c49-122">Intune client managed.</span></span>|
|<span data-ttu-id="16c49-123">easintアンの場合</span><span class="sxs-lookup"><span data-stu-id="16c49-123">easIntuneClient</span></span>|<span data-ttu-id="16c49-124">5</span><span class="sxs-lookup"><span data-stu-id="16c49-124">5</span></span>|<span data-ttu-id="16c49-125">デバイスは EAS で、Intune クライアントはデュアル管理されています。</span><span class="sxs-lookup"><span data-stu-id="16c49-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="16c49-126">configurationmanagerclient</span><span class="sxs-lookup"><span data-stu-id="16c49-126">configurationManagerClient</span></span>|<span data-ttu-id="16c49-127">~</span><span class="sxs-lookup"><span data-stu-id="16c49-127">8</span></span>|<span data-ttu-id="16c49-128">デバイスは構成マネージャーによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="16c49-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="16c49-129">configurationmanagerclientmdm</span><span class="sxs-lookup"><span data-stu-id="16c49-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="16c49-130">個</span><span class="sxs-lookup"><span data-stu-id="16c49-130">10</span></span>|<span data-ttu-id="16c49-131">デバイスは、構成マネージャーおよび MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="16c49-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="16c49-132">configurationmanagerclientmdmeas</span><span class="sxs-lookup"><span data-stu-id="16c49-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="16c49-133">#</span><span class="sxs-lookup"><span data-stu-id="16c49-133">11</span></span>|<span data-ttu-id="16c49-134">デバイスは、構成マネージャー、MDM、Eas によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="16c49-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="16c49-135">不明</span><span class="sxs-lookup"><span data-stu-id="16c49-135">unknown</span></span>|<span data-ttu-id="16c49-136">16</span><span class="sxs-lookup"><span data-stu-id="16c49-136">16</span></span>|<span data-ttu-id="16c49-137">管理エージェントの種類が不明です。</span><span class="sxs-lookup"><span data-stu-id="16c49-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="16c49-138">jamf</span><span class="sxs-lookup"><span data-stu-id="16c49-138">jamf</span></span>|<span data-ttu-id="16c49-139">32</span><span class="sxs-lookup"><span data-stu-id="16c49-139">32</span></span>|<span data-ttu-id="16c49-140">デバイス属性は、Jamf から取得されます。</span><span class="sxs-lookup"><span data-stu-id="16c49-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="16c49-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="16c49-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="16c49-142">64</span><span class="sxs-lookup"><span data-stu-id="16c49-142">64</span></span>|<span data-ttu-id="16c49-143">デバイスは Google の CloudDPC によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="16c49-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="16c49-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="16c49-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="16c49-145">258</span><span class="sxs-lookup"><span data-stu-id="16c49-145">258</span></span>|<span data-ttu-id="16c49-146">このデバイスは、Microsoft 365 によって Intune によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="16c49-146">This device is managed by Microsoft 365 through Intune.</span></span>|




