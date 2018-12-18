---
title: managementAgentType 列挙型
description: 管理エージェントの種類です。
author: tfitzmac
ms.openlocfilehash: b1f6db6eaea1a488831bec3d7ff61d6170414956
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355518"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="84737-103">managementAgentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="84737-103">managementAgentType enum type</span></span>

> <span data-ttu-id="84737-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="84737-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84737-105">管理エージェントの種類です。</span><span class="sxs-lookup"><span data-stu-id="84737-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="84737-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="84737-106">Members</span></span>
|<span data-ttu-id="84737-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="84737-107">Member</span></span>|<span data-ttu-id="84737-108">値</span><span class="sxs-lookup"><span data-stu-id="84737-108">Value</span></span>|<span data-ttu-id="84737-109">説明</span><span class="sxs-lookup"><span data-stu-id="84737-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84737-110">ea</span><span class="sxs-lookup"><span data-stu-id="84737-110">eas</span></span>|<span data-ttu-id="84737-111">1</span><span class="sxs-lookup"><span data-stu-id="84737-111">1</span></span>|<span data-ttu-id="84737-112">デバイスは、Exchange サーバーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="84737-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="84737-113">mdm</span><span class="sxs-lookup"><span data-stu-id="84737-113">mdm</span></span>|<span data-ttu-id="84737-114">2</span><span class="sxs-lookup"><span data-stu-id="84737-114">2</span></span>|<span data-ttu-id="84737-115">Intune MDM. で、デバイスを管理します。</span><span class="sxs-lookup"><span data-stu-id="84737-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="84737-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="84737-116">easMdm</span></span>|<span data-ttu-id="84737-117">3</span><span class="sxs-lookup"><span data-stu-id="84737-117">3</span></span>|<span data-ttu-id="84737-118">Intune MDM. と Exchange サーバーの両方がデバイス管理します。</span><span class="sxs-lookup"><span data-stu-id="84737-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="84737-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="84737-119">intuneClient</span></span>|<span data-ttu-id="84737-120">4</span><span class="sxs-lookup"><span data-stu-id="84737-120">4</span></span>|<span data-ttu-id="84737-121">Intune クライアントが管理されています。</span><span class="sxs-lookup"><span data-stu-id="84737-121">Intune client managed.</span></span>|
|<span data-ttu-id="84737-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="84737-122">easIntuneClient</span></span>|<span data-ttu-id="84737-123">5</span><span class="sxs-lookup"><span data-stu-id="84737-123">5</span></span>|<span data-ttu-id="84737-124">デバイスは、EA と Intune クライアント デュアル管理です。</span><span class="sxs-lookup"><span data-stu-id="84737-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="84737-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="84737-125">configurationManagerClient</span></span>|<span data-ttu-id="84737-126">8</span><span class="sxs-lookup"><span data-stu-id="84737-126">8</span></span>|<span data-ttu-id="84737-127">デバイスは、構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="84737-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="84737-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="84737-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="84737-129">10</span><span class="sxs-lookup"><span data-stu-id="84737-129">10</span></span>|<span data-ttu-id="84737-130">デバイスの管理は、構成マネージャーと MDM.</span><span class="sxs-lookup"><span data-stu-id="84737-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="84737-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="84737-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="84737-132">11</span><span class="sxs-lookup"><span data-stu-id="84737-132">11</span></span>|<span data-ttu-id="84737-133">デバイスは、MDM および Ea は、構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="84737-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="84737-134">不明</span><span class="sxs-lookup"><span data-stu-id="84737-134">unknown</span></span>|<span data-ttu-id="84737-135">16</span><span class="sxs-lookup"><span data-stu-id="84737-135">16</span></span>|<span data-ttu-id="84737-136">不明な管理エージェントの種類です。</span><span class="sxs-lookup"><span data-stu-id="84737-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="84737-137">jamf</span><span class="sxs-lookup"><span data-stu-id="84737-137">jamf</span></span>|<span data-ttu-id="84737-138">32</span><span class="sxs-lookup"><span data-stu-id="84737-138">32</span></span>|<span data-ttu-id="84737-139">デバイス属性は、Jamf からフェッチされます。</span><span class="sxs-lookup"><span data-stu-id="84737-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="84737-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="84737-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="84737-141">64</span><span class="sxs-lookup"><span data-stu-id="84737-141">64</span></span>|<span data-ttu-id="84737-142">デバイスは、Google の CloudDPC によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="84737-142">The device is managed by Google's CloudDPC.</span></span>|



