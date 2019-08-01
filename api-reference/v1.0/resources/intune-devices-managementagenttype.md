---
title: managementAgentType 列挙型
description: 管理エージェントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b1aabb6b3e08abdd3230eaab6ef5d640f4f908fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027441"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="7dbea-103">managementAgentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7dbea-103">managementAgentType enum type</span></span>

> <span data-ttu-id="7dbea-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7dbea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dbea-105">管理エージェントの種類。</span><span class="sxs-lookup"><span data-stu-id="7dbea-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="7dbea-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="7dbea-106">Members</span></span>
|<span data-ttu-id="7dbea-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7dbea-107">Member</span></span>|<span data-ttu-id="7dbea-108">値</span><span class="sxs-lookup"><span data-stu-id="7dbea-108">Value</span></span>|<span data-ttu-id="7dbea-109">説明</span><span class="sxs-lookup"><span data-stu-id="7dbea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dbea-110">eas</span><span class="sxs-lookup"><span data-stu-id="7dbea-110">eas</span></span>|<span data-ttu-id="7dbea-111">1-d</span><span class="sxs-lookup"><span data-stu-id="7dbea-111">1</span></span>|<span data-ttu-id="7dbea-112">デバイスは、Exchange server によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="7dbea-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="7dbea-113">mdm.exe</span><span class="sxs-lookup"><span data-stu-id="7dbea-113">mdm</span></span>|<span data-ttu-id="7dbea-114">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7dbea-114">2</span></span>|<span data-ttu-id="7dbea-115">デバイスは Intune MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="7dbea-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="7dbea-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="7dbea-116">easMdm</span></span>|<span data-ttu-id="7dbea-117">1/3</span><span class="sxs-lookup"><span data-stu-id="7dbea-117">3</span></span>|<span data-ttu-id="7dbea-118">デバイスは、Exchange server と Intune MDM の両方によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="7dbea-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="7dbea-119">Intアンの場合</span><span class="sxs-lookup"><span data-stu-id="7dbea-119">intuneClient</span></span>|<span data-ttu-id="7dbea-120">2/4</span><span class="sxs-lookup"><span data-stu-id="7dbea-120">4</span></span>|<span data-ttu-id="7dbea-121">Intune クライアント管理。</span><span class="sxs-lookup"><span data-stu-id="7dbea-121">Intune client managed.</span></span>|
|<span data-ttu-id="7dbea-122">Easintアンの場合</span><span class="sxs-lookup"><span data-stu-id="7dbea-122">easIntuneClient</span></span>|<span data-ttu-id="7dbea-123">5</span><span class="sxs-lookup"><span data-stu-id="7dbea-123">5</span></span>|<span data-ttu-id="7dbea-124">デバイスは EAS で、Intune クライアントはデュアル管理されています。</span><span class="sxs-lookup"><span data-stu-id="7dbea-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="7dbea-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="7dbea-125">configurationManagerClient</span></span>|<span data-ttu-id="7dbea-126">8 </span><span class="sxs-lookup"><span data-stu-id="7dbea-126">8</span></span>|<span data-ttu-id="7dbea-127">デバイスは構成マネージャーによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="7dbea-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="7dbea-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="7dbea-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="7dbea-129">10 </span><span class="sxs-lookup"><span data-stu-id="7dbea-129">10</span></span>|<span data-ttu-id="7dbea-130">デバイスは、構成マネージャーおよび MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="7dbea-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="7dbea-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="7dbea-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="7dbea-132">#</span><span class="sxs-lookup"><span data-stu-id="7dbea-132">11</span></span>|<span data-ttu-id="7dbea-133">デバイスは、構成マネージャー、MDM、Eas によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="7dbea-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="7dbea-134">不明</span><span class="sxs-lookup"><span data-stu-id="7dbea-134">unknown</span></span>|<span data-ttu-id="7dbea-135">16</span><span class="sxs-lookup"><span data-stu-id="7dbea-135">16</span></span>|<span data-ttu-id="7dbea-136">管理エージェントの種類が不明です。</span><span class="sxs-lookup"><span data-stu-id="7dbea-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="7dbea-137">jamf</span><span class="sxs-lookup"><span data-stu-id="7dbea-137">jamf</span></span>|<span data-ttu-id="7dbea-138">32</span><span class="sxs-lookup"><span data-stu-id="7dbea-138">32</span></span>|<span data-ttu-id="7dbea-139">デバイス属性は、Jamf から取得されます。</span><span class="sxs-lookup"><span data-stu-id="7dbea-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="7dbea-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="7dbea-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="7dbea-141">64</span><span class="sxs-lookup"><span data-stu-id="7dbea-141">64</span></span>|<span data-ttu-id="7dbea-142">デバイスは Google の CloudDPC によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="7dbea-142">The device is managed by Google's CloudDPC.</span></span>|



