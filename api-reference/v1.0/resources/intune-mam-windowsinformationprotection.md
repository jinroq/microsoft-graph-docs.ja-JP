---
title: windowsInformationProtection リソース タイプ
description: 詳細な管理設定を構成するための Windows 情報保護のポリシー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3ac81f6d4e04835308e3d3d89bf02d91c81fe9c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263057"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="e03f8-103">windowsInformationProtection リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="e03f8-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="e03f8-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e03f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e03f8-105">詳細な管理設定を構成するための Windows 情報保護のポリシー</span><span class="sxs-lookup"><span data-stu-id="e03f8-105">Policy for Windows information protection to configure detailed management settings</span></span>


<span data-ttu-id="e03f8-106">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e03f8-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e03f8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e03f8-107">Methods</span></span>
|<span data-ttu-id="e03f8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e03f8-108">Method</span></span>|<span data-ttu-id="e03f8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e03f8-109">Return Type</span></span>|<span data-ttu-id="e03f8-110">説明</span><span class="sxs-lookup"><span data-stu-id="e03f8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e03f8-111">List windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="e03f8-111">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="e03f8-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="e03f8-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e03f8-113">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="e03f8-114">Get windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="e03f8-114">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="e03f8-115">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="e03f8-115">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="e03f8-116">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e03f8-116">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="e03f8-117">assign action</span><span class="sxs-lookup"><span data-stu-id="e03f8-117">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="e03f8-118">なし</span><span class="sxs-lookup"><span data-stu-id="e03f8-118">None</span></span>|<span data-ttu-id="e03f8-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e03f8-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e03f8-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e03f8-120">Properties</span></span>
|<span data-ttu-id="e03f8-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e03f8-121">Property</span></span>|<span data-ttu-id="e03f8-122">型</span><span class="sxs-lookup"><span data-stu-id="e03f8-122">Type</span></span>|<span data-ttu-id="e03f8-123">説明</span><span class="sxs-lookup"><span data-stu-id="e03f8-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e03f8-124">displayName</span><span class="sxs-lookup"><span data-stu-id="e03f8-124">displayName</span></span>|<span data-ttu-id="e03f8-125">String</span><span class="sxs-lookup"><span data-stu-id="e03f8-125">String</span></span>|<span data-ttu-id="e03f8-126">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="e03f8-126">Policy display name.</span></span> <span data-ttu-id="e03f8-127">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e03f8-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e03f8-128">説明</span><span class="sxs-lookup"><span data-stu-id="e03f8-128">description</span></span>|<span data-ttu-id="e03f8-129">文字列</span><span class="sxs-lookup"><span data-stu-id="e03f8-129">String</span></span>|<span data-ttu-id="e03f8-130">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="e03f8-130">The policy's description.</span></span> <span data-ttu-id="e03f8-131">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e03f8-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e03f8-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e03f8-132">createdDateTime</span></span>|<span data-ttu-id="e03f8-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e03f8-133">DateTimeOffset</span></span>|<span data-ttu-id="e03f8-134">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e03f8-134">The date and time the policy was created.</span></span> <span data-ttu-id="e03f8-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e03f8-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e03f8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e03f8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e03f8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e03f8-137">DateTimeOffset</span></span>|<span data-ttu-id="e03f8-138">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="e03f8-138">Last time the policy was modified.</span></span> <span data-ttu-id="e03f8-139">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e03f8-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e03f8-140">id</span><span class="sxs-lookup"><span data-stu-id="e03f8-140">id</span></span>|<span data-ttu-id="e03f8-141">文字列</span><span class="sxs-lookup"><span data-stu-id="e03f8-141">String</span></span>|<span data-ttu-id="e03f8-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e03f8-142">Key of the entity.</span></span> <span data-ttu-id="e03f8-143">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e03f8-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e03f8-144">version</span><span class="sxs-lookup"><span data-stu-id="e03f8-144">version</span></span>|<span data-ttu-id="e03f8-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e03f8-145">String</span></span>|<span data-ttu-id="e03f8-146">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e03f8-146">Version of the entity.</span></span> <span data-ttu-id="e03f8-147">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e03f8-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e03f8-148">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="e03f8-148">enforcementLevel</span></span>|[<span data-ttu-id="e03f8-149">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="e03f8-149">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="e03f8-150">仕掛品の実施レベル。サポートされている値については、Enum 定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e03f8-150">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="e03f8-151">使用可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="e03f8-151">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="e03f8-152">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="e03f8-152">enterpriseDomain</span></span>|<span data-ttu-id="e03f8-153">String</span><span class="sxs-lookup"><span data-stu-id="e03f8-153">String</span></span>|<span data-ttu-id="e03f8-154">プライマリ エンタープライズ ドメイン</span><span class="sxs-lookup"><span data-stu-id="e03f8-154">Primary enterprise domain</span></span>|
|<span data-ttu-id="e03f8-155">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="e03f8-155">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="e03f8-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e03f8-157">保護するエンタープライズ ドメインのリスト</span><span class="sxs-lookup"><span data-stu-id="e03f8-157">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="e03f8-158">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="e03f8-158">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="e03f8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="e03f8-159">Boolean</span></span>|<span data-ttu-id="e03f8-160">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="e03f8-160">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="e03f8-161">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="e03f8-161">dataRecoveryCertificate</span></span>|[<span data-ttu-id="e03f8-162">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="e03f8-162">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="e03f8-163">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="e03f8-163">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="e03f8-164">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです。</span><span class="sxs-lookup"><span data-stu-id="e03f8-164">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="e03f8-165">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="e03f8-165">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="e03f8-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="e03f8-166">Boolean</span></span>|<span data-ttu-id="e03f8-167">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="e03f8-167">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="e03f8-168">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e03f8-168">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="e03f8-169">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="e03f8-169">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="e03f8-170">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="e03f8-170">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="e03f8-171">Guid</span><span class="sxs-lookup"><span data-stu-id="e03f8-171">Guid</span></span>|<span data-ttu-id="e03f8-172">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="e03f8-172">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="e03f8-173">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーとアクセスできる期間について、詳細を構成することができます</span><span class="sxs-lookup"><span data-stu-id="e03f8-173">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="e03f8-174">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="e03f8-174">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="e03f8-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="e03f8-175">Boolean</span></span>|<span data-ttu-id="e03f8-176">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="e03f8-176">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="e03f8-177">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="e03f8-177">iconsVisible</span></span>|<span data-ttu-id="e03f8-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="e03f8-178">Boolean</span></span>|<span data-ttu-id="e03f8-179">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="e03f8-179">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="e03f8-180">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します</span><span class="sxs-lookup"><span data-stu-id="e03f8-180">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="e03f8-181">protectedApps</span><span class="sxs-lookup"><span data-stu-id="e03f8-181">protectedApps</span></span>|<span data-ttu-id="e03f8-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="e03f8-183">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます</span><span class="sxs-lookup"><span data-stu-id="e03f8-183">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="e03f8-184">exemptApps</span><span class="sxs-lookup"><span data-stu-id="e03f8-184">exemptApps</span></span>|<span data-ttu-id="e03f8-185">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-185">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="e03f8-186">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="e03f8-186">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="e03f8-187">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="e03f8-187">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="e03f8-188">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="e03f8-188">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="e03f8-189">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-189">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e03f8-190">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="e03f8-190">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="e03f8-191">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データとみなされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます</span><span class="sxs-lookup"><span data-stu-id="e03f8-191">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="e03f8-192">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="e03f8-192">enterpriseProxiedDomains</span></span>|<span data-ttu-id="e03f8-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="e03f8-194">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e03f8-194">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="e03f8-195">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="e03f8-195">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="e03f8-196">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="e03f8-196">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="e03f8-197">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります</span><span class="sxs-lookup"><span data-stu-id="e03f8-197">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="e03f8-198">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="e03f8-198">enterpriseIPRanges</span></span>|<span data-ttu-id="e03f8-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="e03f8-200">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="e03f8-200">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="e03f8-201">これらのコンピューターからのデータはエンタープライズの一部とみなされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="e03f8-201">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="e03f8-202">これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます</span><span class="sxs-lookup"><span data-stu-id="e03f8-202">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="e03f8-203">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="e03f8-203">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="e03f8-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="e03f8-204">Boolean</span></span>|<span data-ttu-id="e03f8-205">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="e03f8-205">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="e03f8-206">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="e03f8-206">Default is false</span></span>|
|<span data-ttu-id="e03f8-207">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="e03f8-207">enterpriseProxyServers</span></span>|<span data-ttu-id="e03f8-208">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-208">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e03f8-209">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="e03f8-209">This is a list of proxy servers.</span></span> <span data-ttu-id="e03f8-210">このリストにないサーバーは、非エンタープライズとみなされます</span><span class="sxs-lookup"><span data-stu-id="e03f8-210">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="e03f8-211">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="e03f8-211">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="e03f8-212">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-212">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e03f8-213">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="e03f8-213">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="e03f8-214">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="e03f8-214">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="e03f8-215">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="e03f8-215">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="e03f8-216">それらはエンタープライズ ネットワークの場所にあるとみなされます。</span><span class="sxs-lookup"><span data-stu-id="e03f8-216">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="e03f8-217">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します</span><span class="sxs-lookup"><span data-stu-id="e03f8-217">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="e03f8-218">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="e03f8-218">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="e03f8-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="e03f8-219">Boolean</span></span>|<span data-ttu-id="e03f8-220">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="e03f8-220">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="e03f8-221">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="e03f8-221">Default is false</span></span>|
|<span data-ttu-id="e03f8-222">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="e03f8-222">neutralDomainResources</span></span>|<span data-ttu-id="e03f8-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e03f8-224">職場または個人のリソースに使用できるドメイン名のリスト</span><span class="sxs-lookup"><span data-stu-id="e03f8-224">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="e03f8-225">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="e03f8-225">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="e03f8-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="e03f8-226">Boolean</span></span>|<span data-ttu-id="e03f8-227">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します</span><span class="sxs-lookup"><span data-stu-id="e03f8-227">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="e03f8-228">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="e03f8-228">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="e03f8-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e03f8-230">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します</span><span class="sxs-lookup"><span data-stu-id="e03f8-230">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="e03f8-231">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e03f8-231">isAssigned</span></span>|<span data-ttu-id="e03f8-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e03f8-232">Boolean</span></span>|<span data-ttu-id="e03f8-233">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e03f8-233">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e03f8-234">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e03f8-234">Relationships</span></span>
|<span data-ttu-id="e03f8-235">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e03f8-235">Relationship</span></span>|<span data-ttu-id="e03f8-236">型</span><span class="sxs-lookup"><span data-stu-id="e03f8-236">Type</span></span>|<span data-ttu-id="e03f8-237">説明</span><span class="sxs-lookup"><span data-stu-id="e03f8-237">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e03f8-238">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="e03f8-238">protectedAppLockerFiles</span></span>|<span data-ttu-id="e03f8-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="e03f8-240">xml ファイルを使用して、保護されたアプリを入力する別の方法</span><span class="sxs-lookup"><span data-stu-id="e03f8-240">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="e03f8-241">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="e03f8-241">exemptAppLockerFiles</span></span>|<span data-ttu-id="e03f8-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="e03f8-243">xml ファイルを使用して、適用除外アプリを入力する別の方法</span><span class="sxs-lookup"><span data-stu-id="e03f8-243">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="e03f8-244">assignments</span><span class="sxs-lookup"><span data-stu-id="e03f8-244">assignments</span></span>|<span data-ttu-id="e03f8-245">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e03f8-245">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e03f8-246">ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="e03f8-246">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e03f8-247">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e03f8-247">JSON Representation</span></span>
<span data-ttu-id="e03f8-248">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e03f8-248">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```



