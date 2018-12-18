---
title: managementAgentType 列挙型
description: 管理エージェントの種類です。
author: tfitzmac
ms.openlocfilehash: 702f71f3984bda34e31d0a614e45e387f45b587e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321589"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="05d19-103">managementAgentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="05d19-103">managementAgentType enum type</span></span>

> <span data-ttu-id="05d19-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05d19-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05d19-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05d19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05d19-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="05d19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05d19-107">管理エージェントの種類です。</span><span class="sxs-lookup"><span data-stu-id="05d19-107">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="05d19-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="05d19-108">Members</span></span>
|<span data-ttu-id="05d19-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="05d19-109">Member</span></span>|<span data-ttu-id="05d19-110">値</span><span class="sxs-lookup"><span data-stu-id="05d19-110">Value</span></span>|<span data-ttu-id="05d19-111">説明</span><span class="sxs-lookup"><span data-stu-id="05d19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05d19-112">ea</span><span class="sxs-lookup"><span data-stu-id="05d19-112">eas</span></span>|<span data-ttu-id="05d19-113">1</span><span class="sxs-lookup"><span data-stu-id="05d19-113">1</span></span>|<span data-ttu-id="05d19-114">デバイスは、Exchange サーバーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="05d19-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="05d19-115">mdm</span><span class="sxs-lookup"><span data-stu-id="05d19-115">mdm</span></span>|<span data-ttu-id="05d19-116">2</span><span class="sxs-lookup"><span data-stu-id="05d19-116">2</span></span>|<span data-ttu-id="05d19-117">Intune MDM. で、デバイスを管理します。</span><span class="sxs-lookup"><span data-stu-id="05d19-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="05d19-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="05d19-118">easMdm</span></span>|<span data-ttu-id="05d19-119">3</span><span class="sxs-lookup"><span data-stu-id="05d19-119">3</span></span>|<span data-ttu-id="05d19-120">Intune MDM. と Exchange サーバーの両方がデバイス管理します。</span><span class="sxs-lookup"><span data-stu-id="05d19-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="05d19-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="05d19-121">intuneClient</span></span>|<span data-ttu-id="05d19-122">4</span><span class="sxs-lookup"><span data-stu-id="05d19-122">4</span></span>|<span data-ttu-id="05d19-123">Intune クライアントが管理されています。</span><span class="sxs-lookup"><span data-stu-id="05d19-123">Intune client managed.</span></span>|
|<span data-ttu-id="05d19-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="05d19-124">easIntuneClient</span></span>|<span data-ttu-id="05d19-125">5</span><span class="sxs-lookup"><span data-stu-id="05d19-125">5</span></span>|<span data-ttu-id="05d19-126">デバイスは、EA と Intune クライアント デュアル管理です。</span><span class="sxs-lookup"><span data-stu-id="05d19-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="05d19-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="05d19-127">configurationManagerClient</span></span>|<span data-ttu-id="05d19-128">8</span><span class="sxs-lookup"><span data-stu-id="05d19-128">8</span></span>|<span data-ttu-id="05d19-129">デバイスは、構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="05d19-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="05d19-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="05d19-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="05d19-131">10</span><span class="sxs-lookup"><span data-stu-id="05d19-131">10</span></span>|<span data-ttu-id="05d19-132">デバイスの管理は、構成マネージャーと MDM.</span><span class="sxs-lookup"><span data-stu-id="05d19-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="05d19-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="05d19-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="05d19-134">11</span><span class="sxs-lookup"><span data-stu-id="05d19-134">11</span></span>|<span data-ttu-id="05d19-135">デバイスは、MDM および Ea は、構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="05d19-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="05d19-136">不明</span><span class="sxs-lookup"><span data-stu-id="05d19-136">unknown</span></span>|<span data-ttu-id="05d19-137">16</span><span class="sxs-lookup"><span data-stu-id="05d19-137">16</span></span>|<span data-ttu-id="05d19-138">不明な管理エージェントの種類です。</span><span class="sxs-lookup"><span data-stu-id="05d19-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="05d19-139">jamf</span><span class="sxs-lookup"><span data-stu-id="05d19-139">jamf</span></span>|<span data-ttu-id="05d19-140">32</span><span class="sxs-lookup"><span data-stu-id="05d19-140">32</span></span>|<span data-ttu-id="05d19-141">デバイス属性は、Jamf からフェッチされます。</span><span class="sxs-lookup"><span data-stu-id="05d19-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="05d19-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="05d19-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="05d19-143">64</span><span class="sxs-lookup"><span data-stu-id="05d19-143">64</span></span>|<span data-ttu-id="05d19-144">デバイスは、Google の CloudDPC によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="05d19-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="05d19-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="05d19-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="05d19-146">258</span><span class="sxs-lookup"><span data-stu-id="05d19-146">258</span></span>|<span data-ttu-id="05d19-147">Intune によって Microsoft 365 では、このデバイスが管理されます。</span><span class="sxs-lookup"><span data-stu-id="05d19-147">This device is managed by Microsoft 365 through Intune.</span></span>|





