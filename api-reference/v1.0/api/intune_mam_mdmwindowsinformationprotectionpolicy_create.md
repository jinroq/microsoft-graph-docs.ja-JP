# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="bd74d-101">mdmWindowsInformationProtectionPolicy を作成する</span><span class="sxs-lookup"><span data-stu-id="bd74d-101">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="bd74d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd74d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd74d-103">新しい [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-103">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd74d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="bd74d-104">Prerequisites</span></span>
<span data-ttu-id="bd74d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd74d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd74d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd74d-107">Permission type</span></span>|<span data-ttu-id="bd74d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd74d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd74d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd74d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bd74d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd74d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd74d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd74d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd74d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd74d-112">Not supported.</span></span>|
|<span data-ttu-id="bd74d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd74d-113">Application</span></span>|<span data-ttu-id="bd74d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd74d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd74d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd74d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="bd74d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd74d-116">Request headers</span></span>
|<span data-ttu-id="bd74d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd74d-117">Header</span></span>|<span data-ttu-id="bd74d-118">値</span><span class="sxs-lookup"><span data-stu-id="bd74d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd74d-119">承認</span><span class="sxs-lookup"><span data-stu-id="bd74d-119">Authorization</span></span>|<span data-ttu-id="bd74d-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bd74d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd74d-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="bd74d-121">Accept</span></span>|<span data-ttu-id="bd74d-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="bd74d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd74d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd74d-123">Request body</span></span>
<span data-ttu-id="bd74d-124">要求の本文に、mdmWindowsInformationProtectionPolicy オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-124">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="bd74d-125">次の表に、mdmWindowsInformationProtectionPolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-125">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="bd74d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd74d-126">Property</span></span>|<span data-ttu-id="bd74d-127">型</span><span class="sxs-lookup"><span data-stu-id="bd74d-127">Type</span></span>|<span data-ttu-id="bd74d-128">説明</span><span class="sxs-lookup"><span data-stu-id="bd74d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd74d-129">displayName</span><span class="sxs-lookup"><span data-stu-id="bd74d-129">displayName</span></span>|<span data-ttu-id="bd74d-130">文字列</span><span class="sxs-lookup"><span data-stu-id="bd74d-130">String</span></span>|<span data-ttu-id="bd74d-131">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="bd74d-131">Policy display name.</span></span> <span data-ttu-id="bd74d-132">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd74d-133">説明</span><span class="sxs-lookup"><span data-stu-id="bd74d-133">description</span></span>|<span data-ttu-id="bd74d-134">文字列</span><span class="sxs-lookup"><span data-stu-id="bd74d-134">String</span></span>|<span data-ttu-id="bd74d-135">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="bd74d-135">The policy's description.</span></span> <span data-ttu-id="bd74d-136">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd74d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd74d-137">createdDateTime</span></span>|<span data-ttu-id="bd74d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd74d-138">DateTimeOffset</span></span>|<span data-ttu-id="bd74d-139">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="bd74d-139">The date and time the policy was created.</span></span> <span data-ttu-id="bd74d-140">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd74d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd74d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bd74d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd74d-142">DateTimeOffset</span></span>|<span data-ttu-id="bd74d-143">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="bd74d-143">Last time the policy was modified.</span></span> <span data-ttu-id="bd74d-144">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd74d-145">ID</span><span class="sxs-lookup"><span data-stu-id="bd74d-145">id</span></span>|<span data-ttu-id="bd74d-146">文字列</span><span class="sxs-lookup"><span data-stu-id="bd74d-146">String</span></span>|<span data-ttu-id="bd74d-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bd74d-147">Key of the entity.</span></span> <span data-ttu-id="bd74d-148">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd74d-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="bd74d-149">version</span></span>|<span data-ttu-id="bd74d-150">文字列</span><span class="sxs-lookup"><span data-stu-id="bd74d-150">String</span></span>|<span data-ttu-id="bd74d-151">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="bd74d-151">Version of the entity.</span></span> <span data-ttu-id="bd74d-152">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd74d-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="bd74d-153">enforcementLevel</span></span>|[<span data-ttu-id="bd74d-154">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="bd74d-154">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="bd74d-155">WIP の適用レベルです。 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承されるサポートされた値については、列挙型の定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd74d-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: , , , .</span></span> <span data-ttu-id="bd74d-156">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="bd74d-156">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="bd74d-157">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="bd74d-157">enterpriseDomain</span></span>|<span data-ttu-id="bd74d-158">文字列</span><span class="sxs-lookup"><span data-stu-id="bd74d-158">String</span></span>|<span data-ttu-id="bd74d-159">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-159">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-160">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="bd74d-160">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="bd74d-161">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-161">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bd74d-162">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-162">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-163">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="bd74d-163">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="bd74d-164">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd74d-164">Boolean</span></span>|<span data-ttu-id="bd74d-165">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-165">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-166">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="bd74d-166">dataRecoveryCertificate</span></span>|[<span data-ttu-id="bd74d-167">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="bd74d-167">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="bd74d-168">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-168">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="bd74d-169">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-169">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-170">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="bd74d-170">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="bd74d-171">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd74d-171">Boolean</span></span>|<span data-ttu-id="bd74d-172">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-172">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="bd74d-173">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="bd74d-173">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="bd74d-174">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="bd74d-174">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="bd74d-175">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-175">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-176">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="bd74d-176">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="bd74d-177">Guid</span><span class="sxs-lookup"><span data-stu-id="bd74d-177">Guid</span></span>|<span data-ttu-id="bd74d-178">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="bd74d-178">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="bd74d-179">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-179">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-180">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="bd74d-180">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="bd74d-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd74d-181">Boolean</span></span>|<span data-ttu-id="bd74d-182">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-182">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-183">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="bd74d-183">iconsVisible</span></span>|<span data-ttu-id="bd74d-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd74d-184">Boolean</span></span>|<span data-ttu-id="bd74d-185">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-185">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="bd74d-186">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-186">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-187">protectedApps</span><span class="sxs-lookup"><span data-stu-id="bd74d-187">protectedApps</span></span>|<span data-ttu-id="bd74d-188">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-188">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="bd74d-189">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-189">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-190">exemptApps</span><span class="sxs-lookup"><span data-stu-id="bd74d-190">exemptApps</span></span>|<span data-ttu-id="bd74d-191">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-191">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="bd74d-192">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="bd74d-192">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="bd74d-193">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="bd74d-193">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="bd74d-194">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-194">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-195">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="bd74d-195">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="bd74d-196">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-196">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bd74d-197">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="bd74d-197">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="bd74d-198">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-198">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-199">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="bd74d-199">enterpriseProxiedDomains</span></span>|<span data-ttu-id="bd74d-200">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-200">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="bd74d-201">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bd74d-201">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="bd74d-202">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="bd74d-202">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="bd74d-203">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="bd74d-203">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="bd74d-204">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-204">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-205">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="bd74d-205">enterpriseIPRanges</span></span>|<span data-ttu-id="bd74d-206">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-206">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="bd74d-207">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-207">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="bd74d-208">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="bd74d-208">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="bd74d-209">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-209">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-210">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="bd74d-210">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="bd74d-211">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd74d-211">Boolean</span></span>|<span data-ttu-id="bd74d-212">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="bd74d-212">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="bd74d-213">既定値は false です ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-213">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-214">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="bd74d-214">enterpriseProxyServers</span></span>|<span data-ttu-id="bd74d-215">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-215">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bd74d-216">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="bd74d-216">This is a list of proxy servers.</span></span> <span data-ttu-id="bd74d-217">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-217">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-218">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="bd74d-218">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="bd74d-219">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-219">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bd74d-220">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="bd74d-220">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="bd74d-221">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="bd74d-221">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="bd74d-222">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="bd74d-222">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="bd74d-223">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="bd74d-223">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="bd74d-224">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-224">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-225">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="bd74d-225">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="bd74d-226">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd74d-226">Boolean</span></span>|<span data-ttu-id="bd74d-227">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="bd74d-227">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="bd74d-228">既定値は false です ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-228">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-229">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="bd74d-229">neutralDomainResources</span></span>|<span data-ttu-id="bd74d-230">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-230">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bd74d-231">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-231">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-232">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="bd74d-232">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="bd74d-233">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd74d-233">Boolean</span></span>|<span data-ttu-id="bd74d-234">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-234">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-235">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="bd74d-235">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="bd74d-236">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd74d-236">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bd74d-237">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="bd74d-237">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="bd74d-238">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bd74d-238">isAssigned</span></span>|<span data-ttu-id="bd74d-239">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd74d-239">Boolean</span></span>|<span data-ttu-id="bd74d-240">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-240">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="bd74d-241">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bd74d-241">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bd74d-242">応答</span><span class="sxs-lookup"><span data-stu-id="bd74d-242">Response</span></span>
<span data-ttu-id="bd74d-243">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bd74d-243">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd74d-244">例</span><span class="sxs-lookup"><span data-stu-id="bd74d-244">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd74d-245">要求</span><span class="sxs-lookup"><span data-stu-id="bd74d-245">Request</span></span>
<span data-ttu-id="bd74d-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bd74d-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3966

{
  "@odata.type": "#microsoft.intune_mam_graph.windowsInformationProtectionPolicy",
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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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

### <a name="response"></a><span data-ttu-id="bd74d-247">応答</span><span class="sxs-lookup"><span data-stu-id="bd74d-247">Response</span></span>
<span data-ttu-id="bd74d-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd74d-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4074

{
  "@odata.type": "#microsoft.intune_mam_graph.windowsInformationProtectionPolicy",
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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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








