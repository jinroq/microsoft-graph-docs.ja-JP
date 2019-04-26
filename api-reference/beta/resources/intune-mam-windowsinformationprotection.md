---
title: windowsInformationProtection リソース タイプ
description: 詳細な管理設定を構成するための Windows 情報保護のポリシー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1caee1df6dd010d0f5a12e4da61dc33953dd6c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563568"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="6b7e7-103">windowsInformationProtection リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="6b7e7-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="6b7e7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b7e7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b7e7-106">詳細な管理設定を構成するための Windows 情報保護のポリシー</span><span class="sxs-lookup"><span data-stu-id="6b7e7-106">Policy for Windows information protection to configure detailed management settings</span></span>


<span data-ttu-id="6b7e7-107">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6b7e7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6b7e7-108">Methods</span></span>
|<span data-ttu-id="6b7e7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6b7e7-109">Method</span></span>|<span data-ttu-id="6b7e7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6b7e7-110">Return Type</span></span>|<span data-ttu-id="6b7e7-111">説明</span><span class="sxs-lookup"><span data-stu-id="6b7e7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b7e7-112">List windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="6b7e7-112">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="6b7e7-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="6b7e7-114">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-114">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="6b7e7-115">Get windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="6b7e7-115">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="6b7e7-116">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="6b7e7-116">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="6b7e7-117">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-117">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="6b7e7-118">assign action</span><span class="sxs-lookup"><span data-stu-id="6b7e7-118">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="6b7e7-119">なし</span><span class="sxs-lookup"><span data-stu-id="6b7e7-119">None</span></span>|<span data-ttu-id="6b7e7-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6b7e7-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6b7e7-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b7e7-121">Properties</span></span>
|<span data-ttu-id="6b7e7-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b7e7-122">Property</span></span>|<span data-ttu-id="6b7e7-123">型</span><span class="sxs-lookup"><span data-stu-id="6b7e7-123">Type</span></span>|<span data-ttu-id="6b7e7-124">説明</span><span class="sxs-lookup"><span data-stu-id="6b7e7-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b7e7-125">displayName</span><span class="sxs-lookup"><span data-stu-id="6b7e7-125">displayName</span></span>|<span data-ttu-id="6b7e7-126">String</span><span class="sxs-lookup"><span data-stu-id="6b7e7-126">String</span></span>|<span data-ttu-id="6b7e7-127">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-127">Policy display name.</span></span> <span data-ttu-id="6b7e7-128">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6b7e7-129">説明</span><span class="sxs-lookup"><span data-stu-id="6b7e7-129">description</span></span>|<span data-ttu-id="6b7e7-130">String</span><span class="sxs-lookup"><span data-stu-id="6b7e7-130">String</span></span>|<span data-ttu-id="6b7e7-131">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-131">The policy's description.</span></span> <span data-ttu-id="6b7e7-132">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6b7e7-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b7e7-133">createdDateTime</span></span>|<span data-ttu-id="6b7e7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b7e7-134">DateTimeOffset</span></span>|<span data-ttu-id="6b7e7-135">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-135">The date and time the policy was created.</span></span> <span data-ttu-id="6b7e7-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6b7e7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b7e7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6b7e7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b7e7-138">DateTimeOffset</span></span>|<span data-ttu-id="6b7e7-139">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-139">Last time the policy was modified.</span></span> <span data-ttu-id="6b7e7-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6b7e7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b7e7-141">roleScopeTagIds</span></span>|<span data-ttu-id="6b7e7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="6b7e7-142">String collection</span></span>|<span data-ttu-id="6b7e7-143">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b7e7-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6b7e7-145">id</span><span class="sxs-lookup"><span data-stu-id="6b7e7-145">id</span></span>|<span data-ttu-id="6b7e7-146">String</span><span class="sxs-lookup"><span data-stu-id="6b7e7-146">String</span></span>|<span data-ttu-id="6b7e7-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-147">Key of the entity.</span></span> <span data-ttu-id="6b7e7-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6b7e7-149">version</span><span class="sxs-lookup"><span data-stu-id="6b7e7-149">version</span></span>|<span data-ttu-id="6b7e7-150">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6b7e7-150">String</span></span>|<span data-ttu-id="6b7e7-151">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-151">Version of the entity.</span></span> <span data-ttu-id="6b7e7-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6b7e7-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="6b7e7-153">enforcementLevel</span></span>|[<span data-ttu-id="6b7e7-154">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="6b7e7-154">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="6b7e7-155">仕掛品の実施レベル。サポートされている値については、Enum 定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-155">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="6b7e7-156">使用可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-156">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="6b7e7-157">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="6b7e7-157">enterpriseDomain</span></span>|<span data-ttu-id="6b7e7-158">String</span><span class="sxs-lookup"><span data-stu-id="6b7e7-158">String</span></span>|<span data-ttu-id="6b7e7-159">プライマリ エンタープライズ ドメイン</span><span class="sxs-lookup"><span data-stu-id="6b7e7-159">Primary enterprise domain</span></span>|
|<span data-ttu-id="6b7e7-160">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="6b7e7-160">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="6b7e7-161">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-161">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6b7e7-162">保護するエンタープライズ ドメインのリスト</span><span class="sxs-lookup"><span data-stu-id="6b7e7-162">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="6b7e7-163">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="6b7e7-163">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="6b7e7-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b7e7-164">Boolean</span></span>|<span data-ttu-id="6b7e7-165">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-165">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="6b7e7-166">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="6b7e7-166">dataRecoveryCertificate</span></span>|[<span data-ttu-id="6b7e7-167">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="6b7e7-167">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="6b7e7-168">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-168">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="6b7e7-169">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-169">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="6b7e7-170">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="6b7e7-170">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="6b7e7-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b7e7-171">Boolean</span></span>|<span data-ttu-id="6b7e7-172">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-172">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="6b7e7-173">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-173">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="6b7e7-174">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-174">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="6b7e7-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="6b7e7-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="6b7e7-176">GUID</span><span class="sxs-lookup"><span data-stu-id="6b7e7-176">Guid</span></span>|<span data-ttu-id="6b7e7-177">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="6b7e7-178">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーとアクセスできる期間について、詳細を構成することができます</span><span class="sxs-lookup"><span data-stu-id="6b7e7-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="6b7e7-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="6b7e7-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="6b7e7-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b7e7-180">Boolean</span></span>|<span data-ttu-id="6b7e7-181">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-181">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="6b7e7-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="6b7e7-182">iconsVisible</span></span>|<span data-ttu-id="6b7e7-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b7e7-183">Boolean</span></span>|<span data-ttu-id="6b7e7-184">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="6b7e7-185">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="6b7e7-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="6b7e7-186">protectedApps</span></span>|<span data-ttu-id="6b7e7-187">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-187">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="6b7e7-188">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます</span><span class="sxs-lookup"><span data-stu-id="6b7e7-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="6b7e7-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="6b7e7-189">exemptApps</span></span>|<span data-ttu-id="6b7e7-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="6b7e7-191">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="6b7e7-192">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="6b7e7-193">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="6b7e7-193">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="6b7e7-194">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-194">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6b7e7-195">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-195">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="6b7e7-196">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データとみなされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます</span><span class="sxs-lookup"><span data-stu-id="6b7e7-196">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="6b7e7-197">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="6b7e7-197">enterpriseProxiedDomains</span></span>|<span data-ttu-id="6b7e7-198">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-198">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="6b7e7-199">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-199">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="6b7e7-200">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-200">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="6b7e7-201">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-201">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="6b7e7-202">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります</span><span class="sxs-lookup"><span data-stu-id="6b7e7-202">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="6b7e7-203">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="6b7e7-203">enterpriseIPRanges</span></span>|<span data-ttu-id="6b7e7-204">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-204">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="6b7e7-205">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-205">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="6b7e7-206">これらのコンピューターからのデータはエンタープライズの一部とみなされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-206">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="6b7e7-207">これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます</span><span class="sxs-lookup"><span data-stu-id="6b7e7-207">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="6b7e7-208">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="6b7e7-208">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="6b7e7-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b7e7-209">Boolean</span></span>|<span data-ttu-id="6b7e7-210">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-210">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="6b7e7-211">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="6b7e7-211">Default is false</span></span>|
|<span data-ttu-id="6b7e7-212">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="6b7e7-212">enterpriseProxyServers</span></span>|<span data-ttu-id="6b7e7-213">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-213">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6b7e7-214">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-214">This is a list of proxy servers.</span></span> <span data-ttu-id="6b7e7-215">このリストにないサーバーは、非エンタープライズとみなされます</span><span class="sxs-lookup"><span data-stu-id="6b7e7-215">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="6b7e7-216">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="6b7e7-216">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="6b7e7-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6b7e7-218">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-218">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="6b7e7-219">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-219">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="6b7e7-220">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-220">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="6b7e7-221">それらはエンタープライズ ネットワークの場所にあるとみなされます。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-221">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="6b7e7-222">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-222">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="6b7e7-223">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="6b7e7-223">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="6b7e7-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b7e7-224">Boolean</span></span>|<span data-ttu-id="6b7e7-225">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-225">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="6b7e7-226">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="6b7e7-226">Default is false</span></span>|
|<span data-ttu-id="6b7e7-227">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="6b7e7-227">neutralDomainResources</span></span>|<span data-ttu-id="6b7e7-228">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-228">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6b7e7-229">職場または個人のリソースに使用できるドメイン名のリスト</span><span class="sxs-lookup"><span data-stu-id="6b7e7-229">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="6b7e7-230">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="6b7e7-230">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="6b7e7-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b7e7-231">Boolean</span></span>|<span data-ttu-id="6b7e7-232">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-232">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="6b7e7-233">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="6b7e7-233">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="6b7e7-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6b7e7-235">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します</span><span class="sxs-lookup"><span data-stu-id="6b7e7-235">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="6b7e7-236">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6b7e7-236">isAssigned</span></span>|<span data-ttu-id="6b7e7-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b7e7-237">Boolean</span></span>|<span data-ttu-id="6b7e7-238">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-238">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b7e7-239">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6b7e7-239">Relationships</span></span>
|<span data-ttu-id="6b7e7-240">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6b7e7-240">Relationship</span></span>|<span data-ttu-id="6b7e7-241">型</span><span class="sxs-lookup"><span data-stu-id="6b7e7-241">Type</span></span>|<span data-ttu-id="6b7e7-242">説明</span><span class="sxs-lookup"><span data-stu-id="6b7e7-242">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b7e7-243">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="6b7e7-243">protectedAppLockerFiles</span></span>|<span data-ttu-id="6b7e7-244">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-244">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="6b7e7-245">xml ファイルを使用して、保護されたアプリを入力する別の方法</span><span class="sxs-lookup"><span data-stu-id="6b7e7-245">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="6b7e7-246">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="6b7e7-246">exemptAppLockerFiles</span></span>|<span data-ttu-id="6b7e7-247">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-247">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="6b7e7-248">xml ファイルを使用して、適用除外アプリを入力する別の方法</span><span class="sxs-lookup"><span data-stu-id="6b7e7-248">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="6b7e7-249">assignments</span><span class="sxs-lookup"><span data-stu-id="6b7e7-249">assignments</span></span>|<span data-ttu-id="6b7e7-250">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b7e7-250">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="6b7e7-251">ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-251">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b7e7-252">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b7e7-252">JSON Representation</span></span>
<span data-ttu-id="6b7e7-253">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6b7e7-253">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
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





