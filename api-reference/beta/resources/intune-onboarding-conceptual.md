---
title: Intune を使用した管理対象デバイス-Microsoft Graph API
description: テナント組織用にデバイスをオンボード (構成および初期化) するために使用される Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cc082578bea7e6b1d477547538e01dbaa1ef2bdb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998234"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="db506-103">Intune における管理用にデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="db506-103">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="db506-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="db506-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db506-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db506-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db506-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="db506-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db506-107">デバイス (Windows PC を含む) を登録して、Microsoft Intune でモバイル デバイス管理 (MDM) を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="db506-107">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="db506-108">このトピックでは、Intune 管理における、いくつかのモバイル デバイスの登録方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="db506-108">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="db506-109">デバイスを登録する方法は、デバイスの種類、所有権、必要な管理のレベルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="db506-109">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="db506-110">"Bring Your Own Device" (BYOD) の登録により、ユーザーは、個人の電話、タブレット、PC を登録することができます。</span><span class="sxs-lookup"><span data-stu-id="db506-110">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="db506-111">会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。</span><span class="sxs-lookup"><span data-stu-id="db506-111">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="db506-112">次の Graph リソースを使用して、Intune での登録を管理できます。</span><span class="sxs-lookup"><span data-stu-id="db506-112">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="db506-113">証明書コネクタの設定</span><span class="sxs-lookup"><span data-stu-id="db506-113">Certificate connector setting</span></span>](intune-onboarding-certificateconnectorsetting.md)
- [<span data-ttu-id="db506-114">デバイスおよびアプリの管理データ</span><span class="sxs-lookup"><span data-stu-id="db506-114">Device and app management data</span></span>](intune-onboarding-deviceandappmanagementdata.md)
- [<span data-ttu-id="db506-115">デバイス登録の構成</span><span class="sxs-lookup"><span data-stu-id="db506-115">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="db506-116">デバイス登録の制限の構成</span><span class="sxs-lookup"><span data-stu-id="db506-116">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="db506-117">デバイス登録プラットフォームの制限</span><span class="sxs-lookup"><span data-stu-id="db506-117">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="db506-118">デバイス登録プラットフォームの制限の構成</span><span class="sxs-lookup"><span data-stu-id="db506-118">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="db506-119">デバイス登録 Windows Hello for Business の構成</span><span class="sxs-lookup"><span data-stu-id="db506-119">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="db506-120">デバイスの管理 Exchange アクセス レベル</span><span class="sxs-lookup"><span data-stu-id="db506-120">Device management exchange access level</span></span>](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [<span data-ttu-id="db506-121">デバイスの管理 Exchange アクセス ルール</span><span class="sxs-lookup"><span data-stu-id="db506-121">Device management exchange access rule</span></span>](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [<span data-ttu-id="db506-122">デバイスの管理 Exchange アクセス ルールのタイプ</span><span class="sxs-lookup"><span data-stu-id="db506-122">Device management exchange access rule type</span></span>](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [<span data-ttu-id="db506-123">デバイスの管理 Exchange コネクタ</span><span class="sxs-lookup"><span data-stu-id="db506-123">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="db506-124">デバイスの管理 Exchange コネクタの状態</span><span class="sxs-lookup"><span data-stu-id="db506-124">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="db506-125">デバイスの管理 Exchange コネクタの同期タイプ</span><span class="sxs-lookup"><span data-stu-id="db506-125">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="db506-126">デバイスの管理 Exchange コネクタのタイプ</span><span class="sxs-lookup"><span data-stu-id="db506-126">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="db506-127">デバイスの管理 Exchange デバイス クラス</span><span class="sxs-lookup"><span data-stu-id="db506-127">Device management exchange device class</span></span>](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [<span data-ttu-id="db506-128">デバイスの管理 Exchange オンプレミスのポリシー</span><span class="sxs-lookup"><span data-stu-id="db506-128">Device management exchange on-premises policy</span></span>](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [<span data-ttu-id="db506-129">デバイス管理パートナー</span><span class="sxs-lookup"><span data-stu-id="db506-129">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="db506-130">デバイス管理パートナー アプリの種類</span><span class="sxs-lookup"><span data-stu-id="db506-130">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="db506-131">デバイス管理パートナー テナントの状態</span><span class="sxs-lookup"><span data-stu-id="db506-131">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="db506-132">登録構成の割り当て</span><span class="sxs-lookup"><span data-stu-id="db506-132">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="db506-133">Intune ブランド</span><span class="sxs-lookup"><span data-stu-id="db506-133">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="db506-134">MDM 機関</span><span class="sxs-lookup"><span data-stu-id="db506-134">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="db506-135">ビジネス向け Microsoft Store のポータル選択オプション</span><span class="sxs-lookup"><span data-stu-id="db506-135">Microsoft store for business portal selection options</span></span>](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [<span data-ttu-id="db506-136">モバイルの脅威保護コネクタ</span><span class="sxs-lookup"><span data-stu-id="db506-136">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="db506-137">モバイル脅威パートナーのテナント状態</span><span class="sxs-lookup"><span data-stu-id="db506-137">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="db506-138">オンプレミスの条件付きアクセス設定</span><span class="sxs-lookup"><span data-stu-id="db506-138">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="db506-139">組織</span><span class="sxs-lookup"><span data-stu-id="db506-139">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="db506-140">サイドローディング キー</span><span class="sxs-lookup"><span data-stu-id="db506-140">Side loading key</span></span>](intune-onboarding-sideloadingkey.md)
- [<span data-ttu-id="db506-141">VPP トークン</span><span class="sxs-lookup"><span data-stu-id="db506-141">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="db506-142">VPP トークンのアクションの結果</span><span class="sxs-lookup"><span data-stu-id="db506-142">VPP token action result</span></span>](intune-onboarding-vpptokenactionresult.md)
- [<span data-ttu-id="db506-143">VPP トークンのライセンスの概要</span><span class="sxs-lookup"><span data-stu-id="db506-143">VPP token license summary</span></span>](intune-onboarding-vpptokenlicensesummary.md)
- [<span data-ttu-id="db506-144">VPP トークンの失効ライセンスのアクションの結果</span><span class="sxs-lookup"><span data-stu-id="db506-144">VPP token revoke licenses action result</span></span>](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [<span data-ttu-id="db506-145">VPP トークンの状態</span><span class="sxs-lookup"><span data-stu-id="db506-145">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="db506-146">VPP トークンの同期状態</span><span class="sxs-lookup"><span data-stu-id="db506-146">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="db506-147">Windows 10 登録完了ページの構成</span><span class="sxs-lookup"><span data-stu-id="db506-147">Windows 10 enrollment completion page configuration</span></span>](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [<span data-ttu-id="db506-148">ビジネス向け Windows Hello 暗証番号 (PIN) の使用</span><span class="sxs-lookup"><span data-stu-id="db506-148">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)
