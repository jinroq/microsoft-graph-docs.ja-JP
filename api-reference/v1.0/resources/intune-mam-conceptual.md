---
title: Microsoft Intune で会社のアプリ データを保護する方法
description: Microsoft Intune のアプリ保護ポリシーは、会社のデータを保護し、データの損失を防ぐのに役立ちます。
ms.openlocfilehash: d92302b93f46895333e261917ddb91268c5956a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023175"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="f47a3-103">Microsoft Intune で会社のアプリ データを保護する方法</span><span class="sxs-lookup"><span data-stu-id="f47a3-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="f47a3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f47a3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="f47a3-105">Microsoft Intune のアプリ保護ポリシーは、会社のデータを保護し、データの損失を防ぐのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="f47a3-105">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="f47a3-106">Intune のアプリ保護ポリシーを使用して、会社のデータを保護することができます。</span><span class="sxs-lookup"><span data-stu-id="f47a3-106">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="f47a3-107">Intune のアプリ保護ポリシーは、モバイル デバイス管理 (MDM) ソリューションとは独立して使用できるため、デバイス管理ソリューションでのデバイス登録の有無に関係なく、会社のデータを保護することができます。</span><span class="sxs-lookup"><span data-stu-id="f47a3-107">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="f47a3-108">アプリレベルのポリシーを実装することで、会社のリソースへのアクセスを制限し、データを IT 部門の管理範囲内に維持できます。</span><span class="sxs-lookup"><span data-stu-id="f47a3-108">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="f47a3-109">次の Graph リソースを使用して、Intune でのアプリ保護ポリシーを管理できます。</span><span class="sxs-lookup"><span data-stu-id="f47a3-109">The following Graph resources are available to manage app protection polices in Intune:</span></span>  

- [<span data-ttu-id="f47a3-110">Android 管理対象アプリの保護</span><span class="sxs-lookup"><span data-stu-id="f47a3-110">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="f47a3-111">Android 管理対象アプリの登録</span><span class="sxs-lookup"><span data-stu-id="f47a3-111">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="f47a3-112">Android モバイル アプリ ID</span><span class="sxs-lookup"><span data-stu-id="f47a3-112">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="f47a3-113">アプリケーションの種類</span><span class="sxs-lookup"><span data-stu-id="f47a3-113">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="f47a3-114">既定の管理対象アプリ保護</span><span class="sxs-lookup"><span data-stu-id="f47a3-114">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="f47a3-115">iOS 管理対象アプリ保護</span><span class="sxs-lookup"><span data-stu-id="f47a3-115">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="f47a3-116">iOS 管理対象アプリの登録</span><span class="sxs-lookup"><span data-stu-id="f47a3-116">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="f47a3-117">iOS モバイル アプリ ID</span><span class="sxs-lookup"><span data-stu-id="f47a3-117">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="f47a3-118">IP 範囲</span><span class="sxs-lookup"><span data-stu-id="f47a3-118">IP range</span></span>](intune-mam-iprange.md)
- [<span data-ttu-id="f47a3-119">IPv4 の範囲</span><span class="sxs-lookup"><span data-stu-id="f47a3-119">IPv4 range</span></span>](intune-mam-ipv4range.md)
- [<span data-ttu-id="f47a3-120">IPv6 の範囲</span><span class="sxs-lookup"><span data-stu-id="f47a3-120">IPv6 range</span></span>](intune-mam-ipv6range.md)
- [<span data-ttu-id="f47a3-121">JSON</span><span class="sxs-lookup"><span data-stu-id="f47a3-121">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="f47a3-122">キー/値のペア</span><span class="sxs-lookup"><span data-stu-id="f47a3-122">Key/value pair</span></span>](intune-mam-keyvaluepair.md)
- [<span data-ttu-id="f47a3-123">アプリケーションのクリップボード共有機能レベルの管理</span><span class="sxs-lookup"><span data-stu-id="f47a3-123">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="f47a3-124">管理対象アプリの構成</span><span class="sxs-lookup"><span data-stu-id="f47a3-124">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="f47a3-125">アプリケーション データの暗号化の種類を管理</span><span class="sxs-lookup"><span data-stu-id="f47a3-125">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="f47a3-126">管理されているアプリケーション データの格納場所</span><span class="sxs-lookup"><span data-stu-id="f47a3-126">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="f47a3-127">管理されているアプリケーション データの転送レベル</span><span class="sxs-lookup"><span data-stu-id="f47a3-127">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="f47a3-128">管理対象アプリの診断状態</span><span class="sxs-lookup"><span data-stu-id="f47a3-128">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="f47a3-129">マネージ アプリケーションのフラグを設定した理由</span><span class="sxs-lookup"><span data-stu-id="f47a3-129">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="f47a3-130">管理対象アプリの操作</span><span class="sxs-lookup"><span data-stu-id="f47a3-130">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="f47a3-131">暗証番号 (pin) のマネージ アプリケーションの文字セット</span><span class="sxs-lookup"><span data-stu-id="f47a3-131">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="f47a3-132">管理対象アプリ ポリシー</span><span class="sxs-lookup"><span data-stu-id="f47a3-132">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="f47a3-133">管理対象アプリ ポリシーの展開の概要</span><span class="sxs-lookup"><span data-stu-id="f47a3-133">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="f47a3-134">アプリごとの管理対象アプリ ポリシーの展開の概要</span><span class="sxs-lookup"><span data-stu-id="f47a3-134">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="f47a3-135">管理対象アプリ保護</span><span class="sxs-lookup"><span data-stu-id="f47a3-135">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="f47a3-136">管理対象アプリの登録</span><span class="sxs-lookup"><span data-stu-id="f47a3-136">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="f47a3-137">管理対象アプリの状態</span><span class="sxs-lookup"><span data-stu-id="f47a3-137">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="f47a3-138">管理対象アプリの Raw 状態</span><span class="sxs-lookup"><span data-stu-id="f47a3-138">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="f47a3-139">管理対象モバイル アプリ</span><span class="sxs-lookup"><span data-stu-id="f47a3-139">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="f47a3-140">MDM Windows 情報保護ポリシー</span><span class="sxs-lookup"><span data-stu-id="f47a3-140">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="f47a3-141">モバイル アプリ ID</span><span class="sxs-lookup"><span data-stu-id="f47a3-141">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="f47a3-142">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="f47a3-142">Proxied domain</span></span>](intune-mam-proxieddomain.md)
- [<span data-ttu-id="f47a3-143">対象となる管理対象アプリの構成</span><span class="sxs-lookup"><span data-stu-id="f47a3-143">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="f47a3-144">対象となる管理対象アプリ ポリシーの割り当て</span><span class="sxs-lookup"><span data-stu-id="f47a3-144">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="f47a3-145">対象となる管理対象アプリの保護</span><span class="sxs-lookup"><span data-stu-id="f47a3-145">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="f47a3-146">Windows 情報保護</span><span class="sxs-lookup"><span data-stu-id="f47a3-146">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="f47a3-147">Windows 情報保護アプリ</span><span class="sxs-lookup"><span data-stu-id="f47a3-147">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="f47a3-148">Windows 情報保護アプリの学習概要</span><span class="sxs-lookup"><span data-stu-id="f47a3-148">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="f47a3-149">Windows 情報保護アプリの Locker ファイル</span><span class="sxs-lookup"><span data-stu-id="f47a3-149">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="f47a3-150">Windows 情報保護のデータ回復証明書</span><span class="sxs-lookup"><span data-stu-id="f47a3-150">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="f47a3-151">Windows 情報保護のデスクトップ アプリ</span><span class="sxs-lookup"><span data-stu-id="f47a3-151">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="f47a3-152">Windows 情報保護の適用レベル</span><span class="sxs-lookup"><span data-stu-id="f47a3-152">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="f47a3-153">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="f47a3-153">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="f47a3-154">Windows 情報保護のネットワークの学習概要</span><span class="sxs-lookup"><span data-stu-id="f47a3-154">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="f47a3-155">Windows 情報保護暗証番号 (pin) の文字の要件</span><span class="sxs-lookup"><span data-stu-id="f47a3-155">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="f47a3-156">Windows 情報保護ポリシー</span><span class="sxs-lookup"><span data-stu-id="f47a3-156">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="f47a3-157">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="f47a3-157">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="f47a3-158">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="f47a3-158">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="f47a3-159">Windows 情報保護ストア アプリ</span><span class="sxs-lookup"><span data-stu-id="f47a3-159">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)
