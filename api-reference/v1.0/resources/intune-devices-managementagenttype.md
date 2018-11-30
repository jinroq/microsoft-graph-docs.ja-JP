---
title: managementAgentType 列挙型
description: 管理エージェントの種類です。
ms.openlocfilehash: de837f712f69576ea7a862101d2cfaa30b8685d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022630"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="61b9d-103">managementAgentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="61b9d-103">managementAgentType enum type</span></span>

> <span data-ttu-id="61b9d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="61b9d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61b9d-105">管理エージェントの種類です。</span><span class="sxs-lookup"><span data-stu-id="61b9d-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="61b9d-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="61b9d-106">Members</span></span>
|<span data-ttu-id="61b9d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="61b9d-107">Member</span></span>|<span data-ttu-id="61b9d-108">値</span><span class="sxs-lookup"><span data-stu-id="61b9d-108">Value</span></span>|<span data-ttu-id="61b9d-109">説明</span><span class="sxs-lookup"><span data-stu-id="61b9d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61b9d-110">ea</span><span class="sxs-lookup"><span data-stu-id="61b9d-110">eas</span></span>|<span data-ttu-id="61b9d-111">1</span><span class="sxs-lookup"><span data-stu-id="61b9d-111">1</span></span>|<span data-ttu-id="61b9d-112">デバイスは、Exchange サーバーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="61b9d-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="61b9d-113">mdm</span><span class="sxs-lookup"><span data-stu-id="61b9d-113">mdm</span></span>|<span data-ttu-id="61b9d-114">2</span><span class="sxs-lookup"><span data-stu-id="61b9d-114">2</span></span>|<span data-ttu-id="61b9d-115">Intune MDM. で、デバイスを管理します。</span><span class="sxs-lookup"><span data-stu-id="61b9d-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="61b9d-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="61b9d-116">easMdm</span></span>|<span data-ttu-id="61b9d-117">3</span><span class="sxs-lookup"><span data-stu-id="61b9d-117">3</span></span>|<span data-ttu-id="61b9d-118">Intune MDM. と Exchange サーバーの両方がデバイス管理します。</span><span class="sxs-lookup"><span data-stu-id="61b9d-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="61b9d-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="61b9d-119">intuneClient</span></span>|<span data-ttu-id="61b9d-120">4</span><span class="sxs-lookup"><span data-stu-id="61b9d-120">4</span></span>|<span data-ttu-id="61b9d-121">Intune クライアントが管理されています。</span><span class="sxs-lookup"><span data-stu-id="61b9d-121">Intune client managed.</span></span>|
|<span data-ttu-id="61b9d-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="61b9d-122">easIntuneClient</span></span>|<span data-ttu-id="61b9d-123">5</span><span class="sxs-lookup"><span data-stu-id="61b9d-123">5</span></span>|<span data-ttu-id="61b9d-124">デバイスは、EA と Intune クライアント デュアル管理です。</span><span class="sxs-lookup"><span data-stu-id="61b9d-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="61b9d-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="61b9d-125">configurationManagerClient</span></span>|<span data-ttu-id="61b9d-126">8</span><span class="sxs-lookup"><span data-stu-id="61b9d-126">8</span></span>|<span data-ttu-id="61b9d-127">デバイスは、構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="61b9d-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="61b9d-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="61b9d-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="61b9d-129">10</span><span class="sxs-lookup"><span data-stu-id="61b9d-129">10</span></span>|<span data-ttu-id="61b9d-130">デバイスの管理は、構成マネージャーと MDM.</span><span class="sxs-lookup"><span data-stu-id="61b9d-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="61b9d-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="61b9d-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="61b9d-132">11</span><span class="sxs-lookup"><span data-stu-id="61b9d-132">11</span></span>|<span data-ttu-id="61b9d-133">デバイスは、MDM および Ea は、構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="61b9d-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="61b9d-134">不明</span><span class="sxs-lookup"><span data-stu-id="61b9d-134">unknown</span></span>|<span data-ttu-id="61b9d-135">16</span><span class="sxs-lookup"><span data-stu-id="61b9d-135">16</span></span>|<span data-ttu-id="61b9d-136">不明な管理エージェントの種類です。</span><span class="sxs-lookup"><span data-stu-id="61b9d-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="61b9d-137">jamf</span><span class="sxs-lookup"><span data-stu-id="61b9d-137">jamf</span></span>|<span data-ttu-id="61b9d-138">32</span><span class="sxs-lookup"><span data-stu-id="61b9d-138">32</span></span>|<span data-ttu-id="61b9d-139">デバイス属性は、Jamf からフェッチされます。</span><span class="sxs-lookup"><span data-stu-id="61b9d-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="61b9d-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="61b9d-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="61b9d-141">64</span><span class="sxs-lookup"><span data-stu-id="61b9d-141">64</span></span>|<span data-ttu-id="61b9d-142">デバイスは、Google の CloudDPC によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="61b9d-142">The device is managed by Google's CloudDPC.</span></span>|



