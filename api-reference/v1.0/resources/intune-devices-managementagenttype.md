---
title: managementagenttype 列挙型
description: 管理エージェントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251567"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="594ce-103">managementagenttype 列挙型</span><span class="sxs-lookup"><span data-stu-id="594ce-103">managementAgentType enum type</span></span>

> <span data-ttu-id="594ce-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="594ce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="594ce-105">管理エージェントの種類。</span><span class="sxs-lookup"><span data-stu-id="594ce-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="594ce-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="594ce-106">Members</span></span>
|<span data-ttu-id="594ce-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="594ce-107">Member</span></span>|<span data-ttu-id="594ce-108">値</span><span class="sxs-lookup"><span data-stu-id="594ce-108">Value</span></span>|<span data-ttu-id="594ce-109">説明</span><span class="sxs-lookup"><span data-stu-id="594ce-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="594ce-110">eas</span><span class="sxs-lookup"><span data-stu-id="594ce-110">eas</span></span>|<span data-ttu-id="594ce-111">1-d</span><span class="sxs-lookup"><span data-stu-id="594ce-111">1</span></span>|<span data-ttu-id="594ce-112">デバイスは、Exchange server によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="594ce-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="594ce-113">mdm.exe</span><span class="sxs-lookup"><span data-stu-id="594ce-113">mdm</span></span>|<span data-ttu-id="594ce-114">pbm-2</span><span class="sxs-lookup"><span data-stu-id="594ce-114">2</span></span>|<span data-ttu-id="594ce-115">デバイスは Intune MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="594ce-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="594ce-116">easmdm</span><span class="sxs-lookup"><span data-stu-id="594ce-116">easMdm</span></span>|<span data-ttu-id="594ce-117">1/3</span><span class="sxs-lookup"><span data-stu-id="594ce-117">3</span></span>|<span data-ttu-id="594ce-118">デバイスは、Exchange server と Intune MDM の両方によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="594ce-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="594ce-119">intアンの場合</span><span class="sxs-lookup"><span data-stu-id="594ce-119">intuneClient</span></span>|<span data-ttu-id="594ce-120">2/4</span><span class="sxs-lookup"><span data-stu-id="594ce-120">4</span></span>|<span data-ttu-id="594ce-121">Intune クライアント管理。</span><span class="sxs-lookup"><span data-stu-id="594ce-121">Intune client managed.</span></span>|
|<span data-ttu-id="594ce-122">easintアンの場合</span><span class="sxs-lookup"><span data-stu-id="594ce-122">easIntuneClient</span></span>|<span data-ttu-id="594ce-123">5</span><span class="sxs-lookup"><span data-stu-id="594ce-123">5</span></span>|<span data-ttu-id="594ce-124">デバイスは EAS で、Intune クライアントはデュアル管理されています。</span><span class="sxs-lookup"><span data-stu-id="594ce-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="594ce-125">configurationmanagerclient</span><span class="sxs-lookup"><span data-stu-id="594ce-125">configurationManagerClient</span></span>|<span data-ttu-id="594ce-126">~</span><span class="sxs-lookup"><span data-stu-id="594ce-126">8</span></span>|<span data-ttu-id="594ce-127">デバイスは構成マネージャーによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="594ce-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="594ce-128">configurationmanagerclientmdm</span><span class="sxs-lookup"><span data-stu-id="594ce-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="594ce-129">個</span><span class="sxs-lookup"><span data-stu-id="594ce-129">10</span></span>|<span data-ttu-id="594ce-130">デバイスは、構成マネージャーおよび MDM によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="594ce-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="594ce-131">configurationmanagerclientmdmeas</span><span class="sxs-lookup"><span data-stu-id="594ce-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="594ce-132">#</span><span class="sxs-lookup"><span data-stu-id="594ce-132">11</span></span>|<span data-ttu-id="594ce-133">デバイスは、構成マネージャー、MDM、Eas によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="594ce-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="594ce-134">不明</span><span class="sxs-lookup"><span data-stu-id="594ce-134">unknown</span></span>|<span data-ttu-id="594ce-135">16</span><span class="sxs-lookup"><span data-stu-id="594ce-135">16</span></span>|<span data-ttu-id="594ce-136">管理エージェントの種類が不明です。</span><span class="sxs-lookup"><span data-stu-id="594ce-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="594ce-137">jamf</span><span class="sxs-lookup"><span data-stu-id="594ce-137">jamf</span></span>|<span data-ttu-id="594ce-138">32</span><span class="sxs-lookup"><span data-stu-id="594ce-138">32</span></span>|<span data-ttu-id="594ce-139">デバイス属性は、Jamf から取得されます。</span><span class="sxs-lookup"><span data-stu-id="594ce-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="594ce-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="594ce-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="594ce-141">64</span><span class="sxs-lookup"><span data-stu-id="594ce-141">64</span></span>|<span data-ttu-id="594ce-142">デバイスは Google の CloudDPC によって管理されています。</span><span class="sxs-lookup"><span data-stu-id="594ce-142">The device is managed by Google's CloudDPC.</span></span>|



