---
title: Intune における管理用にデバイスを登録する
description: " (BYOD) の登録では、個人の電話、タブレット、または Pc を登録することができます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。"
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 895977194822918fc2ac61ed13e0aae938a25166
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923748"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="33a7b-104">Intune における管理用にデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="33a7b-104">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="33a7b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33a7b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33a7b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33a7b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33a7b-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="33a7b-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="33a7b-108">デバイス (Windows PC を含む) を登録して、Microsoft Intune でモバイル デバイス管理 (MDM) を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="33a7b-108">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="33a7b-109">このトピックでは、Intune 管理における、いくつかのモバイル デバイスの登録方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="33a7b-109">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="33a7b-110">デバイスを登録する方法は、デバイスの種類、所有権、必要な管理のレベルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="33a7b-110">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="33a7b-111">"Bring Your Own Device" (BYOD) の登録により、ユーザーは、個人の電話、タブレット、PC を登録することができます。</span><span class="sxs-lookup"><span data-stu-id="33a7b-111">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="33a7b-112">会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。</span><span class="sxs-lookup"><span data-stu-id="33a7b-112">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="33a7b-113">次の Graph リソースを使用して、Intune での登録を管理できます。</span><span class="sxs-lookup"><span data-stu-id="33a7b-113">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="33a7b-114">証明書のコネクタの設定</span><span class="sxs-lookup"><span data-stu-id="33a7b-114">Certificate connector setting</span></span>](intune-onboarding-certificateconnectorsetting.md)
- [<span data-ttu-id="33a7b-115">デバイスとアプリケーションの管理データ</span><span class="sxs-lookup"><span data-stu-id="33a7b-115">Device and app management data</span></span>](intune-onboarding-deviceandappmanagementdata.md)
- [<span data-ttu-id="33a7b-116">デバイス登録の構成</span><span class="sxs-lookup"><span data-stu-id="33a7b-116">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="33a7b-117">デバイス登録の制限の構成</span><span class="sxs-lookup"><span data-stu-id="33a7b-117">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="33a7b-118">デバイス登録プラットフォームの制限</span><span class="sxs-lookup"><span data-stu-id="33a7b-118">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="33a7b-119">デバイス登録プラットフォームの制限の構成</span><span class="sxs-lookup"><span data-stu-id="33a7b-119">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="33a7b-120">デバイス登録 Windows Hello for Business の構成</span><span class="sxs-lookup"><span data-stu-id="33a7b-120">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="33a7b-121">デバイス管理 exchange のアクセス レベル</span><span class="sxs-lookup"><span data-stu-id="33a7b-121">Device management exchange access level</span></span>](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [<span data-ttu-id="33a7b-122">デバイス管理 exchange のアクセス ルール</span><span class="sxs-lookup"><span data-stu-id="33a7b-122">Device management exchange access rule</span></span>](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [<span data-ttu-id="33a7b-123">デバイス管理 exchange アクセス規則の種類</span><span class="sxs-lookup"><span data-stu-id="33a7b-123">Device management exchange access rule type</span></span>](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [<span data-ttu-id="33a7b-124">デバイスの管理 Exchange コネクタ</span><span class="sxs-lookup"><span data-stu-id="33a7b-124">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="33a7b-125">デバイス管理 exchange コネクタの状態</span><span class="sxs-lookup"><span data-stu-id="33a7b-125">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="33a7b-126">デバイス管理 exchange コネクタの同期の種類</span><span class="sxs-lookup"><span data-stu-id="33a7b-126">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="33a7b-127">デバイス管理 exchange コネクタの種類</span><span class="sxs-lookup"><span data-stu-id="33a7b-127">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="33a7b-128">デバイス管理 exchange デバイス クラス</span><span class="sxs-lookup"><span data-stu-id="33a7b-128">Device management exchange device class</span></span>](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [<span data-ttu-id="33a7b-129">デバイス管理の交換設置のポリシー</span><span class="sxs-lookup"><span data-stu-id="33a7b-129">Device management exchange on-premises policy</span></span>](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [<span data-ttu-id="33a7b-130">デバイス管理パートナー</span><span class="sxs-lookup"><span data-stu-id="33a7b-130">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="33a7b-131">デバイス管理のパートナー アプリケーションの種類</span><span class="sxs-lookup"><span data-stu-id="33a7b-131">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="33a7b-132">デバイス管理のパートナーのテナントの状態</span><span class="sxs-lookup"><span data-stu-id="33a7b-132">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="33a7b-133">登録構成の割り当て</span><span class="sxs-lookup"><span data-stu-id="33a7b-133">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="33a7b-134">Intune ブランド</span><span class="sxs-lookup"><span data-stu-id="33a7b-134">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="33a7b-135">MDM 機関</span><span class="sxs-lookup"><span data-stu-id="33a7b-135">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="33a7b-136">ビジネス ポータルの選択オプションのマイクロソフト ストア</span><span class="sxs-lookup"><span data-stu-id="33a7b-136">Microsoft store for business portal selection options</span></span>](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [<span data-ttu-id="33a7b-137">モバイルの脅威保護コネクタ</span><span class="sxs-lookup"><span data-stu-id="33a7b-137">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="33a7b-138">モバイル脅威パートナー テナントの状態</span><span class="sxs-lookup"><span data-stu-id="33a7b-138">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="33a7b-139">オンプレミスの条件付きアクセス設定</span><span class="sxs-lookup"><span data-stu-id="33a7b-139">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="33a7b-140">組織</span><span class="sxs-lookup"><span data-stu-id="33a7b-140">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="33a7b-141">側のロード キー</span><span class="sxs-lookup"><span data-stu-id="33a7b-141">Side loading key</span></span>](intune-onboarding-sideloadingkey.md)
- [<span data-ttu-id="33a7b-142">VPP トークン</span><span class="sxs-lookup"><span data-stu-id="33a7b-142">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="33a7b-143">VPP トークン処理結果</span><span class="sxs-lookup"><span data-stu-id="33a7b-143">VPP token action result</span></span>](intune-onboarding-vpptokenactionresult.md)
- [<span data-ttu-id="33a7b-144">VPP トークン ライセンスの概要</span><span class="sxs-lookup"><span data-stu-id="33a7b-144">VPP token license summary</span></span>](intune-onboarding-vpptokenlicensesummary.md)
- [<span data-ttu-id="33a7b-145">VPP トークンの取り消しライセンスのアクションの結果</span><span class="sxs-lookup"><span data-stu-id="33a7b-145">VPP token revoke licenses action result</span></span>](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [<span data-ttu-id="33a7b-146">VPP トークンの状態</span><span class="sxs-lookup"><span data-stu-id="33a7b-146">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="33a7b-147">VPP トークンの同期の状態</span><span class="sxs-lookup"><span data-stu-id="33a7b-147">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- <span data-ttu-id="33a7b-148">[Windows 10 登録の完了] ページの構成](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33a7b-148">[Windows 10 enrollment completion page configuration](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)</span></span>
- [<span data-ttu-id="33a7b-149">Windows Hello ビジネス暗証番号 (pin) を使用するため</span><span class="sxs-lookup"><span data-stu-id="33a7b-149">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)
