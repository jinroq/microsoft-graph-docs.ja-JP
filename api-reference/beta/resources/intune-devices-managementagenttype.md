---
title: managementAgentType 列挙型
description: 管理エージェントの種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401006"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="ad237-103">managementAgentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ad237-103">managementAgentType enum type</span></span>

> <span data-ttu-id="ad237-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad237-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ad237-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad237-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad237-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad237-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad237-107">管理エージェントの種類です。</span><span class="sxs-lookup"><span data-stu-id="ad237-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="ad237-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ad237-108">Members</span></span>
|<span data-ttu-id="ad237-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ad237-109">Member</span></span>|<span data-ttu-id="ad237-110">値</span><span class="sxs-lookup"><span data-stu-id="ad237-110">Value</span></span>|<span data-ttu-id="ad237-111">説明</span><span class="sxs-lookup"><span data-stu-id="ad237-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad237-112">ea</span><span class="sxs-lookup"><span data-stu-id="ad237-112">eas</span></span>|<span data-ttu-id="ad237-113">1</span><span class="sxs-lookup"><span data-stu-id="ad237-113">1</span></span>|<span data-ttu-id="ad237-114">デバイスは、Exchange サーバーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="ad237-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="ad237-115">mdm</span><span class="sxs-lookup"><span data-stu-id="ad237-115">mdm</span></span>|<span data-ttu-id="ad237-116">2</span><span class="sxs-lookup"><span data-stu-id="ad237-116">2</span></span>|<span data-ttu-id="ad237-117">Intune MDM. で、デバイスを管理します。</span><span class="sxs-lookup"><span data-stu-id="ad237-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="ad237-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="ad237-118">easMdm</span></span>|<span data-ttu-id="ad237-119">3</span><span class="sxs-lookup"><span data-stu-id="ad237-119">3</span></span>|<span data-ttu-id="ad237-120">Intune MDM. と Exchange サーバーの両方がデバイス管理します。</span><span class="sxs-lookup"><span data-stu-id="ad237-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="ad237-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="ad237-121">intuneClient</span></span>|<span data-ttu-id="ad237-122">4</span><span class="sxs-lookup"><span data-stu-id="ad237-122">4</span></span>|<span data-ttu-id="ad237-123">Intune クライアントが管理されています。</span><span class="sxs-lookup"><span data-stu-id="ad237-123">Intune client managed.</span></span>|
|<span data-ttu-id="ad237-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="ad237-124">easIntuneClient</span></span>|<span data-ttu-id="ad237-125">5</span><span class="sxs-lookup"><span data-stu-id="ad237-125">5</span></span>|<span data-ttu-id="ad237-126">デバイスは、EA と Intune クライアント デュアル管理です。</span><span class="sxs-lookup"><span data-stu-id="ad237-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="ad237-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="ad237-127">configurationManagerClient</span></span>|<span data-ttu-id="ad237-128">8</span><span class="sxs-lookup"><span data-stu-id="ad237-128">8</span></span>|<span data-ttu-id="ad237-129">デバイスは、構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="ad237-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="ad237-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="ad237-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="ad237-131">10</span><span class="sxs-lookup"><span data-stu-id="ad237-131">10</span></span>|<span data-ttu-id="ad237-132">デバイスの管理は、構成マネージャーと MDM.</span><span class="sxs-lookup"><span data-stu-id="ad237-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="ad237-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="ad237-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="ad237-134">11</span><span class="sxs-lookup"><span data-stu-id="ad237-134">11</span></span>|<span data-ttu-id="ad237-135">デバイスは、MDM および Ea は、構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="ad237-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="ad237-136">不明</span><span class="sxs-lookup"><span data-stu-id="ad237-136">unknown</span></span>|<span data-ttu-id="ad237-137">16</span><span class="sxs-lookup"><span data-stu-id="ad237-137">16</span></span>|<span data-ttu-id="ad237-138">不明な管理エージェントの種類です。</span><span class="sxs-lookup"><span data-stu-id="ad237-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="ad237-139">jamf</span><span class="sxs-lookup"><span data-stu-id="ad237-139">jamf</span></span>|<span data-ttu-id="ad237-140">32</span><span class="sxs-lookup"><span data-stu-id="ad237-140">32</span></span>|<span data-ttu-id="ad237-141">デバイス属性は、Jamf からフェッチされます。</span><span class="sxs-lookup"><span data-stu-id="ad237-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="ad237-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="ad237-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="ad237-143">64</span><span class="sxs-lookup"><span data-stu-id="ad237-143">64</span></span>|<span data-ttu-id="ad237-144">デバイスは、Google の CloudDPC によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="ad237-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="ad237-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="ad237-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="ad237-146">258</span><span class="sxs-lookup"><span data-stu-id="ad237-146">258</span></span>|<span data-ttu-id="ad237-147">Intune によって Microsoft 365 では、このデバイスが管理されます。</span><span class="sxs-lookup"><span data-stu-id="ad237-147">This device is managed by Microsoft 365 through Intune.</span></span>|




