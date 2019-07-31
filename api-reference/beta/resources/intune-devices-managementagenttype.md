---
title: managementAgentType 列挙型
description: 管理エージェントの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ae96113e687d406f5c0342b3b71fd63ea6de9918
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999753"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="f2d68-103">managementAgentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f2d68-103">managementAgentType enum type</span></span>

> <span data-ttu-id="f2d68-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2d68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2d68-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2d68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2d68-106">管理エージェントの種類。</span><span class="sxs-lookup"><span data-stu-id="f2d68-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="f2d68-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2d68-107">Members</span></span>
|<span data-ttu-id="f2d68-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2d68-108">Member</span></span>|<span data-ttu-id="f2d68-109">値</span><span class="sxs-lookup"><span data-stu-id="f2d68-109">Value</span></span>|<span data-ttu-id="f2d68-110">説明</span><span class="sxs-lookup"><span data-stu-id="f2d68-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2d68-111">eas</span><span class="sxs-lookup"><span data-stu-id="f2d68-111">eas</span></span>|<span data-ttu-id="f2d68-112">1-d</span><span class="sxs-lookup"><span data-stu-id="f2d68-112">1</span></span>|<span data-ttu-id="f2d68-113">デバイスは、Exchange server によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="f2d68-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="f2d68-114">mdm.exe</span><span class="sxs-lookup"><span data-stu-id="f2d68-114">mdm</span></span>|<span data-ttu-id="f2d68-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f2d68-115">2</span></span>|<span data-ttu-id="f2d68-116">デバイスは Intune MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="f2d68-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="f2d68-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="f2d68-117">easMdm</span></span>|<span data-ttu-id="f2d68-118">1/3</span><span class="sxs-lookup"><span data-stu-id="f2d68-118">3</span></span>|<span data-ttu-id="f2d68-119">デバイスは、Exchange server と Intune MDM の両方によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="f2d68-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="f2d68-120">Intアンの場合</span><span class="sxs-lookup"><span data-stu-id="f2d68-120">intuneClient</span></span>|<span data-ttu-id="f2d68-121">2/4</span><span class="sxs-lookup"><span data-stu-id="f2d68-121">4</span></span>|<span data-ttu-id="f2d68-122">Intune クライアント管理。</span><span class="sxs-lookup"><span data-stu-id="f2d68-122">Intune client managed.</span></span>|
|<span data-ttu-id="f2d68-123">Easintアンの場合</span><span class="sxs-lookup"><span data-stu-id="f2d68-123">easIntuneClient</span></span>|<span data-ttu-id="f2d68-124">5</span><span class="sxs-lookup"><span data-stu-id="f2d68-124">5</span></span>|<span data-ttu-id="f2d68-125">デバイスは EAS で、Intune クライアントはデュアル管理されています。</span><span class="sxs-lookup"><span data-stu-id="f2d68-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="f2d68-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="f2d68-126">configurationManagerClient</span></span>|<span data-ttu-id="f2d68-127">8 </span><span class="sxs-lookup"><span data-stu-id="f2d68-127">8</span></span>|<span data-ttu-id="f2d68-128">デバイスは構成マネージャーによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="f2d68-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="f2d68-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="f2d68-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="f2d68-130">10 </span><span class="sxs-lookup"><span data-stu-id="f2d68-130">10</span></span>|<span data-ttu-id="f2d68-131">デバイスは、構成マネージャーおよび MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="f2d68-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="f2d68-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="f2d68-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="f2d68-133">#</span><span class="sxs-lookup"><span data-stu-id="f2d68-133">11</span></span>|<span data-ttu-id="f2d68-134">デバイスは、構成マネージャー、MDM、Eas によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="f2d68-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="f2d68-135">不明</span><span class="sxs-lookup"><span data-stu-id="f2d68-135">unknown</span></span>|<span data-ttu-id="f2d68-136">16</span><span class="sxs-lookup"><span data-stu-id="f2d68-136">16</span></span>|<span data-ttu-id="f2d68-137">管理エージェントの種類が不明です。</span><span class="sxs-lookup"><span data-stu-id="f2d68-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="f2d68-138">jamf</span><span class="sxs-lookup"><span data-stu-id="f2d68-138">jamf</span></span>|<span data-ttu-id="f2d68-139">32</span><span class="sxs-lookup"><span data-stu-id="f2d68-139">32</span></span>|<span data-ttu-id="f2d68-140">デバイス属性は、Jamf から取得されます。</span><span class="sxs-lookup"><span data-stu-id="f2d68-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="f2d68-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="f2d68-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="f2d68-142">64</span><span class="sxs-lookup"><span data-stu-id="f2d68-142">64</span></span>|<span data-ttu-id="f2d68-143">デバイスは Google の CloudDPC によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="f2d68-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="f2d68-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="f2d68-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="f2d68-145">258</span><span class="sxs-lookup"><span data-stu-id="f2d68-145">258</span></span>|<span data-ttu-id="f2d68-146">このデバイスは、Microsoft 365 によって Intune によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="f2d68-146">This device is managed by Microsoft 365 through Intune.</span></span>|





