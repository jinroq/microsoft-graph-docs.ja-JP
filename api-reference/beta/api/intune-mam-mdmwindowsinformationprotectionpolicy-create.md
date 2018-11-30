---
title: Create mdmWindowsInformationProtectionPolicy
description: 新しい mdmWindowsInformationProtectionPolicy オブジェクトを作成します。
ms.openlocfilehash: 4546a44e859c768303179335e54787f892f6d594
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068868"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="c0b94-103">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0b94-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="c0b94-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0b94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0b94-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0b94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0b94-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0b94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0b94-107">新しい [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-107">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0b94-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c0b94-108">Prerequisites</span></span>
<span data-ttu-id="c0b94-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0b94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b94-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0b94-111">Permission type</span></span>|<span data-ttu-id="c0b94-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0b94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0b94-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0b94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0b94-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b94-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0b94-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0b94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0b94-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0b94-116">Not supported.</span></span>|
|<span data-ttu-id="c0b94-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0b94-117">Application</span></span>|<span data-ttu-id="c0b94-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0b94-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0b94-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0b94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c0b94-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0b94-120">Request headers</span></span>
|<span data-ttu-id="c0b94-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0b94-121">Header</span></span>|<span data-ttu-id="c0b94-122">値</span><span class="sxs-lookup"><span data-stu-id="c0b94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0b94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0b94-123">Authorization</span></span>|<span data-ttu-id="c0b94-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c0b94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0b94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0b94-125">Accept</span></span>|<span data-ttu-id="c0b94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0b94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0b94-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0b94-127">Request body</span></span>
<span data-ttu-id="c0b94-128">要求の本文に、mdmWindowsInformationProtectionPolicy オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-128">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="c0b94-129">次の表に、mdmWindowsInformationProtectionPolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-129">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="c0b94-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0b94-130">Property</span></span>|<span data-ttu-id="c0b94-131">型</span><span class="sxs-lookup"><span data-stu-id="c0b94-131">Type</span></span>|<span data-ttu-id="c0b94-132">説明</span><span class="sxs-lookup"><span data-stu-id="c0b94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b94-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c0b94-133">displayName</span></span>|<span data-ttu-id="c0b94-134">String</span><span class="sxs-lookup"><span data-stu-id="c0b94-134">String</span></span>|<span data-ttu-id="c0b94-135">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="c0b94-135">Policy display name.</span></span> <span data-ttu-id="c0b94-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0b94-137">説明</span><span class="sxs-lookup"><span data-stu-id="c0b94-137">description</span></span>|<span data-ttu-id="c0b94-138">String</span><span class="sxs-lookup"><span data-stu-id="c0b94-138">String</span></span>|<span data-ttu-id="c0b94-139">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="c0b94-139">The policy's description.</span></span> <span data-ttu-id="c0b94-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0b94-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b94-141">createdDateTime</span></span>|<span data-ttu-id="c0b94-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b94-142">DateTimeOffset</span></span>|<span data-ttu-id="c0b94-143">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c0b94-143">The date and time the policy was created.</span></span> <span data-ttu-id="c0b94-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0b94-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b94-145">lastModifiedDateTime</span></span>|<span data-ttu-id="c0b94-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b94-146">DateTimeOffset</span></span>|<span data-ttu-id="c0b94-147">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="c0b94-147">Last time the policy was modified.</span></span> <span data-ttu-id="c0b94-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0b94-149">id</span><span class="sxs-lookup"><span data-stu-id="c0b94-149">id</span></span>|<span data-ttu-id="c0b94-150">String</span><span class="sxs-lookup"><span data-stu-id="c0b94-150">String</span></span>|<span data-ttu-id="c0b94-151">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c0b94-151">Key of the entity.</span></span> <span data-ttu-id="c0b94-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0b94-153">version</span><span class="sxs-lookup"><span data-stu-id="c0b94-153">version</span></span>|<span data-ttu-id="c0b94-154">String</span><span class="sxs-lookup"><span data-stu-id="c0b94-154">String</span></span>|<span data-ttu-id="c0b94-155">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c0b94-155">Version of the entity.</span></span> <span data-ttu-id="c0b94-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0b94-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="c0b94-157">enforcementLevel</span></span>|[<span data-ttu-id="c0b94-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="c0b94-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="c0b94-159">WIP の適用レベルです。[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)からサポートされている値継承の列挙型定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0b94-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="c0b94-160">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="c0b94-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="c0b94-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="c0b94-161">enterpriseDomain</span></span>|<span data-ttu-id="c0b94-162">String</span><span class="sxs-lookup"><span data-stu-id="c0b94-162">String</span></span>|<span data-ttu-id="c0b94-163">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="c0b94-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="c0b94-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c0b94-166">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="c0b94-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="c0b94-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b94-168">Boolean</span></span>|<span data-ttu-id="c0b94-169">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="c0b94-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="c0b94-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="c0b94-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="c0b94-172">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="c0b94-173">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="c0b94-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="c0b94-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b94-175">Boolean</span></span>|<span data-ttu-id="c0b94-176">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="c0b94-177">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="c0b94-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="c0b94-178">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="c0b94-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="c0b94-179">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="c0b94-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="c0b94-181">Guid</span><span class="sxs-lookup"><span data-stu-id="c0b94-181">Guid</span></span>|<span data-ttu-id="c0b94-182">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="c0b94-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="c0b94-183">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="c0b94-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="c0b94-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b94-185">Boolean</span></span>|<span data-ttu-id="c0b94-186">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="c0b94-187">iconsVisible</span></span>|<span data-ttu-id="c0b94-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b94-188">Boolean</span></span>|<span data-ttu-id="c0b94-189">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="c0b94-190">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="c0b94-191">protectedApps</span></span>|<span data-ttu-id="c0b94-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="c0b94-193">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="c0b94-194">exemptApps</span></span>|<span data-ttu-id="c0b94-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="c0b94-196">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="c0b94-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="c0b94-197">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="c0b94-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="c0b94-198">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="c0b94-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="c0b94-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c0b94-201">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="c0b94-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="c0b94-202">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="c0b94-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="c0b94-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="c0b94-205">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0b94-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="c0b94-206">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="c0b94-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="c0b94-207">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="c0b94-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="c0b94-208">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="c0b94-209">enterpriseIPRanges</span></span>|<span data-ttu-id="c0b94-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="c0b94-211">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="c0b94-212">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="c0b94-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="c0b94-213">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="c0b94-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="c0b94-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b94-215">Boolean</span></span>|<span data-ttu-id="c0b94-216">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="c0b94-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="c0b94-217">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="c0b94-218">enterpriseProxyServers</span></span>|<span data-ttu-id="c0b94-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c0b94-220">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="c0b94-220">This is a list of proxy servers.</span></span> <span data-ttu-id="c0b94-221">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="c0b94-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="c0b94-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c0b94-224">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="c0b94-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="c0b94-225">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="c0b94-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="c0b94-226">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="c0b94-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="c0b94-227">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="c0b94-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="c0b94-228">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="c0b94-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="c0b94-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b94-230">Boolean</span></span>|<span data-ttu-id="c0b94-231">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="c0b94-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="c0b94-232">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="c0b94-233">neutralDomainResources</span></span>|<span data-ttu-id="c0b94-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c0b94-235">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="c0b94-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="c0b94-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b94-237">Boolean</span></span>|<span data-ttu-id="c0b94-238">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="c0b94-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="c0b94-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b94-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c0b94-241">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c0b94-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c0b94-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c0b94-242">isAssigned</span></span>|<span data-ttu-id="c0b94-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b94-243">Boolean</span></span>|<span data-ttu-id="c0b94-244">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="c0b94-245">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0b94-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c0b94-246">応答</span><span class="sxs-lookup"><span data-stu-id="c0b94-246">Response</span></span>
<span data-ttu-id="c0b94-247">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c0b94-247">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0b94-248">例</span><span class="sxs-lookup"><span data-stu-id="c0b94-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0b94-249">要求</span><span class="sxs-lookup"><span data-stu-id="c0b94-249">Request</span></span>
<span data-ttu-id="c0b94-250">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0b94-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3969

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="c0b94-251">応答</span><span class="sxs-lookup"><span data-stu-id="c0b94-251">Response</span></span>
<span data-ttu-id="c0b94-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0b94-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





