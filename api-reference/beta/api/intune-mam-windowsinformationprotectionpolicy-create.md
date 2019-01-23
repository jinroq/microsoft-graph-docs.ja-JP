---
title: Create windowsInformationProtectionPolicy
description: 新しい windowsInformationProtectionPolicy オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74d9e4a8ddd9ae0979a6360eaf229396b2e107bb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416609"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="d271f-103">Create windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d271f-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="d271f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d271f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d271f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d271f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d271f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d271f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d271f-107">新しい [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d271f-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d271f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d271f-108">Prerequisites</span></span>
<span data-ttu-id="d271f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d271f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d271f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d271f-111">Permission type</span></span>|<span data-ttu-id="d271f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d271f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d271f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d271f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d271f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d271f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d271f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d271f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d271f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d271f-116">Not supported.</span></span>|
|<span data-ttu-id="d271f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d271f-117">Application</span></span>|<span data-ttu-id="d271f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d271f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d271f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d271f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="d271f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d271f-120">Request headers</span></span>
|<span data-ttu-id="d271f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d271f-121">Header</span></span>|<span data-ttu-id="d271f-122">値</span><span class="sxs-lookup"><span data-stu-id="d271f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d271f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d271f-123">Authorization</span></span>|<span data-ttu-id="d271f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d271f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d271f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d271f-125">Accept</span></span>|<span data-ttu-id="d271f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d271f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d271f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d271f-127">Request body</span></span>
<span data-ttu-id="d271f-128">要求の本文に、windowsInformationProtectionPolicy オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="d271f-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="d271f-129">次の表に、windowsInformationProtectionPolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d271f-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="d271f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d271f-130">Property</span></span>|<span data-ttu-id="d271f-131">型</span><span class="sxs-lookup"><span data-stu-id="d271f-131">Type</span></span>|<span data-ttu-id="d271f-132">説明</span><span class="sxs-lookup"><span data-stu-id="d271f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d271f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d271f-133">displayName</span></span>|<span data-ttu-id="d271f-134">String</span><span class="sxs-lookup"><span data-stu-id="d271f-134">String</span></span>|<span data-ttu-id="d271f-135">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="d271f-135">Policy display name.</span></span> <span data-ttu-id="d271f-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d271f-137">説明</span><span class="sxs-lookup"><span data-stu-id="d271f-137">description</span></span>|<span data-ttu-id="d271f-138">String</span><span class="sxs-lookup"><span data-stu-id="d271f-138">String</span></span>|<span data-ttu-id="d271f-139">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="d271f-139">The policy's description.</span></span> <span data-ttu-id="d271f-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d271f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d271f-141">createdDateTime</span></span>|<span data-ttu-id="d271f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d271f-142">DateTimeOffset</span></span>|<span data-ttu-id="d271f-143">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d271f-143">The date and time the policy was created.</span></span> <span data-ttu-id="d271f-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d271f-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d271f-145">lastModifiedDateTime</span></span>|<span data-ttu-id="d271f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d271f-146">DateTimeOffset</span></span>|<span data-ttu-id="d271f-147">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="d271f-147">Last time the policy was modified.</span></span> <span data-ttu-id="d271f-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d271f-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d271f-149">roleScopeTagIds</span></span>|<span data-ttu-id="d271f-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-150">String collection</span></span>|<span data-ttu-id="d271f-151">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="d271f-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d271f-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d271f-153">id</span><span class="sxs-lookup"><span data-stu-id="d271f-153">id</span></span>|<span data-ttu-id="d271f-154">String</span><span class="sxs-lookup"><span data-stu-id="d271f-154">String</span></span>|<span data-ttu-id="d271f-155">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d271f-155">Key of the entity.</span></span> <span data-ttu-id="d271f-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d271f-157">version</span><span class="sxs-lookup"><span data-stu-id="d271f-157">version</span></span>|<span data-ttu-id="d271f-158">String</span><span class="sxs-lookup"><span data-stu-id="d271f-158">String</span></span>|<span data-ttu-id="d271f-159">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d271f-159">Version of the entity.</span></span> <span data-ttu-id="d271f-160">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d271f-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d271f-161">enforcementLevel</span></span>|[<span data-ttu-id="d271f-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d271f-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="d271f-163">WIP の適用レベルです。[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)からサポートされている値継承の列挙型定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d271f-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="d271f-164">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="d271f-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="d271f-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="d271f-165">enterpriseDomain</span></span>|<span data-ttu-id="d271f-166">String</span><span class="sxs-lookup"><span data-stu-id="d271f-166">String</span></span>|<span data-ttu-id="d271f-167">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="d271f-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="d271f-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d271f-170">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="d271f-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="d271f-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-172">Boolean</span></span>|<span data-ttu-id="d271f-173">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d271f-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="d271f-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d271f-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="d271f-176">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="d271f-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="d271f-177">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="d271f-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="d271f-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-179">Boolean</span></span>|<span data-ttu-id="d271f-180">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="d271f-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="d271f-181">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d271f-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="d271f-182">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="d271f-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="d271f-183">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="d271f-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="d271f-185">Guid</span><span class="sxs-lookup"><span data-stu-id="d271f-185">Guid</span></span>|<span data-ttu-id="d271f-186">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="d271f-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="d271f-187">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="d271f-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="d271f-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-189">Boolean</span></span>|<span data-ttu-id="d271f-190">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="d271f-191">iconsVisible</span></span>|<span data-ttu-id="d271f-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-192">Boolean</span></span>|<span data-ttu-id="d271f-193">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d271f-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="d271f-194">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="d271f-195">protectedApps</span></span>|<span data-ttu-id="d271f-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d271f-197">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="d271f-198">exemptApps</span></span>|<span data-ttu-id="d271f-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d271f-200">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="d271f-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="d271f-201">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="d271f-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="d271f-202">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="d271f-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="d271f-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d271f-205">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="d271f-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="d271f-206">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="d271f-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="d271f-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="d271f-209">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d271f-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="d271f-210">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="d271f-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="d271f-211">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="d271f-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="d271f-212">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="d271f-213">enterpriseIPRanges</span></span>|<span data-ttu-id="d271f-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="d271f-215">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="d271f-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="d271f-216">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="d271f-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="d271f-217">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d271f-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="d271f-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-219">Boolean</span></span>|<span data-ttu-id="d271f-220">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="d271f-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="d271f-221">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="d271f-222">enterpriseProxyServers</span></span>|<span data-ttu-id="d271f-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d271f-224">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="d271f-224">This is a list of proxy servers.</span></span> <span data-ttu-id="d271f-225">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="d271f-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="d271f-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d271f-228">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="d271f-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="d271f-229">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="d271f-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="d271f-230">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="d271f-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="d271f-231">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="d271f-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="d271f-232">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d271f-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="d271f-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-234">Boolean</span></span>|<span data-ttu-id="d271f-235">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="d271f-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="d271f-236">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="d271f-237">neutralDomainResources</span></span>|<span data-ttu-id="d271f-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d271f-239">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="d271f-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="d271f-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-241">Boolean</span></span>|<span data-ttu-id="d271f-242">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="d271f-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="d271f-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d271f-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d271f-245">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d271f-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d271f-246">isAssigned</span></span>|<span data-ttu-id="d271f-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-247">Boolean</span></span>|<span data-ttu-id="d271f-248">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d271f-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="d271f-249">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d271f-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d271f-250">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="d271f-250">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="d271f-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-251">Boolean</span></span>|<span data-ttu-id="d271f-252">RS2 の新しいプロパティ、保留中のドキュメント</span><span class="sxs-lookup"><span data-stu-id="d271f-252">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="d271f-253">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="d271f-253">mdmEnrollmentUrl</span></span>|<span data-ttu-id="d271f-254">String</span><span class="sxs-lookup"><span data-stu-id="d271f-254">String</span></span>|<span data-ttu-id="d271f-255">MDM の登録 URL</span><span class="sxs-lookup"><span data-stu-id="d271f-255">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="d271f-256">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="d271f-256">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="d271f-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271f-257">Boolean</span></span>|<span data-ttu-id="d271f-258">Windows にサインインするためのメソッドとして Windows Hello for Business を設定するブール値です。</span><span class="sxs-lookup"><span data-stu-id="d271f-258">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="d271f-259">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d271f-259">pinMinimumLength</span></span>|<span data-ttu-id="d271f-260">Int32</span><span class="sxs-lookup"><span data-stu-id="d271f-260">Int32</span></span>|<span data-ttu-id="d271f-261">PIN に必要な文字の最小数を設定する整数値です。</span><span class="sxs-lookup"><span data-stu-id="d271f-261">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="d271f-262">既定値は 4 です。</span><span class="sxs-lookup"><span data-stu-id="d271f-262">Default value is 4.</span></span> <span data-ttu-id="d271f-263">このポリシー設定で構成できる最小値は 4 です。</span><span class="sxs-lookup"><span data-stu-id="d271f-263">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="d271f-264">構成できる最大値は、[PIN の最大文字数] ポリシー設定で構成された値、または 127 のうち、どちらか小さい方です。</span><span class="sxs-lookup"><span data-stu-id="d271f-264">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="d271f-265">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="d271f-265">pinUppercaseLetters</span></span>|[<span data-ttu-id="d271f-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="d271f-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="d271f-267">Windows Hello for Business の PIN における大文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="d271f-267">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d271f-268">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="d271f-268">Default is NotAllow.</span></span> <span data-ttu-id="d271f-269">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="d271f-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d271f-270">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="d271f-270">pinLowercaseLetters</span></span>|[<span data-ttu-id="d271f-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="d271f-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="d271f-272">Windows Hello for Business の PIN における小文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="d271f-272">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d271f-273">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="d271f-273">Default is NotAllow.</span></span> <span data-ttu-id="d271f-274">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="d271f-274">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d271f-275">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="d271f-275">pinSpecialCharacters</span></span>|[<span data-ttu-id="d271f-276">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="d271f-276">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="d271f-277">Windows Hello for Business の PIN における特殊文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="d271f-277">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d271f-278">Windows Hello for Business の PIN ジェスチャの有効な特殊文字は以下のとおりです: !</span><span class="sxs-lookup"><span data-stu-id="d271f-278">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="d271f-279">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="d271f-279">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="d271f-280">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="d271f-280">/ : ; < = > ?</span></span><span data-ttu-id="d271f-281"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="d271f-281"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="d271f-282">} ~。</span><span class="sxs-lookup"><span data-stu-id="d271f-282">} ~.</span></span> <span data-ttu-id="d271f-283">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="d271f-283">Default is NotAllow.</span></span> <span data-ttu-id="d271f-284">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="d271f-284">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d271f-285">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d271f-285">pinExpirationDays</span></span>|<span data-ttu-id="d271f-286">Int32</span><span class="sxs-lookup"><span data-stu-id="d271f-286">Int32</span></span>|<span data-ttu-id="d271f-287">この整数値は、システムがユーザーに PIN の変更を要求する前の、PIN の使用可能な期間 (日数) を指定します。</span><span class="sxs-lookup"><span data-stu-id="d271f-287">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="d271f-288">このポリシー設定で構成できる最大値は 730 です。</span><span class="sxs-lookup"><span data-stu-id="d271f-288">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="d271f-289">このポリシー設定で構成できる最小値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="d271f-289">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="d271f-290">このポリシーが 0 に設定されている場合、ユーザーの PIN は期限切れになりません。</span><span class="sxs-lookup"><span data-stu-id="d271f-290">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="d271f-291">このノードは、Windows 10 バージョン 1511 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="d271f-291">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="d271f-292">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="d271f-292">Default is 0.</span></span>|
|<span data-ttu-id="d271f-293">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="d271f-293">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="d271f-294">Int32</span><span class="sxs-lookup"><span data-stu-id="d271f-294">Int32</span></span>|<span data-ttu-id="d271f-295">再使用できないユーザー アカウントに関連付けられる過去の PIN の数を指定する整数値です。</span><span class="sxs-lookup"><span data-stu-id="d271f-295">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="d271f-296">このポリシー設定で構成できる最大値は 50 です。</span><span class="sxs-lookup"><span data-stu-id="d271f-296">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="d271f-297">このポリシー設定で構成できる最小値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="d271f-297">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="d271f-298">このポリシーが 0 に設定されている場合、以前の PIN の格納は不要です。</span><span class="sxs-lookup"><span data-stu-id="d271f-298">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="d271f-299">このノードは、Windows 10 バージョン 1511 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="d271f-299">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="d271f-300">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="d271f-300">Default is 0.</span></span>|
|<span data-ttu-id="d271f-301">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="d271f-301">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="d271f-302">Int32</span><span class="sxs-lookup"><span data-stu-id="d271f-302">Int32</span></span>|<span data-ttu-id="d271f-303">デバイスがワイプされるまでの、許可されている認証失敗の回数です。</span><span class="sxs-lookup"><span data-stu-id="d271f-303">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="d271f-304">値を 0 にすると、デバイス ワイプ機能が無効になります。</span><span class="sxs-lookup"><span data-stu-id="d271f-304">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="d271f-305">範囲は整数 X (デスクトップの場合: 4 <= X <= 16、モバイル デバイスの場合: 0 <= X <= 999) です。</span><span class="sxs-lookup"><span data-stu-id="d271f-305">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="d271f-306">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="d271f-306">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="d271f-307">Int32</span><span class="sxs-lookup"><span data-stu-id="d271f-307">Int32</span></span>|<span data-ttu-id="d271f-308">デバイスがアイドルになった後に、デバイスの PIN またはパスワードがロックされるまでの最大時間 (分) を指定します。</span><span class="sxs-lookup"><span data-stu-id="d271f-308">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="d271f-309">範囲は整数 X (0 < = X < = 999) です。</span><span class="sxs-lookup"><span data-stu-id="d271f-309">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="d271f-310">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="d271f-310">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="d271f-311">Int32</span><span class="sxs-lookup"><span data-stu-id="d271f-311">Int32</span></span>|<span data-ttu-id="d271f-312">アプリのデータがワイプされるまでのオフライン期間 (日数)</span><span class="sxs-lookup"><span data-stu-id="d271f-312">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="d271f-313">応答</span><span class="sxs-lookup"><span data-stu-id="d271f-313">Response</span></span>
<span data-ttu-id="d271f-314">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d271f-314">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d271f-315">例</span><span class="sxs-lookup"><span data-stu-id="d271f-315">Example</span></span>

### <a name="request"></a><span data-ttu-id="d271f-316">要求</span><span class="sxs-lookup"><span data-stu-id="d271f-316">Request</span></span>
<span data-ttu-id="d271f-317">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d271f-317">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
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

### <a name="response"></a><span data-ttu-id="d271f-318">応答</span><span class="sxs-lookup"><span data-stu-id="d271f-318">Response</span></span>
<span data-ttu-id="d271f-p133">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d271f-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




