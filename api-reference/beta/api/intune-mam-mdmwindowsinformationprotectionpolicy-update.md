---
title: Update mdmWindowsInformationProtectionPolicy
description: mdmWindowsInformationProtectionPolicy オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 900a2eaf57b6b6ba33d0f6071aaa9fc875e81762
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400250"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="92b3c-103">Update mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="92b3c-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="92b3c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="92b3c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="92b3c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92b3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92b3c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92b3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92b3c-107">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-107">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92b3c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="92b3c-108">Prerequisites</span></span>
<span data-ttu-id="92b3c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92b3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="92b3c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92b3c-111">Permission type</span></span>|<span data-ttu-id="92b3c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="92b3c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92b3c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92b3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92b3c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92b3c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92b3c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92b3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92b3c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92b3c-116">Not supported.</span></span>|
|<span data-ttu-id="92b3c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92b3c-117">Application</span></span>|<span data-ttu-id="92b3c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92b3c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92b3c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92b3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="92b3c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92b3c-120">Request headers</span></span>
|<span data-ttu-id="92b3c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92b3c-121">Header</span></span>|<span data-ttu-id="92b3c-122">値</span><span class="sxs-lookup"><span data-stu-id="92b3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92b3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="92b3c-123">Authorization</span></span>|<span data-ttu-id="92b3c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="92b3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92b3c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92b3c-125">Accept</span></span>|<span data-ttu-id="92b3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92b3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b3c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="92b3c-127">Request body</span></span>
<span data-ttu-id="92b3c-128">要求の本文に、[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-128">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="92b3c-129">次の表に、[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-129">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="92b3c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92b3c-130">Property</span></span>|<span data-ttu-id="92b3c-131">型</span><span class="sxs-lookup"><span data-stu-id="92b3c-131">Type</span></span>|<span data-ttu-id="92b3c-132">説明</span><span class="sxs-lookup"><span data-stu-id="92b3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92b3c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="92b3c-133">displayName</span></span>|<span data-ttu-id="92b3c-134">String</span><span class="sxs-lookup"><span data-stu-id="92b3c-134">String</span></span>|<span data-ttu-id="92b3c-135">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="92b3c-135">Policy display name.</span></span> <span data-ttu-id="92b3c-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="92b3c-137">説明</span><span class="sxs-lookup"><span data-stu-id="92b3c-137">description</span></span>|<span data-ttu-id="92b3c-138">String</span><span class="sxs-lookup"><span data-stu-id="92b3c-138">String</span></span>|<span data-ttu-id="92b3c-139">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="92b3c-139">The policy's description.</span></span> <span data-ttu-id="92b3c-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="92b3c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92b3c-141">createdDateTime</span></span>|<span data-ttu-id="92b3c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92b3c-142">DateTimeOffset</span></span>|<span data-ttu-id="92b3c-143">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="92b3c-143">The date and time the policy was created.</span></span> <span data-ttu-id="92b3c-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="92b3c-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92b3c-145">lastModifiedDateTime</span></span>|<span data-ttu-id="92b3c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92b3c-146">DateTimeOffset</span></span>|<span data-ttu-id="92b3c-147">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="92b3c-147">Last time the policy was modified.</span></span> <span data-ttu-id="92b3c-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="92b3c-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92b3c-149">roleScopeTagIds</span></span>|<span data-ttu-id="92b3c-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-150">String collection</span></span>|<span data-ttu-id="92b3c-151">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="92b3c-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="92b3c-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="92b3c-153">id</span><span class="sxs-lookup"><span data-stu-id="92b3c-153">id</span></span>|<span data-ttu-id="92b3c-154">String</span><span class="sxs-lookup"><span data-stu-id="92b3c-154">String</span></span>|<span data-ttu-id="92b3c-155">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="92b3c-155">Key of the entity.</span></span> <span data-ttu-id="92b3c-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="92b3c-157">version</span><span class="sxs-lookup"><span data-stu-id="92b3c-157">version</span></span>|<span data-ttu-id="92b3c-158">String</span><span class="sxs-lookup"><span data-stu-id="92b3c-158">String</span></span>|<span data-ttu-id="92b3c-159">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="92b3c-159">Version of the entity.</span></span> <span data-ttu-id="92b3c-160">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="92b3c-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="92b3c-161">enforcementLevel</span></span>|[<span data-ttu-id="92b3c-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="92b3c-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="92b3c-163">WIP の適用レベルです。[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)からサポートされている値継承の列挙型定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92b3c-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="92b3c-164">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="92b3c-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="92b3c-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="92b3c-165">enterpriseDomain</span></span>|<span data-ttu-id="92b3c-166">String</span><span class="sxs-lookup"><span data-stu-id="92b3c-166">String</span></span>|<span data-ttu-id="92b3c-167">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="92b3c-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="92b3c-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="92b3c-170">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="92b3c-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="92b3c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="92b3c-172">Boolean</span></span>|<span data-ttu-id="92b3c-173">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="92b3c-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="92b3c-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="92b3c-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="92b3c-176">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="92b3c-177">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="92b3c-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="92b3c-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="92b3c-179">Boolean</span></span>|<span data-ttu-id="92b3c-180">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="92b3c-181">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="92b3c-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="92b3c-182">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="92b3c-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="92b3c-183">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="92b3c-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="92b3c-185">Guid</span><span class="sxs-lookup"><span data-stu-id="92b3c-185">Guid</span></span>|<span data-ttu-id="92b3c-186">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="92b3c-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="92b3c-187">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="92b3c-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="92b3c-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="92b3c-189">Boolean</span></span>|<span data-ttu-id="92b3c-190">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="92b3c-191">iconsVisible</span></span>|<span data-ttu-id="92b3c-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="92b3c-192">Boolean</span></span>|<span data-ttu-id="92b3c-193">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="92b3c-194">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="92b3c-195">protectedApps</span></span>|<span data-ttu-id="92b3c-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="92b3c-197">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="92b3c-198">exemptApps</span></span>|<span data-ttu-id="92b3c-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="92b3c-200">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="92b3c-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="92b3c-201">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="92b3c-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="92b3c-202">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="92b3c-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="92b3c-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="92b3c-205">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="92b3c-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="92b3c-206">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="92b3c-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="92b3c-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="92b3c-209">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="92b3c-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="92b3c-210">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="92b3c-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="92b3c-211">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="92b3c-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="92b3c-212">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="92b3c-213">enterpriseIPRanges</span></span>|<span data-ttu-id="92b3c-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="92b3c-215">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="92b3c-216">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="92b3c-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="92b3c-217">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="92b3c-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="92b3c-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="92b3c-219">Boolean</span></span>|<span data-ttu-id="92b3c-220">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="92b3c-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="92b3c-221">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="92b3c-222">enterpriseProxyServers</span></span>|<span data-ttu-id="92b3c-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="92b3c-224">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="92b3c-224">This is a list of proxy servers.</span></span> <span data-ttu-id="92b3c-225">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="92b3c-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="92b3c-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="92b3c-228">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="92b3c-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="92b3c-229">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="92b3c-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="92b3c-230">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="92b3c-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="92b3c-231">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="92b3c-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="92b3c-232">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="92b3c-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="92b3c-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="92b3c-234">Boolean</span></span>|<span data-ttu-id="92b3c-235">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="92b3c-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="92b3c-236">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="92b3c-237">neutralDomainResources</span></span>|<span data-ttu-id="92b3c-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="92b3c-239">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="92b3c-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="92b3c-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="92b3c-241">Boolean</span></span>|<span data-ttu-id="92b3c-242">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="92b3c-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="92b3c-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92b3c-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="92b3c-245">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="92b3c-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="92b3c-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="92b3c-246">isAssigned</span></span>|<span data-ttu-id="92b3c-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="92b3c-247">Boolean</span></span>|<span data-ttu-id="92b3c-248">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="92b3c-249">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92b3c-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="92b3c-250">応答</span><span class="sxs-lookup"><span data-stu-id="92b3c-250">Response</span></span>
<span data-ttu-id="92b3c-251">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="92b3c-251">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92b3c-252">例</span><span class="sxs-lookup"><span data-stu-id="92b3c-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="92b3c-253">要求</span><span class="sxs-lookup"><span data-stu-id="92b3c-253">Request</span></span>
<span data-ttu-id="92b3c-254">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92b3c-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
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

### <a name="response"></a><span data-ttu-id="92b3c-255">応答</span><span class="sxs-lookup"><span data-stu-id="92b3c-255">Response</span></span>
<span data-ttu-id="92b3c-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92b3c-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




