---
title: microsoft Intune を使用してモバイルアプリを管理する-microsoft Graph API
description: テナント組織のモバイルアプリ管理 (MAM) に関連する Microsoft graph API for Intune エンドポイント (REST) を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4443c78c6ae58979b0390496d8d560bb15a90669
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150401"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="dd267-103">Microsoft Intune で会社のアプリ データを保護する方法</span><span class="sxs-lookup"><span data-stu-id="dd267-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="dd267-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dd267-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd267-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd267-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd267-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd267-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="dd267-107">Microsoft Intune のアプリ保護ポリシーは、会社のデータを保護し、データの損失を防ぐのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="dd267-107">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="dd267-108">Intune のアプリ保護ポリシーを使用して、会社のデータを保護することができます。</span><span class="sxs-lookup"><span data-stu-id="dd267-108">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="dd267-109">Intune アプリ保護ポリシーは、モバイルデバイス管理 (MDM) ソリューションとは独立して使用できるので、デバイス管理ソリューションでデバイスを登録するかどうかにかかわらず、会社のデータを保護するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="dd267-109">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you can use it to protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="dd267-110">アプリレベルのポリシーを実装することで、会社のリソースへのアクセスを制限し、データを IT 部門の管理範囲内に維持できます。</span><span class="sxs-lookup"><span data-stu-id="dd267-110">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="dd267-111">次の Graph リソースを使用して、Intune でのアプリ保護ポリシーを管理できます。</span><span class="sxs-lookup"><span data-stu-id="dd267-111">The following Graph resources are available to manage app protection polices in Intune:</span></span>

- [<span data-ttu-id="dd267-112">Android 管理対象アプリの保護</span><span class="sxs-lookup"><span data-stu-id="dd267-112">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="dd267-113">Android 管理対象アプリの登録</span><span class="sxs-lookup"><span data-stu-id="dd267-113">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="dd267-114">Android モバイル アプリ ID</span><span class="sxs-lookup"><span data-stu-id="dd267-114">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="dd267-115">アプリ管理レベル</span><span class="sxs-lookup"><span data-stu-id="dd267-115">App management level</span></span>](intune-mam-appmanagementlevel.md)
- [<span data-ttu-id="dd267-116">アプリケーションの種類</span><span class="sxs-lookup"><span data-stu-id="dd267-116">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="dd267-117">既定の管理対象アプリ保護</span><span class="sxs-lookup"><span data-stu-id="dd267-117">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="dd267-118">Intune ブランディング プロファイル</span><span class="sxs-lookup"><span data-stu-id="dd267-118">Intune branding profile</span></span>](intune-wip-intunebrandingprofile.md)
- [<span data-ttu-id="dd267-119">Intune ブランディング プロファイルの割り当て</span><span class="sxs-lookup"><span data-stu-id="dd267-119">Intune branding profile assignment</span></span>](intune-wip-intunebrandingprofileassignment.md)
- [<span data-ttu-id="dd267-120">iOS 管理対象アプリ保護</span><span class="sxs-lookup"><span data-stu-id="dd267-120">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="dd267-121">iOS 管理対象アプリの登録</span><span class="sxs-lookup"><span data-stu-id="dd267-121">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="dd267-122">iOS モバイル アプリ ID</span><span class="sxs-lookup"><span data-stu-id="dd267-122">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="dd267-123">JSON</span><span class="sxs-lookup"><span data-stu-id="dd267-123">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="dd267-124">管理対象アプリのクリップボード共有レベル</span><span class="sxs-lookup"><span data-stu-id="dd267-124">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="dd267-125">管理対象アプリの構成</span><span class="sxs-lookup"><span data-stu-id="dd267-125">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="dd267-126">管理対象アプリのデータの暗号化種類</span><span class="sxs-lookup"><span data-stu-id="dd267-126">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="dd267-127">管理対象アプリのデータの保存場所</span><span class="sxs-lookup"><span data-stu-id="dd267-127">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="dd267-128">管理対象アプリのデータ転送レベル</span><span class="sxs-lookup"><span data-stu-id="dd267-128">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="dd267-129">管理対象アプリの診断状態</span><span class="sxs-lookup"><span data-stu-id="dd267-129">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="dd267-130">管理対象アプリのフラグ付き理由</span><span class="sxs-lookup"><span data-stu-id="dd267-130">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="dd267-131">管理対象アプリの操作</span><span class="sxs-lookup"><span data-stu-id="dd267-131">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="dd267-132">管理対象アプリの暗証番号 (PIN) 文字セット</span><span class="sxs-lookup"><span data-stu-id="dd267-132">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="dd267-133">管理対象アプリ ポリシー</span><span class="sxs-lookup"><span data-stu-id="dd267-133">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="dd267-134">管理対象アプリ ポリシーの展開の概要</span><span class="sxs-lookup"><span data-stu-id="dd267-134">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="dd267-135">アプリごとの管理対象アプリ ポリシーの展開の概要</span><span class="sxs-lookup"><span data-stu-id="dd267-135">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="dd267-136">管理対象アプリ保護</span><span class="sxs-lookup"><span data-stu-id="dd267-136">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="dd267-137">管理対象アプリの登録</span><span class="sxs-lookup"><span data-stu-id="dd267-137">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="dd267-138">管理対象アプリの修復処理</span><span class="sxs-lookup"><span data-stu-id="dd267-138">Managed app remediation action</span></span>](intune-mam-managedappremediationaction.md)
- [<span data-ttu-id="dd267-139">管理対象アプリの状態</span><span class="sxs-lookup"><span data-stu-id="dd267-139">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="dd267-140">管理対象アプリの Raw 状態</span><span class="sxs-lookup"><span data-stu-id="dd267-140">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="dd267-141">管理対象モバイル アプリ</span><span class="sxs-lookup"><span data-stu-id="dd267-141">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="dd267-142">MDM Windows 情報保護ポリシー</span><span class="sxs-lookup"><span data-stu-id="dd267-142">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="dd267-143">モバイル アプリ ID</span><span class="sxs-lookup"><span data-stu-id="dd267-143">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="dd267-144">対象となる管理対象アプリの構成</span><span class="sxs-lookup"><span data-stu-id="dd267-144">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="dd267-145">対象となる管理対象アプリ ポリシーの割り当て</span><span class="sxs-lookup"><span data-stu-id="dd267-145">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="dd267-146">対象となる管理対象アプリの保護</span><span class="sxs-lookup"><span data-stu-id="dd267-146">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="dd267-147">Windows 情報保護</span><span class="sxs-lookup"><span data-stu-id="dd267-147">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="dd267-148">Windows 情報保護アプリ</span><span class="sxs-lookup"><span data-stu-id="dd267-148">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="dd267-149">Windows 情報保護アプリの学習概要</span><span class="sxs-lookup"><span data-stu-id="dd267-149">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="dd267-150">Windows 情報保護アプリの Locker ファイル</span><span class="sxs-lookup"><span data-stu-id="dd267-150">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="dd267-151">Windows 情報保護のデータ回復証明書</span><span class="sxs-lookup"><span data-stu-id="dd267-151">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="dd267-152">Windows 情報保護のデスクトップ アプリ</span><span class="sxs-lookup"><span data-stu-id="dd267-152">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="dd267-153">Windows 情報保護のデバイス登録</span><span class="sxs-lookup"><span data-stu-id="dd267-153">Windows information protection device registration</span></span>](intune-mam-windowsinformationprotectiondeviceregistration.md)
- [<span data-ttu-id="dd267-154">Windows 情報保護の実施レベル</span><span class="sxs-lookup"><span data-stu-id="dd267-154">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="dd267-155">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="dd267-155">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="dd267-156">Windows 情報保護のネットワークの学習概要</span><span class="sxs-lookup"><span data-stu-id="dd267-156">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="dd267-157">Windows 情報保護暗証番号 (PIN) の文字の要件</span><span class="sxs-lookup"><span data-stu-id="dd267-157">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="dd267-158">Windows 情報保護ポリシー</span><span class="sxs-lookup"><span data-stu-id="dd267-158">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="dd267-159">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="dd267-159">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="dd267-160">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="dd267-160">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="dd267-161">Windows 情報保護ストア アプリ</span><span class="sxs-lookup"><span data-stu-id="dd267-161">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)
- [<span data-ttu-id="dd267-162">Windows 情報保護のワイプ アクション</span><span class="sxs-lookup"><span data-stu-id="dd267-162">Windows information protection wipe action</span></span>](intune-mam-windowsinformationprotectionwipeaction.md)
