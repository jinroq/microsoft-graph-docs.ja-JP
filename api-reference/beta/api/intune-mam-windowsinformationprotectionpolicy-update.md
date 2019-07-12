---
title: Update windowsInformationProtectionPolicy
description: windowsInformationProtectionPolicy オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e417f7444e60c7d021c4bb3a88a610e5f6884da
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639096"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="fe070-103">Update windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fe070-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="fe070-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe070-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe070-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe070-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe070-106">[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fe070-106">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe070-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fe070-107">Prerequisites</span></span>
<span data-ttu-id="fe070-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe070-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe070-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe070-110">Permission type</span></span>|<span data-ttu-id="fe070-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe070-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe070-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe070-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe070-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe070-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe070-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe070-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe070-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe070-115">Not supported.</span></span>|
|<span data-ttu-id="fe070-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe070-116">Application</span></span>|<span data-ttu-id="fe070-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe070-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe070-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe070-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fe070-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe070-119">Request headers</span></span>
|<span data-ttu-id="fe070-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe070-120">Header</span></span>|<span data-ttu-id="fe070-121">値</span><span class="sxs-lookup"><span data-stu-id="fe070-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe070-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe070-122">Authorization</span></span>|<span data-ttu-id="fe070-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe070-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe070-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fe070-124">Accept</span></span>|<span data-ttu-id="fe070-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe070-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe070-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe070-126">Request body</span></span>
<span data-ttu-id="fe070-127">要求の本文に、[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe070-127">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="fe070-128">次の表に、[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fe070-128">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="fe070-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe070-129">Property</span></span>|<span data-ttu-id="fe070-130">型</span><span class="sxs-lookup"><span data-stu-id="fe070-130">Type</span></span>|<span data-ttu-id="fe070-131">説明</span><span class="sxs-lookup"><span data-stu-id="fe070-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe070-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fe070-132">displayName</span></span>|<span data-ttu-id="fe070-133">String</span><span class="sxs-lookup"><span data-stu-id="fe070-133">String</span></span>|<span data-ttu-id="fe070-134">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="fe070-134">Policy display name.</span></span> <span data-ttu-id="fe070-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fe070-136">description</span><span class="sxs-lookup"><span data-stu-id="fe070-136">description</span></span>|<span data-ttu-id="fe070-137">String</span><span class="sxs-lookup"><span data-stu-id="fe070-137">String</span></span>|<span data-ttu-id="fe070-138">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="fe070-138">The policy's description.</span></span> <span data-ttu-id="fe070-139">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fe070-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe070-140">createdDateTime</span></span>|<span data-ttu-id="fe070-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe070-141">DateTimeOffset</span></span>|<span data-ttu-id="fe070-142">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="fe070-142">The date and time the policy was created.</span></span> <span data-ttu-id="fe070-143">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fe070-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe070-144">lastModifiedDateTime</span></span>|<span data-ttu-id="fe070-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe070-145">DateTimeOffset</span></span>|<span data-ttu-id="fe070-146">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="fe070-146">Last time the policy was modified.</span></span> <span data-ttu-id="fe070-147">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fe070-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe070-148">roleScopeTagIds</span></span>|<span data-ttu-id="fe070-149">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-149">String collection</span></span>|<span data-ttu-id="fe070-150">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="fe070-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fe070-151">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fe070-152">id</span><span class="sxs-lookup"><span data-stu-id="fe070-152">id</span></span>|<span data-ttu-id="fe070-153">文字列</span><span class="sxs-lookup"><span data-stu-id="fe070-153">String</span></span>|<span data-ttu-id="fe070-154">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fe070-154">Key of the entity.</span></span> <span data-ttu-id="fe070-155">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fe070-156">version</span><span class="sxs-lookup"><span data-stu-id="fe070-156">version</span></span>|<span data-ttu-id="fe070-157">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fe070-157">String</span></span>|<span data-ttu-id="fe070-158">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="fe070-158">Version of the entity.</span></span> <span data-ttu-id="fe070-159">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fe070-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fe070-160">enforcementLevel</span></span>|[<span data-ttu-id="fe070-161">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fe070-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="fe070-162">仕掛品の実施レベル。[Windowsinformationprotection](../resources/intune-mam-windowsinformationprotection.md)から継承した、サポートされている値の列挙定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe070-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="fe070-163">使用可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="fe070-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="fe070-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="fe070-164">enterpriseDomain</span></span>|<span data-ttu-id="fe070-165">String</span><span class="sxs-lookup"><span data-stu-id="fe070-165">String</span></span>|<span data-ttu-id="fe070-166">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="fe070-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="fe070-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fe070-169">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="fe070-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="fe070-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-171">Boolean</span></span>|<span data-ttu-id="fe070-172">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fe070-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="fe070-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fe070-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="fe070-175">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe070-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="fe070-176">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="fe070-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="fe070-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-178">Boolean</span></span>|<span data-ttu-id="fe070-179">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="fe070-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="fe070-180">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="fe070-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="fe070-181">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="fe070-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="fe070-182">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="fe070-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="fe070-184">GUID</span><span class="sxs-lookup"><span data-stu-id="fe070-184">Guid</span></span>|<span data-ttu-id="fe070-185">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="fe070-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="fe070-186">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="fe070-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="fe070-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-188">Boolean</span></span>|<span data-ttu-id="fe070-189">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="fe070-190">iconsVisible</span></span>|<span data-ttu-id="fe070-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-191">Boolean</span></span>|<span data-ttu-id="fe070-192">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="fe070-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="fe070-193">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="fe070-194">protectedApps</span></span>|<span data-ttu-id="fe070-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fe070-196">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="fe070-197">exemptApps</span></span>|<span data-ttu-id="fe070-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fe070-199">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="fe070-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="fe070-200">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="fe070-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="fe070-201">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="fe070-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="fe070-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fe070-204">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="fe070-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="fe070-205">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="fe070-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="fe070-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="fe070-208">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fe070-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="fe070-209">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="fe070-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="fe070-210">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="fe070-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="fe070-211">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="fe070-212">enterpriseIPRanges</span></span>|<span data-ttu-id="fe070-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="fe070-214">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="fe070-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="fe070-215">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="fe070-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="fe070-216">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fe070-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="fe070-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-218">Boolean</span></span>|<span data-ttu-id="fe070-219">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="fe070-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="fe070-220">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="fe070-221">enterpriseProxyServers</span></span>|<span data-ttu-id="fe070-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fe070-223">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="fe070-223">This is a list of proxy servers.</span></span> <span data-ttu-id="fe070-224">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="fe070-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="fe070-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fe070-227">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="fe070-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="fe070-228">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="fe070-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="fe070-229">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="fe070-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="fe070-230">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="fe070-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="fe070-231">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fe070-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="fe070-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-233">Boolean</span></span>|<span data-ttu-id="fe070-234">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="fe070-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="fe070-235">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="fe070-236">neutralDomainResources</span></span>|<span data-ttu-id="fe070-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fe070-238">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="fe070-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="fe070-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-240">Boolean</span></span>|<span data-ttu-id="fe070-241">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="fe070-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="fe070-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe070-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fe070-244">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fe070-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fe070-245">isAssigned</span></span>|<span data-ttu-id="fe070-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-246">Boolean</span></span>|<span data-ttu-id="fe070-247">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fe070-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="fe070-248">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe070-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fe070-249">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="fe070-249">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="fe070-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-250">Boolean</span></span>|<span data-ttu-id="fe070-251">RS2 の新しいプロパティ、保留中のドキュメント</span><span class="sxs-lookup"><span data-stu-id="fe070-251">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="fe070-252">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="fe070-252">mdmEnrollmentUrl</span></span>|<span data-ttu-id="fe070-253">String</span><span class="sxs-lookup"><span data-stu-id="fe070-253">String</span></span>|<span data-ttu-id="fe070-254">MDM の登録 URL</span><span class="sxs-lookup"><span data-stu-id="fe070-254">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="fe070-255">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="fe070-255">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="fe070-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe070-256">Boolean</span></span>|<span data-ttu-id="fe070-257">Windows にサインインするためのメソッドとして Windows Hello for Business を設定するブール値です。</span><span class="sxs-lookup"><span data-stu-id="fe070-257">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="fe070-258">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fe070-258">pinMinimumLength</span></span>|<span data-ttu-id="fe070-259">Int32</span><span class="sxs-lookup"><span data-stu-id="fe070-259">Int32</span></span>|<span data-ttu-id="fe070-260">PIN に必要な文字の最小数を設定する整数値です。</span><span class="sxs-lookup"><span data-stu-id="fe070-260">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="fe070-261">既定値は 4 です。</span><span class="sxs-lookup"><span data-stu-id="fe070-261">Default value is 4.</span></span> <span data-ttu-id="fe070-262">このポリシー設定で構成できる最小値は 4 です。</span><span class="sxs-lookup"><span data-stu-id="fe070-262">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="fe070-263">構成できる最大値は、[PIN の最大文字数] ポリシー設定で構成された値、または 127 のうち、どちらか小さい方です。</span><span class="sxs-lookup"><span data-stu-id="fe070-263">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="fe070-264">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="fe070-264">pinUppercaseLetters</span></span>|[<span data-ttu-id="fe070-265">Windowsinformationprotectionpin文字の要件</span><span class="sxs-lookup"><span data-stu-id="fe070-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="fe070-266">Windows Hello for Business の PIN における大文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="fe070-266">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fe070-267">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="fe070-267">Default is NotAllow.</span></span> <span data-ttu-id="fe070-268">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="fe070-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="fe070-269">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="fe070-269">pinLowercaseLetters</span></span>|[<span data-ttu-id="fe070-270">Windowsinformationprotectionpin文字の要件</span><span class="sxs-lookup"><span data-stu-id="fe070-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="fe070-271">Windows Hello for Business の PIN における小文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="fe070-271">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fe070-272">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="fe070-272">Default is NotAllow.</span></span> <span data-ttu-id="fe070-273">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="fe070-273">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="fe070-274">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="fe070-274">pinSpecialCharacters</span></span>|[<span data-ttu-id="fe070-275">Windowsinformationprotectionpin文字の要件</span><span class="sxs-lookup"><span data-stu-id="fe070-275">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="fe070-276">Windows Hello for Business の PIN における特殊文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="fe070-276">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fe070-277">Windows Hello for Business の PIN ジェスチャの有効な特殊文字は以下のとおりです: !</span><span class="sxs-lookup"><span data-stu-id="fe070-277">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="fe070-278">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="fe070-278">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="fe070-279">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="fe070-279">/ : ; < = > ?</span></span><span data-ttu-id="fe070-280"> @ \[ \ \]^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="fe070-280"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="fe070-281">} ~。</span><span class="sxs-lookup"><span data-stu-id="fe070-281">} ~.</span></span> <span data-ttu-id="fe070-282">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="fe070-282">Default is NotAllow.</span></span> <span data-ttu-id="fe070-283">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="fe070-283">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="fe070-284">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fe070-284">pinExpirationDays</span></span>|<span data-ttu-id="fe070-285">Int32</span><span class="sxs-lookup"><span data-stu-id="fe070-285">Int32</span></span>|<span data-ttu-id="fe070-286">この整数値は、システムがユーザーに PIN の変更を要求する前の、PIN の使用可能な期間 (日数) を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe070-286">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="fe070-287">このポリシー設定で構成できる最大値は 730 です。</span><span class="sxs-lookup"><span data-stu-id="fe070-287">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="fe070-288">このポリシー設定で構成できる最小値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="fe070-288">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="fe070-289">このポリシーが 0 に設定されている場合、ユーザーの PIN は期限切れになりません。</span><span class="sxs-lookup"><span data-stu-id="fe070-289">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="fe070-290">このノードは、Windows 10 バージョン 1511 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="fe070-290">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="fe070-291">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="fe070-291">Default is 0.</span></span>|
|<span data-ttu-id="fe070-292">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="fe070-292">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="fe070-293">Int32</span><span class="sxs-lookup"><span data-stu-id="fe070-293">Int32</span></span>|<span data-ttu-id="fe070-294">再使用できないユーザー アカウントに関連付けられる過去の PIN の数を指定する整数値です。</span><span class="sxs-lookup"><span data-stu-id="fe070-294">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="fe070-295">このポリシー設定で構成できる最大値は 50 です。</span><span class="sxs-lookup"><span data-stu-id="fe070-295">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="fe070-296">このポリシー設定で構成できる最小値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="fe070-296">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="fe070-297">このポリシーが 0 に設定されている場合、以前の PIN の格納は不要です。</span><span class="sxs-lookup"><span data-stu-id="fe070-297">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="fe070-298">このノードは、Windows 10 バージョン 1511 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="fe070-298">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="fe070-299">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="fe070-299">Default is 0.</span></span>|
|<span data-ttu-id="fe070-300">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="fe070-300">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="fe070-301">Int32</span><span class="sxs-lookup"><span data-stu-id="fe070-301">Int32</span></span>|<span data-ttu-id="fe070-302">デバイスがワイプされるまでの、許可されている認証失敗の回数です。</span><span class="sxs-lookup"><span data-stu-id="fe070-302">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="fe070-303">値を 0 にすると、デバイス ワイプ機能が無効になります。</span><span class="sxs-lookup"><span data-stu-id="fe070-303">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="fe070-304">範囲は整数 X (デスクトップの場合: 4 <= X <= 16、モバイル デバイスの場合: 0 <= X <= 999) です。</span><span class="sxs-lookup"><span data-stu-id="fe070-304">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="fe070-305">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="fe070-305">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="fe070-306">Int32</span><span class="sxs-lookup"><span data-stu-id="fe070-306">Int32</span></span>|<span data-ttu-id="fe070-307">デバイスがアイドルになった後に、デバイスの PIN またはパスワードがロックされるまでの最大時間 (分) を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe070-307">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="fe070-308">範囲は整数 X (0 < = X < = 999) です。</span><span class="sxs-lookup"><span data-stu-id="fe070-308">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="fe070-309">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="fe070-309">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="fe070-310">Int32</span><span class="sxs-lookup"><span data-stu-id="fe070-310">Int32</span></span>|<span data-ttu-id="fe070-311">アプリのデータがワイプされるまでのオフライン期間 (日数)</span><span class="sxs-lookup"><span data-stu-id="fe070-311">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="fe070-312">応答</span><span class="sxs-lookup"><span data-stu-id="fe070-312">Response</span></span>
<span data-ttu-id="fe070-313">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="fe070-313">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe070-314">例</span><span class="sxs-lookup"><span data-stu-id="fe070-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe070-315">要求</span><span class="sxs-lookup"><span data-stu-id="fe070-315">Request</span></span>
<span data-ttu-id="fe070-316">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe070-316">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4467

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```

### <a name="response"></a><span data-ttu-id="fe070-317">応答</span><span class="sxs-lookup"><span data-stu-id="fe070-317">Response</span></span>
<span data-ttu-id="fe070-p132">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe070-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4639

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "6397be61-be61-6397-61be-976361be9763",
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
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```





