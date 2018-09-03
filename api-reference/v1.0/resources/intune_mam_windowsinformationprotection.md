# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="2ca4b-101">windowsInformationProtection リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="2ca4b-101">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="2ca4b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ca4b-103">詳細な管理設定を構成するための Windows 情報保護のポリシー</span><span class="sxs-lookup"><span data-stu-id="2ca4b-103">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="2ca4b-104">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2ca4b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ca4b-105">Methods</span></span>
|<span data-ttu-id="2ca4b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ca4b-106">Method</span></span>|<span data-ttu-id="2ca4b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2ca4b-107">Return Type</span></span>|<span data-ttu-id="2ca4b-108">説明</span><span class="sxs-lookup"><span data-stu-id="2ca4b-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ca4b-109">List windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="2ca4b-109">List windowsInformationProtections</span></span>](../api/intune_mam_windowsinformationprotection_list.md)|<span data-ttu-id="2ca4b-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="2ca4b-111">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-111">List properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="2ca4b-112">Get windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="2ca4b-112">Get windowsInformationProtection</span></span>](../api/intune_mam_windowsinformationprotection_get.md)|[<span data-ttu-id="2ca4b-113">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="2ca4b-113">windowsInformationProtection</span></span>](../resources/intune_mam_windowsinformationprotection.md)|<span data-ttu-id="2ca4b-114">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-114">Read properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="2ca4b-115">割り当ての操作</span><span class="sxs-lookup"><span data-stu-id="2ca4b-115">assign action</span></span>](../api/intune_mam_windowsinformationprotection_assign.md)|<span data-ttu-id="2ca4b-116">なし</span><span class="sxs-lookup"><span data-stu-id="2ca4b-116">None</span></span>|<span data-ttu-id="2ca4b-117">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2ca4b-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2ca4b-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ca4b-118">Properties</span></span>
|<span data-ttu-id="2ca4b-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ca4b-119">Property</span></span>|<span data-ttu-id="2ca4b-120">タイプ</span><span class="sxs-lookup"><span data-stu-id="2ca4b-120">Type</span></span>|<span data-ttu-id="2ca4b-121">説明</span><span class="sxs-lookup"><span data-stu-id="2ca4b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ca4b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="2ca4b-122">displayName</span></span>|<span data-ttu-id="2ca4b-123">String</span><span class="sxs-lookup"><span data-stu-id="2ca4b-123">String</span></span>|<span data-ttu-id="2ca4b-124">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-124">Policy display name.</span></span> <span data-ttu-id="2ca4b-125">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-125">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ca4b-126">説明</span><span class="sxs-lookup"><span data-stu-id="2ca4b-126">description</span></span>|<span data-ttu-id="2ca4b-127">String</span><span class="sxs-lookup"><span data-stu-id="2ca4b-127">String</span></span>|<span data-ttu-id="2ca4b-128">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-128">The policy's description.</span></span> <span data-ttu-id="2ca4b-129">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-129">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ca4b-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca4b-130">createdDateTime</span></span>|<span data-ttu-id="2ca4b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ca4b-131">DateTimeOffset</span></span>|<span data-ttu-id="2ca4b-132">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-132">The date and time the policy was created.</span></span> <span data-ttu-id="2ca4b-133">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-133">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ca4b-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca4b-134">lastModifiedDateTime</span></span>|<span data-ttu-id="2ca4b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ca4b-135">DateTimeOffset</span></span>|<span data-ttu-id="2ca4b-136">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-136">Last time the policy was modified.</span></span> <span data-ttu-id="2ca4b-137">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-137">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ca4b-138">id</span><span class="sxs-lookup"><span data-stu-id="2ca4b-138">id</span></span>|<span data-ttu-id="2ca4b-139">文字列</span><span class="sxs-lookup"><span data-stu-id="2ca4b-139">String</span></span>|<span data-ttu-id="2ca4b-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-140">Key of the entity.</span></span> <span data-ttu-id="2ca4b-141">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-141">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ca4b-142">version</span><span class="sxs-lookup"><span data-stu-id="2ca4b-142">version</span></span>|<span data-ttu-id="2ca4b-143">String</span><span class="sxs-lookup"><span data-stu-id="2ca4b-143">String</span></span>|<span data-ttu-id="2ca4b-144">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-144">Version of the entity.</span></span> <span data-ttu-id="2ca4b-145">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-145">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ca4b-146">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="2ca4b-146">enforcementLevel</span></span>|[<span data-ttu-id="2ca4b-147">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="2ca4b-147">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="2ca4b-148">WIP の適用レベルです。サポートされている値については、列挙型の定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-148">WIP enforcement level.See the Enum definition for supported values Possible values are: , , , .</span></span> <span data-ttu-id="2ca4b-149">指定できる値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-149">The possible values are `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`, , , , , , , , or .</span></span>|
|<span data-ttu-id="2ca4b-150">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="2ca4b-150">enterpriseDomain</span></span>|<span data-ttu-id="2ca4b-151">String</span><span class="sxs-lookup"><span data-stu-id="2ca4b-151">String</span></span>|<span data-ttu-id="2ca4b-152">プライマリ エンタープライズ ドメイン</span><span class="sxs-lookup"><span data-stu-id="2ca4b-152">Primary enterprise domain</span></span>|
|<span data-ttu-id="2ca4b-153">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="2ca4b-153">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="2ca4b-154">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-154">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2ca4b-155">保護するエンタープライズ ドメインのリスト</span><span class="sxs-lookup"><span data-stu-id="2ca4b-155">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="2ca4b-156">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="2ca4b-156">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="2ca4b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca4b-157">Boolean</span></span>|<span data-ttu-id="2ca4b-158">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-158">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="2ca4b-159">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="2ca4b-159">dataRecoveryCertificate</span></span>|[<span data-ttu-id="2ca4b-160">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="2ca4b-160">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="2ca4b-161">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-161">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="2ca4b-162">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-162">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="2ca4b-163">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="2ca4b-163">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="2ca4b-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca4b-164">Boolean</span></span>|<span data-ttu-id="2ca4b-165">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-165">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="2ca4b-166">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-166">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="2ca4b-167">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-167">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="2ca4b-168">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="2ca4b-168">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="2ca4b-169">Guid</span><span class="sxs-lookup"><span data-stu-id="2ca4b-169">Guid</span></span>|<span data-ttu-id="2ca4b-170">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-170">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="2ca4b-171">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーとアクセスできる期間について、詳細を構成することができます</span><span class="sxs-lookup"><span data-stu-id="2ca4b-171">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="2ca4b-172">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="2ca4b-172">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="2ca4b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca4b-173">Boolean</span></span>|<span data-ttu-id="2ca4b-174">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-174">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="2ca4b-175">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="2ca4b-175">iconsVisible</span></span>|<span data-ttu-id="2ca4b-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca4b-176">Boolean</span></span>|<span data-ttu-id="2ca4b-177">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-177">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="2ca4b-178">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-178">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="2ca4b-179">protectedApps</span><span class="sxs-lookup"><span data-stu-id="2ca4b-179">protectedApps</span></span>|<span data-ttu-id="2ca4b-180">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-180">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="2ca4b-181">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます</span><span class="sxs-lookup"><span data-stu-id="2ca4b-181">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="2ca4b-182">exemptApps</span><span class="sxs-lookup"><span data-stu-id="2ca4b-182">exemptApps</span></span>|<span data-ttu-id="2ca4b-183">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-183">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="2ca4b-184">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-184">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="2ca4b-185">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-185">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="2ca4b-186">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="2ca4b-186">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="2ca4b-187">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-187">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2ca4b-188">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-188">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="2ca4b-189">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データとみなされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます</span><span class="sxs-lookup"><span data-stu-id="2ca4b-189">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="2ca4b-190">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="2ca4b-190">enterpriseProxiedDomains</span></span>|<span data-ttu-id="2ca4b-191">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-191">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="2ca4b-192">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-192">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="2ca4b-193">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-193">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="2ca4b-194">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-194">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="2ca4b-195">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります</span><span class="sxs-lookup"><span data-stu-id="2ca4b-195">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="2ca4b-196">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="2ca4b-196">enterpriseIPRanges</span></span>|<span data-ttu-id="2ca4b-197">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-197">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="2ca4b-198">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-198">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="2ca4b-199">これらのコンピューターからのデータはエンタープライズの一部とみなされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-199">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="2ca4b-200">これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます</span><span class="sxs-lookup"><span data-stu-id="2ca4b-200">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="2ca4b-201">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="2ca4b-201">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="2ca4b-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca4b-202">Boolean</span></span>|<span data-ttu-id="2ca4b-203">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-203">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="2ca4b-204">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="2ca4b-204">Default is false</span></span>|
|<span data-ttu-id="2ca4b-205">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="2ca4b-205">enterpriseProxyServers</span></span>|<span data-ttu-id="2ca4b-206">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-206">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2ca4b-207">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-207">This is a list of proxy servers.</span></span> <span data-ttu-id="2ca4b-208">このリストにないサーバーは、非エンタープライズとみなされます</span><span class="sxs-lookup"><span data-stu-id="2ca4b-208">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="2ca4b-209">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="2ca4b-209">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="2ca4b-210">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-210">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2ca4b-211">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-211">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="2ca4b-212">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-212">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="2ca4b-213">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-213">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="2ca4b-214">それらはエンタープライズ ネットワークの場所にあるとみなされます。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-214">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="2ca4b-215">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-215">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="2ca4b-216">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="2ca4b-216">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="2ca4b-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca4b-217">Boolean</span></span>|<span data-ttu-id="2ca4b-218">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-218">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="2ca4b-219">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="2ca4b-219">Default is false</span></span>|
|<span data-ttu-id="2ca4b-220">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="2ca4b-220">neutralDomainResources</span></span>|<span data-ttu-id="2ca4b-221">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-221">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2ca4b-222">職場または個人のリソースに使用できるドメイン名のリスト</span><span class="sxs-lookup"><span data-stu-id="2ca4b-222">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="2ca4b-223">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="2ca4b-223">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="2ca4b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca4b-224">Boolean</span></span>|<span data-ttu-id="2ca4b-225">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-225">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="2ca4b-226">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="2ca4b-226">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="2ca4b-227">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-227">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2ca4b-228">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します</span><span class="sxs-lookup"><span data-stu-id="2ca4b-228">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="2ca4b-229">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2ca4b-229">isAssigned</span></span>|<span data-ttu-id="2ca4b-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca4b-230">Boolean</span></span>|<span data-ttu-id="2ca4b-231">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-231">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ca4b-232">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ca4b-232">Relationships</span></span>
|<span data-ttu-id="2ca4b-233">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ca4b-233">Relationship</span></span>|<span data-ttu-id="2ca4b-234">型</span><span class="sxs-lookup"><span data-stu-id="2ca4b-234">Type</span></span>|<span data-ttu-id="2ca4b-235">説明</span><span class="sxs-lookup"><span data-stu-id="2ca4b-235">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ca4b-236">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="2ca4b-236">protectedAppLockerFiles</span></span>|<span data-ttu-id="2ca4b-237">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-237">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="2ca4b-238">xml ファイルを使用して、保護されたアプリを入力する別の方法</span><span class="sxs-lookup"><span data-stu-id="2ca4b-238">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="2ca4b-239">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="2ca4b-239">exemptAppLockerFiles</span></span>|<span data-ttu-id="2ca4b-240">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-240">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="2ca4b-241">xml ファイルを使用して、適用除外アプリを入力する別の方法</span><span class="sxs-lookup"><span data-stu-id="2ca4b-241">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="2ca4b-242">assignments</span><span class="sxs-lookup"><span data-stu-id="2ca4b-242">assignments</span></span>|<span data-ttu-id="2ca4b-243">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ca4b-243">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="2ca4b-244">ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-244">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ca4b-245">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ca4b-245">JSON Representation</span></span>
<span data-ttu-id="2ca4b-246">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ca4b-246">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppPolicy",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
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
  "rightsManagementServicesTemplateId": "79199ed9-e50b-4257-8de4-70b9c8685061",
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



