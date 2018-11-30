---
title: Update windowsInformationProtectionPolicy
description: windowsInformationProtectionPolicy オブジェクトのプロパティを更新します。
ms.openlocfilehash: 15fc74d9f5155fdda9513812ab0dbbdb6770c879
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023846"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="4138d-103">Update windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="4138d-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="4138d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4138d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4138d-105">[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4138d-105">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4138d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4138d-106">Prerequisites</span></span>
<span data-ttu-id="4138d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4138d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4138d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4138d-109">Permission type</span></span>|<span data-ttu-id="4138d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4138d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4138d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4138d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4138d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4138d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4138d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4138d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4138d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4138d-114">Not supported.</span></span>|
|<span data-ttu-id="4138d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4138d-115">Application</span></span>|<span data-ttu-id="4138d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4138d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4138d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4138d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4138d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4138d-118">Request headers</span></span>
|<span data-ttu-id="4138d-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4138d-119">Header</span></span>|<span data-ttu-id="4138d-120">値</span><span class="sxs-lookup"><span data-stu-id="4138d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4138d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4138d-121">Authorization</span></span>|<span data-ttu-id="4138d-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4138d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4138d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4138d-123">Accept</span></span>|<span data-ttu-id="4138d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4138d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4138d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4138d-125">Request body</span></span>
<span data-ttu-id="4138d-126">要求の本文に、[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="4138d-126">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="4138d-127">次の表に、[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4138d-127">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="4138d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4138d-128">Property</span></span>|<span data-ttu-id="4138d-129">型</span><span class="sxs-lookup"><span data-stu-id="4138d-129">Type</span></span>|<span data-ttu-id="4138d-130">説明</span><span class="sxs-lookup"><span data-stu-id="4138d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4138d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="4138d-131">displayName</span></span>|<span data-ttu-id="4138d-132">String</span><span class="sxs-lookup"><span data-stu-id="4138d-132">String</span></span>|<span data-ttu-id="4138d-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="4138d-133">Policy display name.</span></span> <span data-ttu-id="4138d-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4138d-135">説明</span><span class="sxs-lookup"><span data-stu-id="4138d-135">description</span></span>|<span data-ttu-id="4138d-136">String</span><span class="sxs-lookup"><span data-stu-id="4138d-136">String</span></span>|<span data-ttu-id="4138d-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="4138d-137">The policy's description.</span></span> <span data-ttu-id="4138d-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4138d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4138d-139">createdDateTime</span></span>|<span data-ttu-id="4138d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4138d-140">DateTimeOffset</span></span>|<span data-ttu-id="4138d-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4138d-141">The date and time the policy was created.</span></span> <span data-ttu-id="4138d-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4138d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4138d-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4138d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4138d-144">DateTimeOffset</span></span>|<span data-ttu-id="4138d-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="4138d-145">Last time the policy was modified.</span></span> <span data-ttu-id="4138d-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4138d-147">id</span><span class="sxs-lookup"><span data-stu-id="4138d-147">id</span></span>|<span data-ttu-id="4138d-148">String</span><span class="sxs-lookup"><span data-stu-id="4138d-148">String</span></span>|<span data-ttu-id="4138d-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4138d-149">Key of the entity.</span></span> <span data-ttu-id="4138d-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4138d-151">version</span><span class="sxs-lookup"><span data-stu-id="4138d-151">version</span></span>|<span data-ttu-id="4138d-152">String</span><span class="sxs-lookup"><span data-stu-id="4138d-152">String</span></span>|<span data-ttu-id="4138d-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4138d-153">Version of the entity.</span></span> <span data-ttu-id="4138d-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4138d-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="4138d-155">enforcementLevel</span></span>|[<span data-ttu-id="4138d-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="4138d-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="4138d-157">WIP の適用レベルです。[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)からサポートされている値継承の列挙型定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4138d-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="4138d-158">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="4138d-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="4138d-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="4138d-159">enterpriseDomain</span></span>|<span data-ttu-id="4138d-160">String</span><span class="sxs-lookup"><span data-stu-id="4138d-160">String</span></span>|<span data-ttu-id="4138d-161">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="4138d-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="4138d-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4138d-164">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="4138d-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="4138d-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-166">Boolean</span></span>|<span data-ttu-id="4138d-167">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4138d-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="4138d-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4138d-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="4138d-170">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="4138d-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="4138d-171">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="4138d-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="4138d-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-173">Boolean</span></span>|<span data-ttu-id="4138d-174">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="4138d-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="4138d-175">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="4138d-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="4138d-176">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="4138d-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="4138d-177">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="4138d-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="4138d-179">Guid</span><span class="sxs-lookup"><span data-stu-id="4138d-179">Guid</span></span>|<span data-ttu-id="4138d-180">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="4138d-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="4138d-181">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="4138d-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="4138d-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-183">Boolean</span></span>|<span data-ttu-id="4138d-184">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="4138d-185">iconsVisible</span></span>|<span data-ttu-id="4138d-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-186">Boolean</span></span>|<span data-ttu-id="4138d-187">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="4138d-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="4138d-188">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="4138d-189">protectedApps</span></span>|<span data-ttu-id="4138d-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="4138d-191">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="4138d-192">exemptApps</span></span>|<span data-ttu-id="4138d-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="4138d-194">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="4138d-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="4138d-195">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="4138d-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="4138d-196">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="4138d-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="4138d-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4138d-199">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="4138d-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="4138d-200">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="4138d-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="4138d-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="4138d-203">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4138d-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="4138d-204">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="4138d-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="4138d-205">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="4138d-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="4138d-206">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="4138d-207">enterpriseIPRanges</span></span>|<span data-ttu-id="4138d-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="4138d-209">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="4138d-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="4138d-210">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="4138d-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="4138d-211">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="4138d-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="4138d-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-213">Boolean</span></span>|<span data-ttu-id="4138d-214">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="4138d-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="4138d-215">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="4138d-216">enterpriseProxyServers</span></span>|<span data-ttu-id="4138d-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4138d-218">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="4138d-218">This is a list of proxy servers.</span></span> <span data-ttu-id="4138d-219">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="4138d-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="4138d-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4138d-222">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="4138d-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="4138d-223">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="4138d-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="4138d-224">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="4138d-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="4138d-225">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="4138d-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="4138d-226">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="4138d-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="4138d-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-228">Boolean</span></span>|<span data-ttu-id="4138d-229">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="4138d-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="4138d-230">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="4138d-231">neutralDomainResources</span></span>|<span data-ttu-id="4138d-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4138d-233">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="4138d-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="4138d-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-235">Boolean</span></span>|<span data-ttu-id="4138d-236">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="4138d-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="4138d-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4138d-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4138d-239">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4138d-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4138d-240">isAssigned</span></span>|<span data-ttu-id="4138d-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-241">Boolean</span></span>|<span data-ttu-id="4138d-242">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4138d-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="4138d-243">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4138d-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4138d-244">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="4138d-244">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="4138d-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-245">Boolean</span></span>|<span data-ttu-id="4138d-246">RS2 の新しいプロパティ、保留中のドキュメント</span><span class="sxs-lookup"><span data-stu-id="4138d-246">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="4138d-247">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="4138d-247">mdmEnrollmentUrl</span></span>|<span data-ttu-id="4138d-248">String</span><span class="sxs-lookup"><span data-stu-id="4138d-248">String</span></span>|<span data-ttu-id="4138d-249">MDM の登録 URL</span><span class="sxs-lookup"><span data-stu-id="4138d-249">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="4138d-250">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="4138d-250">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="4138d-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="4138d-251">Boolean</span></span>|<span data-ttu-id="4138d-252">Windows にサインインするためのメソッドとして Windows Hello for Business を設定するブール値です。</span><span class="sxs-lookup"><span data-stu-id="4138d-252">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="4138d-253">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4138d-253">pinMinimumLength</span></span>|<span data-ttu-id="4138d-254">Int32</span><span class="sxs-lookup"><span data-stu-id="4138d-254">Int32</span></span>|<span data-ttu-id="4138d-255">PIN に必要な文字の最小数を設定する整数値です。</span><span class="sxs-lookup"><span data-stu-id="4138d-255">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="4138d-256">既定値は 4 です。</span><span class="sxs-lookup"><span data-stu-id="4138d-256">Default value is 4.</span></span> <span data-ttu-id="4138d-257">このポリシー設定で構成できる最小値は 4 です。</span><span class="sxs-lookup"><span data-stu-id="4138d-257">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="4138d-258">構成できる最大値は、[PIN の最大文字数] ポリシー設定で構成された値、または 127 のうち、どちらか小さい方です。</span><span class="sxs-lookup"><span data-stu-id="4138d-258">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="4138d-259">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="4138d-259">pinUppercaseLetters</span></span>|[<span data-ttu-id="4138d-260">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="4138d-260">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="4138d-261">Windows Hello for Business の PIN における大文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="4138d-261">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4138d-262">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="4138d-262">Default is NotAllow.</span></span> <span data-ttu-id="4138d-263">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="4138d-263">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="4138d-264">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="4138d-264">pinLowercaseLetters</span></span>|[<span data-ttu-id="4138d-265">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="4138d-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="4138d-266">Windows Hello for Business の PIN における小文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="4138d-266">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4138d-267">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="4138d-267">Default is NotAllow.</span></span> <span data-ttu-id="4138d-268">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="4138d-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="4138d-269">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="4138d-269">pinSpecialCharacters</span></span>|[<span data-ttu-id="4138d-270">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="4138d-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="4138d-271">Windows Hello for Business の PIN における特殊文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="4138d-271">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4138d-272">Windows Hello for Business の PIN ジェスチャの有効な特殊文字は以下のとおりです: !</span><span class="sxs-lookup"><span data-stu-id="4138d-272">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="4138d-273">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="4138d-273">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="4138d-274">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="4138d-274">/ : ; < = > ?</span></span><span data-ttu-id="4138d-275"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="4138d-275"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="4138d-276">} ~。</span><span class="sxs-lookup"><span data-stu-id="4138d-276">} ~.</span></span> <span data-ttu-id="4138d-277">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="4138d-277">Default is NotAllow.</span></span> <span data-ttu-id="4138d-278">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="4138d-278">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="4138d-279">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4138d-279">pinExpirationDays</span></span>|<span data-ttu-id="4138d-280">Int32</span><span class="sxs-lookup"><span data-stu-id="4138d-280">Int32</span></span>|<span data-ttu-id="4138d-281">この整数値は、システムがユーザーに PIN の変更を要求する前の、PIN の使用可能な期間 (日数) を指定します。</span><span class="sxs-lookup"><span data-stu-id="4138d-281">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="4138d-282">このポリシー設定で構成できる最大値は 730 です。</span><span class="sxs-lookup"><span data-stu-id="4138d-282">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="4138d-283">このポリシー設定で構成できる最小値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="4138d-283">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="4138d-284">このポリシーが 0 に設定されている場合、ユーザーの PIN は期限切れになりません。</span><span class="sxs-lookup"><span data-stu-id="4138d-284">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="4138d-285">このノードは、Windows 10 バージョン 1511 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="4138d-285">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="4138d-286">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="4138d-286">Default is 0.</span></span>|
|<span data-ttu-id="4138d-287">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="4138d-287">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="4138d-288">Int32</span><span class="sxs-lookup"><span data-stu-id="4138d-288">Int32</span></span>|<span data-ttu-id="4138d-289">再使用できないユーザー アカウントに関連付けられる過去の PIN の数を指定する整数値です。</span><span class="sxs-lookup"><span data-stu-id="4138d-289">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="4138d-290">このポリシー設定で構成できる最大値は 50 です。</span><span class="sxs-lookup"><span data-stu-id="4138d-290">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="4138d-291">このポリシー設定で構成できる最小値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="4138d-291">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="4138d-292">このポリシーが 0 に設定されている場合、以前の PIN の格納は不要です。</span><span class="sxs-lookup"><span data-stu-id="4138d-292">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="4138d-293">このノードは、Windows 10 バージョン 1511 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="4138d-293">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="4138d-294">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="4138d-294">Default is 0.</span></span>|
|<span data-ttu-id="4138d-295">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="4138d-295">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="4138d-296">Int32</span><span class="sxs-lookup"><span data-stu-id="4138d-296">Int32</span></span>|<span data-ttu-id="4138d-297">デバイスがワイプされるまでの、許可されている認証失敗の回数です。</span><span class="sxs-lookup"><span data-stu-id="4138d-297">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="4138d-298">値を 0 にすると、デバイス ワイプ機能が無効になります。</span><span class="sxs-lookup"><span data-stu-id="4138d-298">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="4138d-299">範囲は整数 X (デスクトップの場合: 4 <= X <= 16、モバイル デバイスの場合: 0 <= X <= 999) です。</span><span class="sxs-lookup"><span data-stu-id="4138d-299">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="4138d-300">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="4138d-300">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="4138d-301">Int32</span><span class="sxs-lookup"><span data-stu-id="4138d-301">Int32</span></span>|<span data-ttu-id="4138d-302">デバイスがアイドルになった後に、デバイスの PIN またはパスワードがロックされるまでの最大時間 (分) を指定します。</span><span class="sxs-lookup"><span data-stu-id="4138d-302">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="4138d-303">範囲は整数 X (0 < = X < = 999) です。</span><span class="sxs-lookup"><span data-stu-id="4138d-303">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="4138d-304">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="4138d-304">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="4138d-305">Int32</span><span class="sxs-lookup"><span data-stu-id="4138d-305">Int32</span></span>|<span data-ttu-id="4138d-306">アプリのデータがワイプされるまでのオフライン期間 (日数)</span><span class="sxs-lookup"><span data-stu-id="4138d-306">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="4138d-307">応答</span><span class="sxs-lookup"><span data-stu-id="4138d-307">Response</span></span>
<span data-ttu-id="4138d-308">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="4138d-308">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4138d-309">例</span><span class="sxs-lookup"><span data-stu-id="4138d-309">Example</span></span>
### <a name="request"></a><span data-ttu-id="4138d-310">要求</span><span class="sxs-lookup"><span data-stu-id="4138d-310">Request</span></span>
<span data-ttu-id="4138d-311">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4138d-311">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4405

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
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

### <a name="response"></a><span data-ttu-id="4138d-312">応答</span><span class="sxs-lookup"><span data-stu-id="4138d-312">Response</span></span>
<span data-ttu-id="4138d-p131">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4138d-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4577

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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


