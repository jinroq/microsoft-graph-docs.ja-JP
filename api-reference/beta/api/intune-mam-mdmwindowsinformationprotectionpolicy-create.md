---
title: Create mdmWindowsInformationProtectionPolicy
description: 新しい mdmWindowsInformationProtectionPolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9fe1573f05f19e31d6413343254b9701b6b8c32f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143114"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="a6a12-103">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a6a12-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="a6a12-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6a12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6a12-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6a12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6a12-106">新しい [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-106">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6a12-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6a12-107">Prerequisites</span></span>
<span data-ttu-id="a6a12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6a12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6a12-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6a12-110">Permission type</span></span>|<span data-ttu-id="a6a12-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6a12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6a12-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6a12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6a12-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6a12-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6a12-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6a12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6a12-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6a12-115">Not supported.</span></span>|
|<span data-ttu-id="a6a12-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6a12-116">Application</span></span>|<span data-ttu-id="a6a12-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6a12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6a12-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6a12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a6a12-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6a12-119">Request headers</span></span>
|<span data-ttu-id="a6a12-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6a12-120">Header</span></span>|<span data-ttu-id="a6a12-121">値</span><span class="sxs-lookup"><span data-stu-id="a6a12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6a12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6a12-122">Authorization</span></span>|<span data-ttu-id="a6a12-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a6a12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6a12-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a6a12-124">Accept</span></span>|<span data-ttu-id="a6a12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6a12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6a12-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6a12-126">Request body</span></span>
<span data-ttu-id="a6a12-127">要求の本文に、mdmWindowsInformationProtectionPolicy オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-127">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="a6a12-128">次の表に、mdmWindowsInformationProtectionPolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-128">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="a6a12-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6a12-129">Property</span></span>|<span data-ttu-id="a6a12-130">型</span><span class="sxs-lookup"><span data-stu-id="a6a12-130">Type</span></span>|<span data-ttu-id="a6a12-131">説明</span><span class="sxs-lookup"><span data-stu-id="a6a12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6a12-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a6a12-132">displayName</span></span>|<span data-ttu-id="a6a12-133">String</span><span class="sxs-lookup"><span data-stu-id="a6a12-133">String</span></span>|<span data-ttu-id="a6a12-134">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="a6a12-134">Policy display name.</span></span> <span data-ttu-id="a6a12-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6a12-136">説明</span><span class="sxs-lookup"><span data-stu-id="a6a12-136">description</span></span>|<span data-ttu-id="a6a12-137">文字列</span><span class="sxs-lookup"><span data-stu-id="a6a12-137">String</span></span>|<span data-ttu-id="a6a12-138">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="a6a12-138">The policy's description.</span></span> <span data-ttu-id="a6a12-139">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6a12-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a12-140">createdDateTime</span></span>|<span data-ttu-id="a6a12-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a12-141">DateTimeOffset</span></span>|<span data-ttu-id="a6a12-142">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="a6a12-142">The date and time the policy was created.</span></span> <span data-ttu-id="a6a12-143">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6a12-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a12-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a6a12-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a12-145">DateTimeOffset</span></span>|<span data-ttu-id="a6a12-146">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="a6a12-146">Last time the policy was modified.</span></span> <span data-ttu-id="a6a12-147">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6a12-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6a12-148">roleScopeTagIds</span></span>|<span data-ttu-id="a6a12-149">String collection</span><span class="sxs-lookup"><span data-stu-id="a6a12-149">String collection</span></span>|<span data-ttu-id="a6a12-150">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a6a12-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a6a12-151">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6a12-152">id</span><span class="sxs-lookup"><span data-stu-id="a6a12-152">id</span></span>|<span data-ttu-id="a6a12-153">文字列</span><span class="sxs-lookup"><span data-stu-id="a6a12-153">String</span></span>|<span data-ttu-id="a6a12-154">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a6a12-154">Key of the entity.</span></span> <span data-ttu-id="a6a12-155">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6a12-156">version</span><span class="sxs-lookup"><span data-stu-id="a6a12-156">version</span></span>|<span data-ttu-id="a6a12-157">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a6a12-157">String</span></span>|<span data-ttu-id="a6a12-158">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="a6a12-158">Version of the entity.</span></span> <span data-ttu-id="a6a12-159">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6a12-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a6a12-160">enforcementLevel</span></span>|[<span data-ttu-id="a6a12-161">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a6a12-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="a6a12-162">仕掛品の実施レベル。[windowsinformationprotection](../resources/intune-mam-windowsinformationprotection.md)から継承した、サポートされている値の列挙定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6a12-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="a6a12-163">使用可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="a6a12-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="a6a12-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="a6a12-164">enterpriseDomain</span></span>|<span data-ttu-id="a6a12-165">String</span><span class="sxs-lookup"><span data-stu-id="a6a12-165">String</span></span>|<span data-ttu-id="a6a12-166">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="a6a12-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="a6a12-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6a12-169">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="a6a12-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="a6a12-171">ブール値</span><span class="sxs-lookup"><span data-stu-id="a6a12-171">Boolean</span></span>|<span data-ttu-id="a6a12-172">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a6a12-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="a6a12-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a6a12-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="a6a12-175">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="a6a12-176">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="a6a12-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="a6a12-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="a6a12-178">Boolean</span></span>|<span data-ttu-id="a6a12-179">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="a6a12-180">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a6a12-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="a6a12-181">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="a6a12-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="a6a12-182">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="a6a12-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="a6a12-184">Guid</span><span class="sxs-lookup"><span data-stu-id="a6a12-184">Guid</span></span>|<span data-ttu-id="a6a12-185">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="a6a12-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="a6a12-186">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="a6a12-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="a6a12-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6a12-188">Boolean</span></span>|<span data-ttu-id="a6a12-189">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="a6a12-190">iconsVisible</span></span>|<span data-ttu-id="a6a12-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6a12-191">Boolean</span></span>|<span data-ttu-id="a6a12-192">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="a6a12-193">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="a6a12-194">protectedApps</span></span>|<span data-ttu-id="a6a12-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a6a12-196">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="a6a12-197">exemptApps</span></span>|<span data-ttu-id="a6a12-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a6a12-199">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="a6a12-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="a6a12-200">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="a6a12-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="a6a12-201">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="a6a12-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="a6a12-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6a12-204">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="a6a12-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="a6a12-205">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="a6a12-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="a6a12-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="a6a12-208">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6a12-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="a6a12-209">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="a6a12-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="a6a12-210">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="a6a12-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="a6a12-211">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="a6a12-212">enterpriseIPRanges</span></span>|<span data-ttu-id="a6a12-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="a6a12-214">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="a6a12-215">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="a6a12-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="a6a12-216">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a6a12-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="a6a12-218">ブール値</span><span class="sxs-lookup"><span data-stu-id="a6a12-218">Boolean</span></span>|<span data-ttu-id="a6a12-219">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="a6a12-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="a6a12-220">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="a6a12-221">enterpriseProxyServers</span></span>|<span data-ttu-id="a6a12-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6a12-223">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="a6a12-223">This is a list of proxy servers.</span></span> <span data-ttu-id="a6a12-224">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="a6a12-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="a6a12-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6a12-227">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="a6a12-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="a6a12-228">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="a6a12-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="a6a12-229">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="a6a12-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="a6a12-230">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="a6a12-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="a6a12-231">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a6a12-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="a6a12-233">ブール値</span><span class="sxs-lookup"><span data-stu-id="a6a12-233">Boolean</span></span>|<span data-ttu-id="a6a12-234">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="a6a12-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="a6a12-235">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="a6a12-236">neutralDomainResources</span></span>|<span data-ttu-id="a6a12-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6a12-238">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="a6a12-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="a6a12-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6a12-240">Boolean</span></span>|<span data-ttu-id="a6a12-241">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="a6a12-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="a6a12-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6a12-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6a12-244">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a6a12-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a6a12-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a6a12-245">isAssigned</span></span>|<span data-ttu-id="a6a12-246">ブール値</span><span class="sxs-lookup"><span data-stu-id="a6a12-246">Boolean</span></span>|<span data-ttu-id="a6a12-247">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="a6a12-248">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6a12-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a6a12-249">応答</span><span class="sxs-lookup"><span data-stu-id="a6a12-249">Response</span></span>
<span data-ttu-id="a6a12-250">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a6a12-250">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6a12-251">例</span><span class="sxs-lookup"><span data-stu-id="a6a12-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6a12-252">要求</span><span class="sxs-lookup"><span data-stu-id="a6a12-252">Request</span></span>
<span data-ttu-id="a6a12-253">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6a12-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3967

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="a6a12-254">応答</span><span class="sxs-lookup"><span data-stu-id="a6a12-254">Response</span></span>
<span data-ttu-id="a6a12-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6a12-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4139

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




