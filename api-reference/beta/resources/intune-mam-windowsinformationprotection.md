---
title: windowsInformationProtection リソース タイプ
description: 詳細な管理設定を構成するための Windows 情報保護のポリシー
author: tfitzmac
ms.openlocfilehash: 5d4d36e0b4be5c5549c9ff1120756f8e851c2869
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304320"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="9ed59-103">windowsInformationProtection リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="9ed59-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="9ed59-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ed59-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ed59-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ed59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ed59-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ed59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ed59-107">詳細な管理設定を構成するための Windows 情報保護のポリシー</span><span class="sxs-lookup"><span data-stu-id="9ed59-107">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="9ed59-108">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ed59-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9ed59-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ed59-109">Methods</span></span>
|<span data-ttu-id="9ed59-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ed59-110">Method</span></span>|<span data-ttu-id="9ed59-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9ed59-111">Return Type</span></span>|<span data-ttu-id="9ed59-112">説明</span><span class="sxs-lookup"><span data-stu-id="9ed59-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ed59-113">List windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="9ed59-113">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="9ed59-114">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-114">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="9ed59-115">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9ed59-115">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="9ed59-116">Get windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="9ed59-116">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="9ed59-117">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="9ed59-117">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="9ed59-118">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9ed59-118">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="9ed59-119">assign action</span><span class="sxs-lookup"><span data-stu-id="9ed59-119">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="9ed59-120">なし</span><span class="sxs-lookup"><span data-stu-id="9ed59-120">None</span></span>|<span data-ttu-id="9ed59-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9ed59-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9ed59-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ed59-122">Properties</span></span>
|<span data-ttu-id="9ed59-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ed59-123">Property</span></span>|<span data-ttu-id="9ed59-124">種類</span><span class="sxs-lookup"><span data-stu-id="9ed59-124">Type</span></span>|<span data-ttu-id="9ed59-125">説明</span><span class="sxs-lookup"><span data-stu-id="9ed59-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ed59-126">displayName</span><span class="sxs-lookup"><span data-stu-id="9ed59-126">displayName</span></span>|<span data-ttu-id="9ed59-127">String</span><span class="sxs-lookup"><span data-stu-id="9ed59-127">String</span></span>|<span data-ttu-id="9ed59-128">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="9ed59-128">Policy display name.</span></span> <span data-ttu-id="9ed59-129">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ed59-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ed59-130">説明</span><span class="sxs-lookup"><span data-stu-id="9ed59-130">description</span></span>|<span data-ttu-id="9ed59-131">String</span><span class="sxs-lookup"><span data-stu-id="9ed59-131">String</span></span>|<span data-ttu-id="9ed59-132">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="9ed59-132">The policy's description.</span></span> <span data-ttu-id="9ed59-133">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ed59-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ed59-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ed59-134">createdDateTime</span></span>|<span data-ttu-id="9ed59-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ed59-135">DateTimeOffset</span></span>|<span data-ttu-id="9ed59-136">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="9ed59-136">The date and time the policy was created.</span></span> <span data-ttu-id="9ed59-137">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ed59-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ed59-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ed59-138">lastModifiedDateTime</span></span>|<span data-ttu-id="9ed59-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ed59-139">DateTimeOffset</span></span>|<span data-ttu-id="9ed59-140">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="9ed59-140">Last time the policy was modified.</span></span> <span data-ttu-id="9ed59-141">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ed59-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ed59-142">id</span><span class="sxs-lookup"><span data-stu-id="9ed59-142">id</span></span>|<span data-ttu-id="9ed59-143">String</span><span class="sxs-lookup"><span data-stu-id="9ed59-143">String</span></span>|<span data-ttu-id="9ed59-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9ed59-144">Key of the entity.</span></span> <span data-ttu-id="9ed59-145">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ed59-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ed59-146">version</span><span class="sxs-lookup"><span data-stu-id="9ed59-146">version</span></span>|<span data-ttu-id="9ed59-147">String</span><span class="sxs-lookup"><span data-stu-id="9ed59-147">String</span></span>|<span data-ttu-id="9ed59-148">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="9ed59-148">Version of the entity.</span></span> <span data-ttu-id="9ed59-149">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ed59-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ed59-150">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="9ed59-150">enforcementLevel</span></span>|[<span data-ttu-id="9ed59-151">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="9ed59-151">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="9ed59-152">WIP の適用レベルです。サポートされている値の列挙型定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ed59-152">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="9ed59-153">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="9ed59-153">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="9ed59-154">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="9ed59-154">enterpriseDomain</span></span>|<span data-ttu-id="9ed59-155">String</span><span class="sxs-lookup"><span data-stu-id="9ed59-155">String</span></span>|<span data-ttu-id="9ed59-156">プライマリ エンタープライズ ドメイン</span><span class="sxs-lookup"><span data-stu-id="9ed59-156">Primary enterprise domain</span></span>|
|<span data-ttu-id="9ed59-157">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="9ed59-157">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="9ed59-158">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-158">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9ed59-159">保護するエンタープライズ ドメインのリスト</span><span class="sxs-lookup"><span data-stu-id="9ed59-159">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="9ed59-160">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="9ed59-160">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="9ed59-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed59-161">Boolean</span></span>|<span data-ttu-id="9ed59-162">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="9ed59-162">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="9ed59-163">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9ed59-163">dataRecoveryCertificate</span></span>|[<span data-ttu-id="9ed59-164">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9ed59-164">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="9ed59-165">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ed59-165">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="9ed59-166">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです。</span><span class="sxs-lookup"><span data-stu-id="9ed59-166">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="9ed59-167">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="9ed59-167">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="9ed59-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed59-168">Boolean</span></span>|<span data-ttu-id="9ed59-169">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="9ed59-169">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="9ed59-170">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="9ed59-170">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="9ed59-171">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="9ed59-171">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="9ed59-172">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="9ed59-172">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="9ed59-173">Guid</span><span class="sxs-lookup"><span data-stu-id="9ed59-173">Guid</span></span>|<span data-ttu-id="9ed59-174">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="9ed59-174">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="9ed59-175">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーとアクセスできる期間について、詳細を構成することができます</span><span class="sxs-lookup"><span data-stu-id="9ed59-175">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="9ed59-176">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="9ed59-176">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="9ed59-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed59-177">Boolean</span></span>|<span data-ttu-id="9ed59-178">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="9ed59-178">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="9ed59-179">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="9ed59-179">iconsVisible</span></span>|<span data-ttu-id="9ed59-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed59-180">Boolean</span></span>|<span data-ttu-id="9ed59-181">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="9ed59-181">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="9ed59-182">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します</span><span class="sxs-lookup"><span data-stu-id="9ed59-182">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="9ed59-183">protectedApps</span><span class="sxs-lookup"><span data-stu-id="9ed59-183">protectedApps</span></span>|<span data-ttu-id="9ed59-184">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-184">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="9ed59-185">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます</span><span class="sxs-lookup"><span data-stu-id="9ed59-185">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="9ed59-186">exemptApps</span><span class="sxs-lookup"><span data-stu-id="9ed59-186">exemptApps</span></span>|<span data-ttu-id="9ed59-187">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-187">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="9ed59-188">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="9ed59-188">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="9ed59-189">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="9ed59-189">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="9ed59-190">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="9ed59-190">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="9ed59-191">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-191">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9ed59-192">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="9ed59-192">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="9ed59-193">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データとみなされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます</span><span class="sxs-lookup"><span data-stu-id="9ed59-193">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="9ed59-194">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="9ed59-194">enterpriseProxiedDomains</span></span>|<span data-ttu-id="9ed59-195">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-195">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="9ed59-196">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ed59-196">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="9ed59-197">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="9ed59-197">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="9ed59-198">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="9ed59-198">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="9ed59-199">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります</span><span class="sxs-lookup"><span data-stu-id="9ed59-199">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="9ed59-200">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="9ed59-200">enterpriseIPRanges</span></span>|<span data-ttu-id="9ed59-201">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-201">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="9ed59-202">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="9ed59-202">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="9ed59-203">これらのコンピューターからのデータはエンタープライズの一部とみなされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="9ed59-203">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="9ed59-204">これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます</span><span class="sxs-lookup"><span data-stu-id="9ed59-204">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="9ed59-205">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9ed59-205">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="9ed59-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed59-206">Boolean</span></span>|<span data-ttu-id="9ed59-207">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="9ed59-207">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="9ed59-208">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="9ed59-208">Default is false</span></span>|
|<span data-ttu-id="9ed59-209">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="9ed59-209">enterpriseProxyServers</span></span>|<span data-ttu-id="9ed59-210">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-210">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9ed59-211">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="9ed59-211">This is a list of proxy servers.</span></span> <span data-ttu-id="9ed59-212">このリストにないサーバーは、非エンタープライズとみなされます</span><span class="sxs-lookup"><span data-stu-id="9ed59-212">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="9ed59-213">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="9ed59-213">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="9ed59-214">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-214">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9ed59-215">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="9ed59-215">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="9ed59-216">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="9ed59-216">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="9ed59-217">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="9ed59-217">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="9ed59-218">それらはエンタープライズ ネットワークの場所にあるとみなされます。</span><span class="sxs-lookup"><span data-stu-id="9ed59-218">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="9ed59-219">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します</span><span class="sxs-lookup"><span data-stu-id="9ed59-219">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="9ed59-220">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9ed59-220">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="9ed59-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed59-221">Boolean</span></span>|<span data-ttu-id="9ed59-222">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="9ed59-222">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="9ed59-223">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="9ed59-223">Default is false</span></span>|
|<span data-ttu-id="9ed59-224">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="9ed59-224">neutralDomainResources</span></span>|<span data-ttu-id="9ed59-225">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-225">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9ed59-226">職場または個人のリソースに使用できるドメイン名のリスト</span><span class="sxs-lookup"><span data-stu-id="9ed59-226">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="9ed59-227">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="9ed59-227">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="9ed59-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed59-228">Boolean</span></span>|<span data-ttu-id="9ed59-229">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します</span><span class="sxs-lookup"><span data-stu-id="9ed59-229">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="9ed59-230">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="9ed59-230">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="9ed59-231">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-231">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9ed59-232">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します</span><span class="sxs-lookup"><span data-stu-id="9ed59-232">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="9ed59-233">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9ed59-233">isAssigned</span></span>|<span data-ttu-id="9ed59-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed59-234">Boolean</span></span>|<span data-ttu-id="9ed59-235">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ed59-235">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ed59-236">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9ed59-236">Relationships</span></span>
|<span data-ttu-id="9ed59-237">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9ed59-237">Relationship</span></span>|<span data-ttu-id="9ed59-238">型</span><span class="sxs-lookup"><span data-stu-id="9ed59-238">Type</span></span>|<span data-ttu-id="9ed59-239">説明</span><span class="sxs-lookup"><span data-stu-id="9ed59-239">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ed59-240">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="9ed59-240">protectedAppLockerFiles</span></span>|<span data-ttu-id="9ed59-241">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-241">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="9ed59-242">xml ファイルを使用して、保護されたアプリを入力する別の方法</span><span class="sxs-lookup"><span data-stu-id="9ed59-242">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="9ed59-243">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="9ed59-243">exemptAppLockerFiles</span></span>|<span data-ttu-id="9ed59-244">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-244">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="9ed59-245">xml ファイルを使用して、適用除外アプリを入力する別の方法</span><span class="sxs-lookup"><span data-stu-id="9ed59-245">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="9ed59-246">assignments</span><span class="sxs-lookup"><span data-stu-id="9ed59-246">assignments</span></span>|<span data-ttu-id="9ed59-247">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ed59-247">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="9ed59-248">ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="9ed59-248">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ed59-249">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ed59-249">JSON Representation</span></span>
<span data-ttu-id="9ed59-250">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9ed59-250">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
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





