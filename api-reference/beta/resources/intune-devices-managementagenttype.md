---
title: managementagenttype 列挙型
description: 管理エージェントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf8a40b8d6951c13da49766430fdd7fb303cbba0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775304"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="73075-103">managementagenttype 列挙型</span><span class="sxs-lookup"><span data-stu-id="73075-103">managementAgentType enum type</span></span>

> <span data-ttu-id="73075-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73075-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73075-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="73075-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73075-106">管理エージェントの種類。</span><span class="sxs-lookup"><span data-stu-id="73075-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="73075-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="73075-107">Members</span></span>
|<span data-ttu-id="73075-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="73075-108">Member</span></span>|<span data-ttu-id="73075-109">値</span><span class="sxs-lookup"><span data-stu-id="73075-109">Value</span></span>|<span data-ttu-id="73075-110">説明</span><span class="sxs-lookup"><span data-stu-id="73075-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73075-111">eas</span><span class="sxs-lookup"><span data-stu-id="73075-111">eas</span></span>|<span data-ttu-id="73075-112">1-d</span><span class="sxs-lookup"><span data-stu-id="73075-112">1</span></span>|<span data-ttu-id="73075-113">デバイスは、Exchange server によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="73075-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="73075-114">mdm.exe</span><span class="sxs-lookup"><span data-stu-id="73075-114">mdm</span></span>|<span data-ttu-id="73075-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="73075-115">2</span></span>|<span data-ttu-id="73075-116">デバイスは Intune MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="73075-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="73075-117">easmdm</span><span class="sxs-lookup"><span data-stu-id="73075-117">easMdm</span></span>|<span data-ttu-id="73075-118">1/3</span><span class="sxs-lookup"><span data-stu-id="73075-118">3</span></span>|<span data-ttu-id="73075-119">デバイスは、Exchange server と Intune MDM の両方によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="73075-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="73075-120">intアンの場合</span><span class="sxs-lookup"><span data-stu-id="73075-120">intuneClient</span></span>|<span data-ttu-id="73075-121">2/4</span><span class="sxs-lookup"><span data-stu-id="73075-121">4</span></span>|<span data-ttu-id="73075-122">Intune クライアント管理。</span><span class="sxs-lookup"><span data-stu-id="73075-122">Intune client managed.</span></span>|
|<span data-ttu-id="73075-123">easintアンの場合</span><span class="sxs-lookup"><span data-stu-id="73075-123">easIntuneClient</span></span>|<span data-ttu-id="73075-124">5</span><span class="sxs-lookup"><span data-stu-id="73075-124">5</span></span>|<span data-ttu-id="73075-125">デバイスは EAS で、Intune クライアントはデュアル管理されています。</span><span class="sxs-lookup"><span data-stu-id="73075-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="73075-126">configurationmanagerclient</span><span class="sxs-lookup"><span data-stu-id="73075-126">configurationManagerClient</span></span>|<span data-ttu-id="73075-127">~</span><span class="sxs-lookup"><span data-stu-id="73075-127">8</span></span>|<span data-ttu-id="73075-128">デバイスは構成マネージャーによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="73075-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="73075-129">configurationmanagerclientmdm</span><span class="sxs-lookup"><span data-stu-id="73075-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="73075-130">個</span><span class="sxs-lookup"><span data-stu-id="73075-130">10</span></span>|<span data-ttu-id="73075-131">デバイスは、構成マネージャーおよび MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="73075-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="73075-132">configurationmanagerclientmdmeas</span><span class="sxs-lookup"><span data-stu-id="73075-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="73075-133">#</span><span class="sxs-lookup"><span data-stu-id="73075-133">11</span></span>|<span data-ttu-id="73075-134">デバイスは、構成マネージャー、MDM、Eas によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="73075-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="73075-135">不明</span><span class="sxs-lookup"><span data-stu-id="73075-135">unknown</span></span>|<span data-ttu-id="73075-136">16</span><span class="sxs-lookup"><span data-stu-id="73075-136">16</span></span>|<span data-ttu-id="73075-137">管理エージェントの種類が不明です。</span><span class="sxs-lookup"><span data-stu-id="73075-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="73075-138">jamf</span><span class="sxs-lookup"><span data-stu-id="73075-138">jamf</span></span>|<span data-ttu-id="73075-139">32</span><span class="sxs-lookup"><span data-stu-id="73075-139">32</span></span>|<span data-ttu-id="73075-140">デバイス属性は、Jamf から取得されます。</span><span class="sxs-lookup"><span data-stu-id="73075-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="73075-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="73075-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="73075-142">64</span><span class="sxs-lookup"><span data-stu-id="73075-142">64</span></span>|<span data-ttu-id="73075-143">デバイスは Google の CloudDPC によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="73075-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="73075-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="73075-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="73075-145">258</span><span class="sxs-lookup"><span data-stu-id="73075-145">258</span></span>|<span data-ttu-id="73075-146">このデバイスは、Microsoft 365 によって Intune によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="73075-146">This device is managed by Microsoft 365 through Intune.</span></span>|





