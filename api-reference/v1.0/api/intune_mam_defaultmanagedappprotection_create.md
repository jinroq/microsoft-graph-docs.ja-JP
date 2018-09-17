# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="29a96-101">defaultManagedAppProtection を作成</span><span class="sxs-lookup"><span data-stu-id="29a96-101">Create defaultManagedAppProtection</span></span>

> <span data-ttu-id="29a96-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29a96-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29a96-103">新しい [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="29a96-103">Create a new [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29a96-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="29a96-104">Prerequisites</span></span>
<span data-ttu-id="29a96-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="29a96-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29a96-107">Permission type</span></span>|<span data-ttu-id="29a96-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="29a96-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29a96-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29a96-109">Delegated (work or school account)</span></span>|<span data-ttu-id="29a96-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29a96-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="29a96-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29a96-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29a96-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29a96-112">Not supported.</span></span>|
|<span data-ttu-id="29a96-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29a96-113">Application</span></span>|<span data-ttu-id="29a96-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29a96-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29a96-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29a96-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="29a96-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29a96-116">Request headers</span></span>
|<span data-ttu-id="29a96-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29a96-117">Header</span></span>|<span data-ttu-id="29a96-118">値</span><span class="sxs-lookup"><span data-stu-id="29a96-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29a96-119">承認</span><span class="sxs-lookup"><span data-stu-id="29a96-119">Authorization</span></span>|<span data-ttu-id="29a96-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="29a96-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29a96-121">承諾</span><span class="sxs-lookup"><span data-stu-id="29a96-121">Accept</span></span>|<span data-ttu-id="29a96-122">アプリケーションまたは JSON</span><span class="sxs-lookup"><span data-stu-id="29a96-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29a96-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="29a96-123">Request body</span></span>
<span data-ttu-id="29a96-124">要求本文において、defaultManagedAppProtection オブジェクト用の JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="29a96-124">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="29a96-125">次の表に、defaultManagedAppProtection 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-125">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="29a96-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29a96-126">Property</span></span>|<span data-ttu-id="29a96-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="29a96-127">Type</span></span>|<span data-ttu-id="29a96-128">説明</span><span class="sxs-lookup"><span data-stu-id="29a96-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a96-129">displayName</span><span class="sxs-lookup"><span data-stu-id="29a96-129">displayName</span></span>|<span data-ttu-id="29a96-130">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-130">String</span></span>|<span data-ttu-id="29a96-131">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="29a96-131">Policy display name.</span></span> <span data-ttu-id="29a96-132">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="29a96-133">説明</span><span class="sxs-lookup"><span data-stu-id="29a96-133">description</span></span>|<span data-ttu-id="29a96-134">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-134">String</span></span>|<span data-ttu-id="29a96-135">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="29a96-135">The policy's description.</span></span> <span data-ttu-id="29a96-136">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="29a96-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29a96-137">createdDateTime</span></span>|<span data-ttu-id="29a96-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29a96-138">DateTimeOffset</span></span>|<span data-ttu-id="29a96-139">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="29a96-139">The date and time the policy was created.</span></span> <span data-ttu-id="29a96-140">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="29a96-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29a96-141">lastModifiedDateTime</span></span>|<span data-ttu-id="29a96-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29a96-142">DateTimeOffset</span></span>|<span data-ttu-id="29a96-143">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="29a96-143">Last time the policy was modified.</span></span> <span data-ttu-id="29a96-144">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="29a96-145">ID</span><span class="sxs-lookup"><span data-stu-id="29a96-145">id</span></span>|<span data-ttu-id="29a96-146">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-146">String</span></span>|<span data-ttu-id="29a96-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="29a96-147">Key of the entity.</span></span> <span data-ttu-id="29a96-148">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="29a96-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="29a96-149">version</span></span>|<span data-ttu-id="29a96-150">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-150">String</span></span>|<span data-ttu-id="29a96-151">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="29a96-151">Version of the entity.</span></span> <span data-ttu-id="29a96-152">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="29a96-153">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="29a96-153">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="29a96-154">期間</span><span class="sxs-lookup"><span data-stu-id="29a96-154">Duration</span></span>|<span data-ttu-id="29a96-155">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="29a96-155">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="29a96-156">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-156">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-157">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="29a96-157">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="29a96-158">期間</span><span class="sxs-lookup"><span data-stu-id="29a96-158">Duration</span></span>|<span data-ttu-id="29a96-159">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="29a96-159">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="29a96-160">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-160">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-161">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="29a96-161">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="29a96-162">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="29a96-162">managedAppDataTransferLevel</span></span>](../resources/intune_mam_managedappdatatransferlevel.md)|<span data-ttu-id="29a96-p110">データの転送が許可されたソース。[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="29a96-p110">Sources from which data is allowed to be transferred. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="29a96-166">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="29a96-166">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="29a96-167">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="29a96-167">managedAppDataTransferLevel</span></span>](../resources/intune_mam_managedappdatatransferlevel.md)|<span data-ttu-id="29a96-p111">データの転送が許可された宛先。[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="29a96-p111">Destinations to which data is allowed to be transferred. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="29a96-171">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="29a96-171">organizationalCredentialsRequired</span></span>|<span data-ttu-id="29a96-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-172">Boolean</span></span>|<span data-ttu-id="29a96-173">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-173">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="29a96-174">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-174">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-175">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="29a96-175">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="29a96-176">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="29a96-176">managedAppClipboardSharingLevel</span></span>](../resources/intune_mam_managedappclipboardsharinglevel.md)|<span data-ttu-id="29a96-p113">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="29a96-p113">The level to which the clipboard may be shared between apps on the managed device. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="29a96-180">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="29a96-180">dataBackupBlocked</span></span>|<span data-ttu-id="29a96-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-181">Boolean</span></span>|<span data-ttu-id="29a96-182">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-182">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="29a96-183">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-183">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-184">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="29a96-184">deviceComplianceRequired</span></span>|<span data-ttu-id="29a96-185">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-185">Boolean</span></span>|<span data-ttu-id="29a96-186">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-186">Indicates whether device compliance is required.</span></span> <span data-ttu-id="29a96-187">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-187">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-188">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="29a96-188">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="29a96-189">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-189">Boolean</span></span>|<span data-ttu-id="29a96-190">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-190">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="29a96-191">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-191">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-192">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="29a96-192">saveAsBlocked</span></span>|<span data-ttu-id="29a96-193">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-193">Boolean</span></span>|<span data-ttu-id="29a96-194">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-194">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="29a96-195">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-195">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-196">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="29a96-196">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="29a96-197">期間</span><span class="sxs-lookup"><span data-stu-id="29a96-197">Duration</span></span>|<span data-ttu-id="29a96-198">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="29a96-198">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="29a96-199">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-199">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-200">pinRequired</span><span class="sxs-lookup"><span data-stu-id="29a96-200">pinRequired</span></span>|<span data-ttu-id="29a96-201">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-201">Boolean</span></span>|<span data-ttu-id="29a96-202">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-202">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="29a96-203">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-203">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-204">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="29a96-204">maximumPinRetries</span></span>|<span data-ttu-id="29a96-205">Int32</span><span class="sxs-lookup"><span data-stu-id="29a96-205">Int32</span></span>|<span data-ttu-id="29a96-206">正しくない pin の再試行の最大回数。この回数を超えると管理対象アプリがブロックまたは消去されます。</span><span class="sxs-lookup"><span data-stu-id="29a96-206">Maximum number of incorrect pin retry attempts before the managed app is wiped.</span></span> <span data-ttu-id="29a96-207">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-207">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-208">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="29a96-208">simplePinBlocked</span></span>|<span data-ttu-id="29a96-209">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-209">Boolean</span></span>|<span data-ttu-id="29a96-210">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-210">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="29a96-211">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-211">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-212">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="29a96-212">minimumPinLength</span></span>|<span data-ttu-id="29a96-213">Int32</span><span class="sxs-lookup"><span data-stu-id="29a96-213">Int32</span></span>|<span data-ttu-id="29a96-214">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="29a96-214">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-215">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="29a96-215">pinCharacterSet</span></span>|[<span data-ttu-id="29a96-216">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="29a96-216">managedAppPinCharacterSet</span></span>](../resources/intune_mam_managedapppincharacterset.md)|<span data-ttu-id="29a96-p122">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="29a96-p122">Character set which may be used for an app-level pin if PinRequired is set to True. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="29a96-220">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="29a96-220">periodBeforePinReset</span></span>|<span data-ttu-id="29a96-221">期間</span><span class="sxs-lookup"><span data-stu-id="29a96-221">Duration</span></span>|<span data-ttu-id="29a96-222">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="29a96-222">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="29a96-223">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-223">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-224">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="29a96-224">allowedDataStorageLocations</span></span>|<span data-ttu-id="29a96-225">[managedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29a96-225">[managedAppDataStorageLocation enum](../resources/intune_mam_managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="29a96-p124">ユーザーが管理対象データを格納できるデータの保存場所。[ManagedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="29a96-p124">Data storage locations where a user may store managed data. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="29a96-229">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="29a96-229">contactSyncBlocked</span></span>|<span data-ttu-id="29a96-230">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-230">Boolean</span></span>|<span data-ttu-id="29a96-231">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-231">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="29a96-232">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-232">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-233">printBlocked</span><span class="sxs-lookup"><span data-stu-id="29a96-233">printBlocked</span></span>|<span data-ttu-id="29a96-234">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-234">Boolean</span></span>|<span data-ttu-id="29a96-235">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-235">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="29a96-236">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-236">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-237">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="29a96-237">fingerprintBlocked</span></span>|<span data-ttu-id="29a96-238">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-238">Boolean</span></span>|<span data-ttu-id="29a96-239">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-239">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="29a96-240">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-240">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-241">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="29a96-241">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="29a96-242">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-242">Boolean</span></span>|<span data-ttu-id="29a96-243">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-243">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="29a96-244">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-244">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-245">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="29a96-245">minimumRequiredOsVersion</span></span>|<span data-ttu-id="29a96-246">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-246">String</span></span>|<span data-ttu-id="29a96-247">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="29a96-247">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="29a96-248">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-248">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-249">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="29a96-249">minimumWarningOsVersion</span></span>|<span data-ttu-id="29a96-250">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-250">String</span></span>|<span data-ttu-id="29a96-251">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="29a96-251">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="29a96-252">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-252">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-253">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="29a96-253">minimumRequiredAppVersion</span></span>|<span data-ttu-id="29a96-254">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-254">String</span></span>|<span data-ttu-id="29a96-255">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="29a96-255">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="29a96-256">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-256">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-257">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="29a96-257">minimumWarningAppVersion</span></span>|<span data-ttu-id="29a96-258">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-258">String</span></span>|<span data-ttu-id="29a96-259">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="29a96-259">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="29a96-260">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29a96-260">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="29a96-261">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="29a96-261">appDataEncryptionType</span></span>|[<span data-ttu-id="29a96-262">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="29a96-262">managedAppDataEncryptionType</span></span>](../resources/intune_mam_managedappdataencryptiontype.md)|<span data-ttu-id="29a96-p133">(IOS のみ) のマネージ アプリケーション内のデータに対して使用する暗号化の種類です。使用可能な値: `useDeviceSettings`、 `afterDeviceRestart`、 `whenDeviceLockedExceptOpenFiles`、 `whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="29a96-p133">Type of encryption which should be used for data in a managed app. (iOS Only). The possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="29a96-266">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="29a96-266">screenCaptureBlocked</span></span>|<span data-ttu-id="29a96-267">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-267">Boolean</span></span>|<span data-ttu-id="29a96-268">画面キャプチャがブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-268">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="29a96-269">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="29a96-269">(Android only)</span></span>|
|<span data-ttu-id="29a96-270">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="29a96-270">encryptAppData</span></span>|<span data-ttu-id="29a96-271">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-271">Boolean</span></span>|<span data-ttu-id="29a96-272">管理対象アプリのデータを暗号化するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-272">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="29a96-273">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="29a96-273">(Android only)</span></span>|
|<span data-ttu-id="29a96-274">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="29a96-274">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="29a96-275">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-275">Boolean</span></span>|<span data-ttu-id="29a96-276">この設定が有効で、デバイス レベルの暗号化が有効な場合、アプリ レベルの暗号化は無効になります</span><span class="sxs-lookup"><span data-stu-id="29a96-276">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span> <span data-ttu-id="29a96-277">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="29a96-277">(Android only)</span></span>|
|<span data-ttu-id="29a96-278">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="29a96-278">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="29a96-279">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-279">String</span></span>|<span data-ttu-id="29a96-280">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="29a96-280">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="29a96-281">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="29a96-281">(iOS Only).</span></span>|
|<span data-ttu-id="29a96-282">customSettings</span><span class="sxs-lookup"><span data-stu-id="29a96-282">customSettings</span></span>|<span data-ttu-id="29a96-283">[keyValuePair](../resources/intune_mam_keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29a96-283">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="29a96-284">このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="29a96-284">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="29a96-285">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="29a96-285">deployedAppCount</span></span>|<span data-ttu-id="29a96-286">Int32</span><span class="sxs-lookup"><span data-stu-id="29a96-286">Int32</span></span>|<span data-ttu-id="29a96-287">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="29a96-287">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="29a96-288">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="29a96-288">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="29a96-289">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-289">String</span></span>|<span data-ttu-id="29a96-290">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="29a96-290">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="29a96-291">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="29a96-291">(Android only)</span></span>|
|<span data-ttu-id="29a96-292">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="29a96-292">minimumWarningPatchVersion</span></span>|<span data-ttu-id="29a96-293">文字列</span><span class="sxs-lookup"><span data-stu-id="29a96-293">String</span></span>|<span data-ttu-id="29a96-294">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="29a96-294">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="29a96-295">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="29a96-295">(Android only)</span></span>|
|<span data-ttu-id="29a96-296">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="29a96-296">faceIdBlocked</span></span>|<span data-ttu-id="29a96-297">ブール値</span><span class="sxs-lookup"><span data-stu-id="29a96-297">Boolean</span></span>|<span data-ttu-id="29a96-298">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29a96-298">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="29a96-299">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="29a96-299">(iOS Only).</span></span>|



## <a name="response"></a><span data-ttu-id="29a96-300">応答</span><span class="sxs-lookup"><span data-stu-id="29a96-300">Response</span></span>
<span data-ttu-id="29a96-301">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="29a96-301">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29a96-302">例</span><span class="sxs-lookup"><span data-stu-id="29a96-302">Example</span></span>
### <a name="request"></a><span data-ttu-id="29a96-303">要求</span><span class="sxs-lookup"><span data-stu-id="29a96-303">Request</span></span>
<span data-ttu-id="29a96-304">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29a96-304">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 2035

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "faceIdBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="29a96-305">応答</span><span class="sxs-lookup"><span data-stu-id="29a96-305">Response</span></span>
<span data-ttu-id="29a96-p141">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29a96-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2143

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "77064c51-4c51-7706-514c-0677514c0677",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "faceIdBlocked": true
}
```








