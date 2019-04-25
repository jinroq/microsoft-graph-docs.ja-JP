---
title: Create mdmWindowsInformationProtectionPolicy
description: 新しい mdmWindowsInformationProtectionPolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67a1238695edf6178a87f746c8393bc6668788b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525720"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="e69b8-103">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e69b8-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="e69b8-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e69b8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e69b8-105">新しい [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-105">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e69b8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e69b8-106">Prerequisites</span></span>
<span data-ttu-id="e69b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e69b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e69b8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e69b8-109">Permission type</span></span>|<span data-ttu-id="e69b8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e69b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e69b8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e69b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e69b8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e69b8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e69b8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e69b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e69b8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e69b8-114">Not supported.</span></span>|
|<span data-ttu-id="e69b8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e69b8-115">Application</span></span>|<span data-ttu-id="e69b8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e69b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e69b8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e69b8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e69b8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e69b8-118">Request headers</span></span>
|<span data-ttu-id="e69b8-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e69b8-119">Header</span></span>|<span data-ttu-id="e69b8-120">値</span><span class="sxs-lookup"><span data-stu-id="e69b8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e69b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e69b8-121">Authorization</span></span>|<span data-ttu-id="e69b8-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e69b8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e69b8-123">承諾</span><span class="sxs-lookup"><span data-stu-id="e69b8-123">Accept</span></span>|<span data-ttu-id="e69b8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e69b8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e69b8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e69b8-125">Request body</span></span>
<span data-ttu-id="e69b8-126">要求の本文に、mdmWindowsInformationProtectionPolicy オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-126">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="e69b8-127">次の表に、mdmWindowsInformationProtectionPolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-127">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="e69b8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e69b8-128">Property</span></span>|<span data-ttu-id="e69b8-129">型</span><span class="sxs-lookup"><span data-stu-id="e69b8-129">Type</span></span>|<span data-ttu-id="e69b8-130">説明</span><span class="sxs-lookup"><span data-stu-id="e69b8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e69b8-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e69b8-131">displayName</span></span>|<span data-ttu-id="e69b8-132">String</span><span class="sxs-lookup"><span data-stu-id="e69b8-132">String</span></span>|<span data-ttu-id="e69b8-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="e69b8-133">Policy display name.</span></span> <span data-ttu-id="e69b8-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e69b8-135">description</span><span class="sxs-lookup"><span data-stu-id="e69b8-135">description</span></span>|<span data-ttu-id="e69b8-136">String</span><span class="sxs-lookup"><span data-stu-id="e69b8-136">String</span></span>|<span data-ttu-id="e69b8-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="e69b8-137">The policy's description.</span></span> <span data-ttu-id="e69b8-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e69b8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e69b8-139">createdDateTime</span></span>|<span data-ttu-id="e69b8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e69b8-140">DateTimeOffset</span></span>|<span data-ttu-id="e69b8-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e69b8-141">The date and time the policy was created.</span></span> <span data-ttu-id="e69b8-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e69b8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e69b8-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e69b8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e69b8-144">DateTimeOffset</span></span>|<span data-ttu-id="e69b8-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="e69b8-145">Last time the policy was modified.</span></span> <span data-ttu-id="e69b8-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e69b8-147">id</span><span class="sxs-lookup"><span data-stu-id="e69b8-147">id</span></span>|<span data-ttu-id="e69b8-148">String</span><span class="sxs-lookup"><span data-stu-id="e69b8-148">String</span></span>|<span data-ttu-id="e69b8-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e69b8-149">Key of the entity.</span></span> <span data-ttu-id="e69b8-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e69b8-151">version</span><span class="sxs-lookup"><span data-stu-id="e69b8-151">version</span></span>|<span data-ttu-id="e69b8-152">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e69b8-152">String</span></span>|<span data-ttu-id="e69b8-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e69b8-153">Version of the entity.</span></span> <span data-ttu-id="e69b8-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e69b8-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="e69b8-155">enforcementLevel</span></span>|[<span data-ttu-id="e69b8-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="e69b8-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="e69b8-157">仕掛品の実施レベル。[windowsinformationprotection](../resources/intune-mam-windowsinformationprotection.md)から継承した、サポートされている値の列挙定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e69b8-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="e69b8-158">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="e69b8-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="e69b8-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="e69b8-159">enterpriseDomain</span></span>|<span data-ttu-id="e69b8-160">String</span><span class="sxs-lookup"><span data-stu-id="e69b8-160">String</span></span>|<span data-ttu-id="e69b8-161">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="e69b8-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="e69b8-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e69b8-164">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="e69b8-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="e69b8-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="e69b8-166">Boolean</span></span>|<span data-ttu-id="e69b8-167">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="e69b8-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="e69b8-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="e69b8-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="e69b8-170">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="e69b8-171">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="e69b8-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="e69b8-173">ブール値</span><span class="sxs-lookup"><span data-stu-id="e69b8-173">Boolean</span></span>|<span data-ttu-id="e69b8-174">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="e69b8-175">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e69b8-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="e69b8-176">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="e69b8-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="e69b8-177">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="e69b8-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="e69b8-179">GUID</span><span class="sxs-lookup"><span data-stu-id="e69b8-179">Guid</span></span>|<span data-ttu-id="e69b8-180">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="e69b8-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="e69b8-181">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="e69b8-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="e69b8-183">ブール値</span><span class="sxs-lookup"><span data-stu-id="e69b8-183">Boolean</span></span>|<span data-ttu-id="e69b8-184">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="e69b8-185">iconsVisible</span></span>|<span data-ttu-id="e69b8-186">ブール値</span><span class="sxs-lookup"><span data-stu-id="e69b8-186">Boolean</span></span>|<span data-ttu-id="e69b8-187">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="e69b8-188">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="e69b8-189">protectedApps</span></span>|<span data-ttu-id="e69b8-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="e69b8-191">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="e69b8-192">exemptApps</span></span>|<span data-ttu-id="e69b8-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="e69b8-194">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="e69b8-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="e69b8-195">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="e69b8-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="e69b8-196">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="e69b8-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="e69b8-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e69b8-199">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="e69b8-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="e69b8-200">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="e69b8-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="e69b8-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="e69b8-203">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e69b8-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="e69b8-204">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="e69b8-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="e69b8-205">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="e69b8-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="e69b8-206">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="e69b8-207">enterpriseIPRanges</span></span>|<span data-ttu-id="e69b8-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="e69b8-209">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="e69b8-210">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="e69b8-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="e69b8-211">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="e69b8-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="e69b8-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e69b8-213">Boolean</span></span>|<span data-ttu-id="e69b8-214">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="e69b8-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="e69b8-215">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="e69b8-216">enterpriseProxyServers</span></span>|<span data-ttu-id="e69b8-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e69b8-218">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="e69b8-218">This is a list of proxy servers.</span></span> <span data-ttu-id="e69b8-219">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="e69b8-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="e69b8-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e69b8-222">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="e69b8-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="e69b8-223">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="e69b8-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="e69b8-224">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="e69b8-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="e69b8-225">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="e69b8-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="e69b8-226">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="e69b8-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="e69b8-228">ブール値</span><span class="sxs-lookup"><span data-stu-id="e69b8-228">Boolean</span></span>|<span data-ttu-id="e69b8-229">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="e69b8-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="e69b8-230">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="e69b8-231">neutralDomainResources</span></span>|<span data-ttu-id="e69b8-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e69b8-233">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="e69b8-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="e69b8-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="e69b8-235">Boolean</span></span>|<span data-ttu-id="e69b8-236">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="e69b8-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="e69b8-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e69b8-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e69b8-239">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e69b8-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e69b8-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e69b8-240">isAssigned</span></span>|<span data-ttu-id="e69b8-241">ブール値</span><span class="sxs-lookup"><span data-stu-id="e69b8-241">Boolean</span></span>|<span data-ttu-id="e69b8-242">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="e69b8-243">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e69b8-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e69b8-244">応答</span><span class="sxs-lookup"><span data-stu-id="e69b8-244">Response</span></span>
<span data-ttu-id="e69b8-245">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e69b8-245">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e69b8-246">例</span><span class="sxs-lookup"><span data-stu-id="e69b8-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="e69b8-247">要求</span><span class="sxs-lookup"><span data-stu-id="e69b8-247">Request</span></span>
<span data-ttu-id="e69b8-248">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e69b8-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3905

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="e69b8-249">応答</span><span class="sxs-lookup"><span data-stu-id="e69b8-249">Response</span></span>
<span data-ttu-id="e69b8-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e69b8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4077

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true
}
```



