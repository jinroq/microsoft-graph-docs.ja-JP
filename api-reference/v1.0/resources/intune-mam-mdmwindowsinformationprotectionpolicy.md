---
title: mdmWindowsInformationProtectionPolicy リソース タイプ
description: MDM を使用する Windows 情報保護のポリシー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c47936a64e6f09f47592c025dc3e55aeec267164
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037857"
---
# <a name="mdmwindowsinformationprotectionpolicy-resource-type"></a><span data-ttu-id="5b429-103">mdmWindowsInformationProtectionPolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="5b429-103">mdmWindowsInformationProtectionPolicy resource type</span></span>

> <span data-ttu-id="5b429-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b429-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b429-105">MDM を使用する Windows 情報保護のポリシー</span><span class="sxs-lookup"><span data-stu-id="5b429-105">Policy for Windows information protection with MDM</span></span>


<span data-ttu-id="5b429-106">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-106">Inherits from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5b429-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b429-107">Methods</span></span>
|<span data-ttu-id="5b429-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b429-108">Method</span></span>|<span data-ttu-id="5b429-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5b429-109">Return Type</span></span>|<span data-ttu-id="5b429-110">説明</span><span class="sxs-lookup"><span data-stu-id="5b429-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5b429-111">List mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="5b429-111">List mdmWindowsInformationProtectionPolicies</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-list.md)|<span data-ttu-id="5b429-112">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-112">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="5b429-113">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5b429-113">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>|
|[<span data-ttu-id="5b429-114">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5b429-114">Get mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-get.md)|[<span data-ttu-id="5b429-115">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5b429-115">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="5b429-116">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5b429-116">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="5b429-117">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5b429-117">Create mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-create.md)|[<span data-ttu-id="5b429-118">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5b429-118">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="5b429-119">新しい [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5b429-119">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="5b429-120">Delete mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5b429-120">Delete mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-delete.md)|<span data-ttu-id="5b429-121">なし</span><span class="sxs-lookup"><span data-stu-id="5b429-121">None</span></span>|<span data-ttu-id="5b429-122">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5b429-122">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>|
|[<span data-ttu-id="5b429-123">Update mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5b429-123">Update mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-update.md)|[<span data-ttu-id="5b429-124">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5b429-124">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="5b429-125">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5b429-125">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b429-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b429-126">Properties</span></span>
|<span data-ttu-id="5b429-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b429-127">Property</span></span>|<span data-ttu-id="5b429-128">型</span><span class="sxs-lookup"><span data-stu-id="5b429-128">Type</span></span>|<span data-ttu-id="5b429-129">説明</span><span class="sxs-lookup"><span data-stu-id="5b429-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b429-130">displayName</span><span class="sxs-lookup"><span data-stu-id="5b429-130">displayName</span></span>|<span data-ttu-id="5b429-131">String</span><span class="sxs-lookup"><span data-stu-id="5b429-131">String</span></span>|<span data-ttu-id="5b429-132">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="5b429-132">Policy display name.</span></span> <span data-ttu-id="5b429-133">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b429-134">description</span><span class="sxs-lookup"><span data-stu-id="5b429-134">description</span></span>|<span data-ttu-id="5b429-135">String</span><span class="sxs-lookup"><span data-stu-id="5b429-135">String</span></span>|<span data-ttu-id="5b429-136">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="5b429-136">The policy's description.</span></span> <span data-ttu-id="5b429-137">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b429-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b429-138">createdDateTime</span></span>|<span data-ttu-id="5b429-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b429-139">DateTimeOffset</span></span>|<span data-ttu-id="5b429-140">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="5b429-140">The date and time the policy was created.</span></span> <span data-ttu-id="5b429-141">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b429-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b429-142">lastModifiedDateTime</span></span>|<span data-ttu-id="5b429-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b429-143">DateTimeOffset</span></span>|<span data-ttu-id="5b429-144">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="5b429-144">Last time the policy was modified.</span></span> <span data-ttu-id="5b429-145">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b429-146">id</span><span class="sxs-lookup"><span data-stu-id="5b429-146">id</span></span>|<span data-ttu-id="5b429-147">文字列</span><span class="sxs-lookup"><span data-stu-id="5b429-147">String</span></span>|<span data-ttu-id="5b429-148">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5b429-148">Key of the entity.</span></span> <span data-ttu-id="5b429-149">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b429-150">version</span><span class="sxs-lookup"><span data-stu-id="5b429-150">version</span></span>|<span data-ttu-id="5b429-151">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5b429-151">String</span></span>|<span data-ttu-id="5b429-152">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="5b429-152">Version of the entity.</span></span> <span data-ttu-id="5b429-153">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b429-154">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="5b429-154">enforcementLevel</span></span>|[<span data-ttu-id="5b429-155">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="5b429-155">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="5b429-156">仕掛品の実施レベル。[Windowsinformationprotection](../resources/intune-mam-windowsinformationprotection.md)から継承した、サポートされている値の列挙定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b429-156">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="5b429-157">使用可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="5b429-157">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="5b429-158">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="5b429-158">enterpriseDomain</span></span>|<span data-ttu-id="5b429-159">String</span><span class="sxs-lookup"><span data-stu-id="5b429-159">String</span></span>|<span data-ttu-id="5b429-160">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-160">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-161">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="5b429-161">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="5b429-162">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-162">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="5b429-163">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-163">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-164">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="5b429-164">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="5b429-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b429-165">Boolean</span></span>|<span data-ttu-id="5b429-166">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-166">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-167">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="5b429-167">dataRecoveryCertificate</span></span>|[<span data-ttu-id="5b429-168">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="5b429-168">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="5b429-169">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b429-169">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="5b429-170">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-170">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-171">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="5b429-171">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="5b429-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b429-172">Boolean</span></span>|<span data-ttu-id="5b429-173">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="5b429-173">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="5b429-174">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5b429-174">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="5b429-175">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="5b429-175">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="5b429-176">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-176">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-177">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="5b429-177">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="5b429-178">GUID</span><span class="sxs-lookup"><span data-stu-id="5b429-178">Guid</span></span>|<span data-ttu-id="5b429-179">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="5b429-179">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="5b429-180">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-180">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-181">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="5b429-181">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="5b429-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b429-182">Boolean</span></span>|<span data-ttu-id="5b429-183">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-183">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-184">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="5b429-184">iconsVisible</span></span>|<span data-ttu-id="5b429-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b429-185">Boolean</span></span>|<span data-ttu-id="5b429-186">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="5b429-186">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="5b429-187">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-187">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-188">protectedApps</span><span class="sxs-lookup"><span data-stu-id="5b429-188">protectedApps</span></span>|<span data-ttu-id="5b429-189">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-189">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="5b429-190">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-190">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-191">exemptApps</span><span class="sxs-lookup"><span data-stu-id="5b429-191">exemptApps</span></span>|<span data-ttu-id="5b429-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="5b429-193">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="5b429-193">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="5b429-194">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="5b429-194">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="5b429-195">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-195">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-196">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="5b429-196">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="5b429-197">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-197">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="5b429-198">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="5b429-198">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="5b429-199">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-199">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-200">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="5b429-200">enterpriseProxiedDomains</span></span>|<span data-ttu-id="5b429-201">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-201">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="5b429-202">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b429-202">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="5b429-203">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="5b429-203">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="5b429-204">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="5b429-204">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="5b429-205">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-205">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-206">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="5b429-206">enterpriseIPRanges</span></span>|<span data-ttu-id="5b429-207">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-207">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="5b429-208">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="5b429-208">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="5b429-209">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="5b429-209">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="5b429-210">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-210">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-211">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="5b429-211">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="5b429-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b429-212">Boolean</span></span>|<span data-ttu-id="5b429-213">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="5b429-213">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="5b429-214">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-214">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-215">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="5b429-215">enterpriseProxyServers</span></span>|<span data-ttu-id="5b429-216">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-216">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="5b429-217">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="5b429-217">This is a list of proxy servers.</span></span> <span data-ttu-id="5b429-218">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-218">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-219">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="5b429-219">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="5b429-220">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-220">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="5b429-221">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="5b429-221">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="5b429-222">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="5b429-222">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="5b429-223">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="5b429-223">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="5b429-224">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="5b429-224">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="5b429-225">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-225">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-226">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="5b429-226">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="5b429-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b429-227">Boolean</span></span>|<span data-ttu-id="5b429-228">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="5b429-228">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="5b429-229">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-229">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-230">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="5b429-230">neutralDomainResources</span></span>|<span data-ttu-id="5b429-231">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-231">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="5b429-232">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-232">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-233">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="5b429-233">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="5b429-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b429-234">Boolean</span></span>|<span data-ttu-id="5b429-235">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-235">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-236">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="5b429-236">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="5b429-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="5b429-238">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-238">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-239">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5b429-239">isAssigned</span></span>|<span data-ttu-id="5b429-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b429-240">Boolean</span></span>|<span data-ttu-id="5b429-241">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b429-241">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="5b429-242">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-242">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b429-243">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b429-243">Relationships</span></span>
|<span data-ttu-id="5b429-244">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b429-244">Relationship</span></span>|<span data-ttu-id="5b429-245">型</span><span class="sxs-lookup"><span data-stu-id="5b429-245">Type</span></span>|<span data-ttu-id="5b429-246">説明</span><span class="sxs-lookup"><span data-stu-id="5b429-246">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b429-247">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="5b429-247">protectedAppLockerFiles</span></span>|<span data-ttu-id="5b429-248">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-248">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="5b429-249">xml ファイルを使用して、保護されたアプリを入力する別の方法 ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-249">Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-250">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="5b429-250">exemptAppLockerFiles</span></span>|<span data-ttu-id="5b429-251">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-251">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="5b429-252">xml ファイルを使用して、保護されていないアプリを入力する別の方法 ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="5b429-252">Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="5b429-253">assignments</span><span class="sxs-lookup"><span data-stu-id="5b429-253">assignments</span></span>|<span data-ttu-id="5b429-254">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b429-254">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="5b429-255">ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="5b429-255">Navigation property to list of security groups targeted for policy.</span></span> <span data-ttu-id="5b429-256">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b429-256">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b429-257">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b429-257">JSON Representation</span></span>
<span data-ttu-id="5b429-258">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b429-258">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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



