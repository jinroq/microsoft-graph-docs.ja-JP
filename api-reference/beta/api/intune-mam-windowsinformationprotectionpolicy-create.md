---
title: Create windowsInformationProtectionPolicy
description: 新しい windowsInformationProtectionPolicy オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 80615563dcc85b74a7f8d40f9c6752d4c16fdae8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323780"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="89f3a-103">Create windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="89f3a-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="89f3a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="89f3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89f3a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89f3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89f3a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89f3a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89f3a-107">新しい [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89f3a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="89f3a-108">Prerequisites</span></span>
<span data-ttu-id="89f3a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89f3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89f3a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89f3a-111">Permission type</span></span>|<span data-ttu-id="89f3a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="89f3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89f3a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89f3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89f3a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89f3a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89f3a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89f3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89f3a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89f3a-116">Not supported.</span></span>|
|<span data-ttu-id="89f3a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89f3a-117">Application</span></span>|<span data-ttu-id="89f3a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89f3a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89f3a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89f3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="89f3a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89f3a-120">Request headers</span></span>
|<span data-ttu-id="89f3a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89f3a-121">Header</span></span>|<span data-ttu-id="89f3a-122">値</span><span class="sxs-lookup"><span data-stu-id="89f3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89f3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89f3a-123">Authorization</span></span>|<span data-ttu-id="89f3a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="89f3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89f3a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89f3a-125">Accept</span></span>|<span data-ttu-id="89f3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89f3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89f3a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="89f3a-127">Request body</span></span>
<span data-ttu-id="89f3a-128">要求の本文に、windowsInformationProtectionPolicy オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="89f3a-129">次の表に、windowsInformationProtectionPolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="89f3a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89f3a-130">Property</span></span>|<span data-ttu-id="89f3a-131">種類</span><span class="sxs-lookup"><span data-stu-id="89f3a-131">Type</span></span>|<span data-ttu-id="89f3a-132">説明</span><span class="sxs-lookup"><span data-stu-id="89f3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f3a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="89f3a-133">displayName</span></span>|<span data-ttu-id="89f3a-134">String</span><span class="sxs-lookup"><span data-stu-id="89f3a-134">String</span></span>|<span data-ttu-id="89f3a-135">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="89f3a-135">Policy display name.</span></span> <span data-ttu-id="89f3a-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="89f3a-137">説明</span><span class="sxs-lookup"><span data-stu-id="89f3a-137">description</span></span>|<span data-ttu-id="89f3a-138">String</span><span class="sxs-lookup"><span data-stu-id="89f3a-138">String</span></span>|<span data-ttu-id="89f3a-139">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="89f3a-139">The policy's description.</span></span> <span data-ttu-id="89f3a-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="89f3a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89f3a-141">createdDateTime</span></span>|<span data-ttu-id="89f3a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f3a-142">DateTimeOffset</span></span>|<span data-ttu-id="89f3a-143">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="89f3a-143">The date and time the policy was created.</span></span> <span data-ttu-id="89f3a-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="89f3a-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89f3a-145">lastModifiedDateTime</span></span>|<span data-ttu-id="89f3a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f3a-146">DateTimeOffset</span></span>|<span data-ttu-id="89f3a-147">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="89f3a-147">Last time the policy was modified.</span></span> <span data-ttu-id="89f3a-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="89f3a-149">id</span><span class="sxs-lookup"><span data-stu-id="89f3a-149">id</span></span>|<span data-ttu-id="89f3a-150">String</span><span class="sxs-lookup"><span data-stu-id="89f3a-150">String</span></span>|<span data-ttu-id="89f3a-151">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="89f3a-151">Key of the entity.</span></span> <span data-ttu-id="89f3a-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="89f3a-153">version</span><span class="sxs-lookup"><span data-stu-id="89f3a-153">version</span></span>|<span data-ttu-id="89f3a-154">String</span><span class="sxs-lookup"><span data-stu-id="89f3a-154">String</span></span>|<span data-ttu-id="89f3a-155">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="89f3a-155">Version of the entity.</span></span> <span data-ttu-id="89f3a-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="89f3a-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="89f3a-157">enforcementLevel</span></span>|[<span data-ttu-id="89f3a-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="89f3a-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="89f3a-159">WIP の適用レベルです。[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)からサポートされている値継承の列挙型定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89f3a-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="89f3a-160">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="89f3a-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="89f3a-161">enterpriseDomain</span></span>|<span data-ttu-id="89f3a-162">String</span><span class="sxs-lookup"><span data-stu-id="89f3a-162">String</span></span>|<span data-ttu-id="89f3a-163">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="89f3a-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="89f3a-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="89f3a-166">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="89f3a-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="89f3a-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-168">Boolean</span></span>|<span data-ttu-id="89f3a-169">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="89f3a-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="89f3a-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="89f3a-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="89f3a-172">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="89f3a-173">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="89f3a-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="89f3a-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-175">Boolean</span></span>|<span data-ttu-id="89f3a-176">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="89f3a-177">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="89f3a-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="89f3a-178">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="89f3a-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="89f3a-179">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="89f3a-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="89f3a-181">Guid</span><span class="sxs-lookup"><span data-stu-id="89f3a-181">Guid</span></span>|<span data-ttu-id="89f3a-182">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="89f3a-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="89f3a-183">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="89f3a-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="89f3a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-185">Boolean</span></span>|<span data-ttu-id="89f3a-186">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="89f3a-187">iconsVisible</span></span>|<span data-ttu-id="89f3a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-188">Boolean</span></span>|<span data-ttu-id="89f3a-189">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="89f3a-190">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="89f3a-191">protectedApps</span></span>|<span data-ttu-id="89f3a-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="89f3a-193">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="89f3a-194">exemptApps</span></span>|<span data-ttu-id="89f3a-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="89f3a-196">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="89f3a-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="89f3a-197">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="89f3a-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="89f3a-198">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="89f3a-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="89f3a-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="89f3a-201">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="89f3a-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="89f3a-202">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="89f3a-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="89f3a-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="89f3a-205">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="89f3a-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="89f3a-206">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="89f3a-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="89f3a-207">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="89f3a-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="89f3a-208">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="89f3a-209">enterpriseIPRanges</span></span>|<span data-ttu-id="89f3a-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="89f3a-211">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="89f3a-212">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="89f3a-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="89f3a-213">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="89f3a-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="89f3a-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-215">Boolean</span></span>|<span data-ttu-id="89f3a-216">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="89f3a-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="89f3a-217">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="89f3a-218">enterpriseProxyServers</span></span>|<span data-ttu-id="89f3a-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="89f3a-220">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="89f3a-220">This is a list of proxy servers.</span></span> <span data-ttu-id="89f3a-221">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="89f3a-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="89f3a-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="89f3a-224">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="89f3a-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="89f3a-225">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="89f3a-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="89f3a-226">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="89f3a-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="89f3a-227">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="89f3a-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="89f3a-228">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="89f3a-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="89f3a-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-230">Boolean</span></span>|<span data-ttu-id="89f3a-231">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="89f3a-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="89f3a-232">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="89f3a-233">neutralDomainResources</span></span>|<span data-ttu-id="89f3a-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="89f3a-235">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="89f3a-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="89f3a-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-237">Boolean</span></span>|<span data-ttu-id="89f3a-238">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="89f3a-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="89f3a-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89f3a-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="89f3a-241">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="89f3a-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="89f3a-242">isAssigned</span></span>|<span data-ttu-id="89f3a-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-243">Boolean</span></span>|<span data-ttu-id="89f3a-244">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="89f3a-245">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89f3a-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="89f3a-246">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="89f3a-246">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="89f3a-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-247">Boolean</span></span>|<span data-ttu-id="89f3a-248">RS2 の新しいプロパティ、保留中のドキュメント</span><span class="sxs-lookup"><span data-stu-id="89f3a-248">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="89f3a-249">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="89f3a-249">mdmEnrollmentUrl</span></span>|<span data-ttu-id="89f3a-250">String</span><span class="sxs-lookup"><span data-stu-id="89f3a-250">String</span></span>|<span data-ttu-id="89f3a-251">MDM の登録 URL</span><span class="sxs-lookup"><span data-stu-id="89f3a-251">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="89f3a-252">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="89f3a-252">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="89f3a-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f3a-253">Boolean</span></span>|<span data-ttu-id="89f3a-254">Windows にサインインするためのメソッドとして Windows Hello for Business を設定するブール値です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-254">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="89f3a-255">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="89f3a-255">pinMinimumLength</span></span>|<span data-ttu-id="89f3a-256">Int32</span><span class="sxs-lookup"><span data-stu-id="89f3a-256">Int32</span></span>|<span data-ttu-id="89f3a-257">PIN に必要な文字の最小数を設定する整数値です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-257">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="89f3a-258">既定値は 4 です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-258">Default value is 4.</span></span> <span data-ttu-id="89f3a-259">このポリシー設定で構成できる最小値は 4 です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-259">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="89f3a-260">構成できる最大値は、[PIN の最大文字数] ポリシー設定で構成された値、または 127 のうち、どちらか小さい方です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-260">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="89f3a-261">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="89f3a-261">pinUppercaseLetters</span></span>|[<span data-ttu-id="89f3a-262">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="89f3a-262">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="89f3a-263">Windows Hello for Business の PIN における大文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-263">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="89f3a-264">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-264">Default is NotAllow.</span></span> <span data-ttu-id="89f3a-265">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="89f3a-266">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="89f3a-266">pinLowercaseLetters</span></span>|[<span data-ttu-id="89f3a-267">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="89f3a-267">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="89f3a-268">Windows Hello for Business の PIN における小文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-268">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="89f3a-269">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-269">Default is NotAllow.</span></span> <span data-ttu-id="89f3a-270">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-270">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="89f3a-271">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="89f3a-271">pinSpecialCharacters</span></span>|[<span data-ttu-id="89f3a-272">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="89f3a-272">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="89f3a-273">Windows Hello for Business の PIN における特殊文字の使用を構成する整数値です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-273">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="89f3a-274">Windows Hello for Business の PIN ジェスチャの有効な特殊文字は以下のとおりです: !</span><span class="sxs-lookup"><span data-stu-id="89f3a-274">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="89f3a-275">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="89f3a-275">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="89f3a-276">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="89f3a-276">/ : ; < = > ?</span></span><span data-ttu-id="89f3a-277"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="89f3a-277"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="89f3a-278">} ~。</span><span class="sxs-lookup"><span data-stu-id="89f3a-278">} ~.</span></span> <span data-ttu-id="89f3a-279">既定値は NotAllow です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-279">Default is NotAllow.</span></span> <span data-ttu-id="89f3a-280">可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-280">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="89f3a-281">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="89f3a-281">pinExpirationDays</span></span>|<span data-ttu-id="89f3a-282">Int32</span><span class="sxs-lookup"><span data-stu-id="89f3a-282">Int32</span></span>|<span data-ttu-id="89f3a-283">この整数値は、システムがユーザーに PIN の変更を要求する前の、PIN の使用可能な期間 (日数) を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-283">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="89f3a-284">このポリシー設定で構成できる最大値は 730 です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-284">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="89f3a-285">このポリシー設定で構成できる最小値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-285">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="89f3a-286">このポリシーが 0 に設定されている場合、ユーザーの PIN は期限切れになりません。</span><span class="sxs-lookup"><span data-stu-id="89f3a-286">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="89f3a-287">このノードは、Windows 10 バージョン 1511 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="89f3a-287">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="89f3a-288">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-288">Default is 0.</span></span>|
|<span data-ttu-id="89f3a-289">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="89f3a-289">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="89f3a-290">Int32</span><span class="sxs-lookup"><span data-stu-id="89f3a-290">Int32</span></span>|<span data-ttu-id="89f3a-291">再使用できないユーザー アカウントに関連付けられる過去の PIN の数を指定する整数値です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-291">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="89f3a-292">このポリシー設定で構成できる最大値は 50 です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-292">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="89f3a-293">このポリシー設定で構成できる最小値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-293">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="89f3a-294">このポリシーが 0 に設定されている場合、以前の PIN の格納は不要です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-294">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="89f3a-295">このノードは、Windows 10 バージョン 1511 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="89f3a-295">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="89f3a-296">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-296">Default is 0.</span></span>|
|<span data-ttu-id="89f3a-297">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="89f3a-297">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="89f3a-298">Int32</span><span class="sxs-lookup"><span data-stu-id="89f3a-298">Int32</span></span>|<span data-ttu-id="89f3a-299">デバイスがワイプされるまでの、許可されている認証失敗の回数です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-299">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="89f3a-300">値を 0 にすると、デバイス ワイプ機能が無効になります。</span><span class="sxs-lookup"><span data-stu-id="89f3a-300">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="89f3a-301">範囲は整数 X (デスクトップの場合: 4 <= X <= 16、モバイル デバイスの場合: 0 <= X <= 999) です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-301">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="89f3a-302">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="89f3a-302">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="89f3a-303">Int32</span><span class="sxs-lookup"><span data-stu-id="89f3a-303">Int32</span></span>|<span data-ttu-id="89f3a-304">デバイスがアイドルになった後に、デバイスの PIN またはパスワードがロックされるまでの最大時間 (分) を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-304">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="89f3a-305">範囲は整数 X (0 < = X < = 999) です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-305">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="89f3a-306">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="89f3a-306">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="89f3a-307">Int32</span><span class="sxs-lookup"><span data-stu-id="89f3a-307">Int32</span></span>|<span data-ttu-id="89f3a-308">アプリのデータがワイプされるまでのオフライン期間 (日数)</span><span class="sxs-lookup"><span data-stu-id="89f3a-308">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="89f3a-309">応答</span><span class="sxs-lookup"><span data-stu-id="89f3a-309">Response</span></span>
<span data-ttu-id="89f3a-310">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89f3a-310">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89f3a-311">例</span><span class="sxs-lookup"><span data-stu-id="89f3a-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="89f3a-312">要求</span><span class="sxs-lookup"><span data-stu-id="89f3a-312">Request</span></span>
<span data-ttu-id="89f3a-313">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89f3a-313">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4469

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
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

### <a name="response"></a><span data-ttu-id="89f3a-314">応答</span><span class="sxs-lookup"><span data-stu-id="89f3a-314">Response</span></span>
<span data-ttu-id="89f3a-p132">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89f3a-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





