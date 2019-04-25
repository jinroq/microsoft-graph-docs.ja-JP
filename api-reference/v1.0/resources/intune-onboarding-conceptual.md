---
title: Intune における管理用にデバイスを登録する
description: " (byod) の登録では、ユーザーは自分の携帯電話、タブレット、または pc を登録できます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。"
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 2e7f6e85e32137804556c64a1995bd2e78b04068
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564240"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="0aae8-104">Intune における管理用にデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="0aae8-104">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="0aae8-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0aae8-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="0aae8-106">デバイス (Windows PC を含む) を登録して、Microsoft Intune でモバイル デバイス管理 (MDM) を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0aae8-106">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="0aae8-107">このトピックでは、Intune 管理における、いくつかのモバイル デバイスの登録方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="0aae8-107">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="0aae8-108">デバイスを登録する方法は、デバイスの種類、所有権、必要な管理のレベルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="0aae8-108">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="0aae8-109">"Bring Your Own Device" (BYOD) の登録により、ユーザーは、個人の電話、タブレット、PC を登録することができます。</span><span class="sxs-lookup"><span data-stu-id="0aae8-109">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="0aae8-110">会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。</span><span class="sxs-lookup"><span data-stu-id="0aae8-110">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="0aae8-111">次の Graph リソースを使用して、Intune での登録を管理できます。</span><span class="sxs-lookup"><span data-stu-id="0aae8-111">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="0aae8-112">デバイス登録の構成</span><span class="sxs-lookup"><span data-stu-id="0aae8-112">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="0aae8-113">デバイス登録の制限の構成</span><span class="sxs-lookup"><span data-stu-id="0aae8-113">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="0aae8-114">デバイス登録プラットフォームの制限</span><span class="sxs-lookup"><span data-stu-id="0aae8-114">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="0aae8-115">デバイス登録プラットフォームの制限の構成</span><span class="sxs-lookup"><span data-stu-id="0aae8-115">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="0aae8-116">デバイス登録 Windows Hello for Business の構成</span><span class="sxs-lookup"><span data-stu-id="0aae8-116">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="0aae8-117">デバイスの管理 Exchange コネクタ</span><span class="sxs-lookup"><span data-stu-id="0aae8-117">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="0aae8-118">デバイスの管理 Exchange コネクタの状態</span><span class="sxs-lookup"><span data-stu-id="0aae8-118">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="0aae8-119">デバイスの管理 Exchange コネクタの同期タイプ</span><span class="sxs-lookup"><span data-stu-id="0aae8-119">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="0aae8-120">デバイスの管理 Exchange コネクタのタイプ</span><span class="sxs-lookup"><span data-stu-id="0aae8-120">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="0aae8-121">デバイス管理パートナー</span><span class="sxs-lookup"><span data-stu-id="0aae8-121">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="0aae8-122">デバイス管理パートナー アプリの種類</span><span class="sxs-lookup"><span data-stu-id="0aae8-122">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="0aae8-123">デバイス管理パートナー テナントの状態</span><span class="sxs-lookup"><span data-stu-id="0aae8-123">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="0aae8-124">有効化</span><span class="sxs-lookup"><span data-stu-id="0aae8-124">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="0aae8-125">登録構成の割り当て</span><span class="sxs-lookup"><span data-stu-id="0aae8-125">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="0aae8-126">Intune ブランド</span><span class="sxs-lookup"><span data-stu-id="0aae8-126">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="0aae8-127">MDM 機関</span><span class="sxs-lookup"><span data-stu-id="0aae8-127">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="0aae8-128">モバイルの脅威保護コネクタ</span><span class="sxs-lookup"><span data-stu-id="0aae8-128">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="0aae8-129">モバイル脅威パートナーのテナント状態</span><span class="sxs-lookup"><span data-stu-id="0aae8-129">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="0aae8-130">オンプレミスの条件付きアクセス設定</span><span class="sxs-lookup"><span data-stu-id="0aae8-130">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="0aae8-131">組織</span><span class="sxs-lookup"><span data-stu-id="0aae8-131">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="0aae8-132">RGB カラー</span><span class="sxs-lookup"><span data-stu-id="0aae8-132">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="0aae8-133">VPP トークン</span><span class="sxs-lookup"><span data-stu-id="0aae8-133">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="0aae8-134">VPP トークンの状態</span><span class="sxs-lookup"><span data-stu-id="0aae8-134">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="0aae8-135">VPP トークンの同期状態</span><span class="sxs-lookup"><span data-stu-id="0aae8-135">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="0aae8-136">ビジネス向け Windows Hello 暗証番号 (PIN) の使用</span><span class="sxs-lookup"><span data-stu-id="0aae8-136">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)
