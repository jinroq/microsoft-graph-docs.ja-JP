---
title: Intune における管理用にデバイスを登録する
description: " (BYOD) の登録では、個人の電話、タブレット、または Pc を登録することができます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。"
localization_priority: Normal
ms.openlocfilehash: de2a87c08851081891ee641db50a4ca1c64cb314
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841322"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="457b2-104">Intune における管理用にデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="457b2-104">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="457b2-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="457b2-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="457b2-106">デバイス (Windows PC を含む) を登録して、Microsoft Intune でモバイル デバイス管理 (MDM) を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="457b2-106">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="457b2-107">このトピックでは、Intune 管理における、いくつかのモバイル デバイスの登録方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="457b2-107">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="457b2-108">デバイスを登録する方法は、デバイスの種類、所有権、必要な管理のレベルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="457b2-108">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="457b2-109">"Bring Your Own Device" (BYOD) の登録により、ユーザーは、個人の電話、タブレット、PC を登録することができます。</span><span class="sxs-lookup"><span data-stu-id="457b2-109">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="457b2-110">会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。</span><span class="sxs-lookup"><span data-stu-id="457b2-110">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="457b2-111">次の Graph リソースを使用して、Intune での登録を管理できます。</span><span class="sxs-lookup"><span data-stu-id="457b2-111">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="457b2-112">デバイス登録の構成</span><span class="sxs-lookup"><span data-stu-id="457b2-112">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="457b2-113">デバイス登録の制限の構成</span><span class="sxs-lookup"><span data-stu-id="457b2-113">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="457b2-114">デバイス登録プラットフォームの制限</span><span class="sxs-lookup"><span data-stu-id="457b2-114">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="457b2-115">デバイス登録プラットフォームの制限の構成</span><span class="sxs-lookup"><span data-stu-id="457b2-115">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="457b2-116">デバイス登録 Windows Hello for Business の構成</span><span class="sxs-lookup"><span data-stu-id="457b2-116">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="457b2-117">デバイスの管理 Exchange コネクタ</span><span class="sxs-lookup"><span data-stu-id="457b2-117">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="457b2-118">デバイス管理 exchange コネクタの状態</span><span class="sxs-lookup"><span data-stu-id="457b2-118">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="457b2-119">デバイス管理 exchange コネクタの同期の種類</span><span class="sxs-lookup"><span data-stu-id="457b2-119">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="457b2-120">デバイス管理 exchange コネクタの種類</span><span class="sxs-lookup"><span data-stu-id="457b2-120">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="457b2-121">デバイス管理パートナー</span><span class="sxs-lookup"><span data-stu-id="457b2-121">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="457b2-122">デバイス管理のパートナー アプリケーションの種類</span><span class="sxs-lookup"><span data-stu-id="457b2-122">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="457b2-123">デバイス管理のパートナーのテナントの状態</span><span class="sxs-lookup"><span data-stu-id="457b2-123">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="457b2-124">有効化</span><span class="sxs-lookup"><span data-stu-id="457b2-124">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="457b2-125">登録構成の割り当て</span><span class="sxs-lookup"><span data-stu-id="457b2-125">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="457b2-126">Intune ブランド</span><span class="sxs-lookup"><span data-stu-id="457b2-126">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="457b2-127">MDM 機関</span><span class="sxs-lookup"><span data-stu-id="457b2-127">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="457b2-128">モバイルの脅威保護コネクタ</span><span class="sxs-lookup"><span data-stu-id="457b2-128">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="457b2-129">モバイル脅威パートナー テナントの状態</span><span class="sxs-lookup"><span data-stu-id="457b2-129">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="457b2-130">オンプレミスの条件付きアクセス設定</span><span class="sxs-lookup"><span data-stu-id="457b2-130">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="457b2-131">組織</span><span class="sxs-lookup"><span data-stu-id="457b2-131">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="457b2-132">RGB カラー</span><span class="sxs-lookup"><span data-stu-id="457b2-132">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="457b2-133">VPP トークン</span><span class="sxs-lookup"><span data-stu-id="457b2-133">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="457b2-134">VPP トークンの状態</span><span class="sxs-lookup"><span data-stu-id="457b2-134">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="457b2-135">VPP トークンの同期の状態</span><span class="sxs-lookup"><span data-stu-id="457b2-135">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="457b2-136">Windows Hello ビジネス暗証番号 (pin) を使用するため</span><span class="sxs-lookup"><span data-stu-id="457b2-136">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)
