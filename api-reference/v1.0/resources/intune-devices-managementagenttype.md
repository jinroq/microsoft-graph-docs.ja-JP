---
title: managementagenttype 列挙型
description: 管理エージェントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522714"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="c4256-103">managementagenttype 列挙型</span><span class="sxs-lookup"><span data-stu-id="c4256-103">managementAgentType enum type</span></span>

> <span data-ttu-id="c4256-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4256-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4256-105">管理エージェントの種類。</span><span class="sxs-lookup"><span data-stu-id="c4256-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="c4256-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4256-106">Members</span></span>
|<span data-ttu-id="c4256-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4256-107">Member</span></span>|<span data-ttu-id="c4256-108">値</span><span class="sxs-lookup"><span data-stu-id="c4256-108">Value</span></span>|<span data-ttu-id="c4256-109">説明</span><span class="sxs-lookup"><span data-stu-id="c4256-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4256-110">eas</span><span class="sxs-lookup"><span data-stu-id="c4256-110">eas</span></span>|<span data-ttu-id="c4256-111">1 </span><span class="sxs-lookup"><span data-stu-id="c4256-111">1</span></span>|<span data-ttu-id="c4256-112">デバイスは、Exchange server によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="c4256-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="c4256-113">mdm.exe</span><span class="sxs-lookup"><span data-stu-id="c4256-113">mdm</span></span>|<span data-ttu-id="c4256-114">2 </span><span class="sxs-lookup"><span data-stu-id="c4256-114">2</span></span>|<span data-ttu-id="c4256-115">デバイスは Intune MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="c4256-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="c4256-116">easmdm</span><span class="sxs-lookup"><span data-stu-id="c4256-116">easMdm</span></span>|<span data-ttu-id="c4256-117">3 </span><span class="sxs-lookup"><span data-stu-id="c4256-117">3</span></span>|<span data-ttu-id="c4256-118">デバイスは、Exchange server と Intune MDM の両方によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="c4256-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="c4256-119">intアンの場合</span><span class="sxs-lookup"><span data-stu-id="c4256-119">intuneClient</span></span>|<span data-ttu-id="c4256-120">4 </span><span class="sxs-lookup"><span data-stu-id="c4256-120">4</span></span>|<span data-ttu-id="c4256-121">Intune クライアント管理。</span><span class="sxs-lookup"><span data-stu-id="c4256-121">Intune client managed.</span></span>|
|<span data-ttu-id="c4256-122">easintアンの場合</span><span class="sxs-lookup"><span data-stu-id="c4256-122">easIntuneClient</span></span>|<span data-ttu-id="c4256-123">5 </span><span class="sxs-lookup"><span data-stu-id="c4256-123">5</span></span>|<span data-ttu-id="c4256-124">デバイスは EAS で、Intune クライアントはデュアル管理されています。</span><span class="sxs-lookup"><span data-stu-id="c4256-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="c4256-125">configurationmanagerclient</span><span class="sxs-lookup"><span data-stu-id="c4256-125">configurationManagerClient</span></span>|<span data-ttu-id="c4256-126">8 </span><span class="sxs-lookup"><span data-stu-id="c4256-126">8</span></span>|<span data-ttu-id="c4256-127">デバイスは構成マネージャーによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="c4256-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="c4256-128">configurationmanagerclientmdm</span><span class="sxs-lookup"><span data-stu-id="c4256-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="c4256-129">10  </span><span class="sxs-lookup"><span data-stu-id="c4256-129">10</span></span>|<span data-ttu-id="c4256-130">デバイスは、構成マネージャーおよび MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="c4256-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="c4256-131">configurationmanagerclientmdmeas</span><span class="sxs-lookup"><span data-stu-id="c4256-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="c4256-132">11 </span><span class="sxs-lookup"><span data-stu-id="c4256-132">11</span></span>|<span data-ttu-id="c4256-133">デバイスは、構成マネージャー、MDM、Eas によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="c4256-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="c4256-134">不明</span><span class="sxs-lookup"><span data-stu-id="c4256-134">unknown</span></span>|<span data-ttu-id="c4256-135">16 </span><span class="sxs-lookup"><span data-stu-id="c4256-135">16</span></span>|<span data-ttu-id="c4256-136">管理エージェントの種類が不明です。</span><span class="sxs-lookup"><span data-stu-id="c4256-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="c4256-137">jamf</span><span class="sxs-lookup"><span data-stu-id="c4256-137">jamf</span></span>|<span data-ttu-id="c4256-138">32</span><span class="sxs-lookup"><span data-stu-id="c4256-138">32</span></span>|<span data-ttu-id="c4256-139">デバイス属性は、Jamf から取得されます。</span><span class="sxs-lookup"><span data-stu-id="c4256-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="c4256-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="c4256-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="c4256-141">64</span><span class="sxs-lookup"><span data-stu-id="c4256-141">64</span></span>|<span data-ttu-id="c4256-142">デバイスは Google の CloudDPC によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="c4256-142">The device is managed by Google's CloudDPC.</span></span>|



