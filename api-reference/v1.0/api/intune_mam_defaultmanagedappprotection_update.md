# <a name="update-defaultmanagedappprotection"></a><span data-ttu-id="2267b-101">Update defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="2267b-101">Update defaultManagedAppProtection</span></span>

> <span data-ttu-id="2267b-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2267b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2267b-103">[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2267b-103">Update the properties of a [calendar](../resources/intune_mam_defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2267b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2267b-104">Prerequisites</span></span>
<span data-ttu-id="2267b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2267b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2267b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2267b-107">Permission type</span></span>|<span data-ttu-id="2267b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2267b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2267b-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="2267b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2267b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2267b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2267b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2267b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2267b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2267b-112">Not supported.</span></span>|
|<span data-ttu-id="2267b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2267b-113">Application</span></span>|<span data-ttu-id="2267b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2267b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2267b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2267b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="2267b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2267b-116">Request headers</span></span>
|<span data-ttu-id="2267b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2267b-117">Header</span></span>|<span data-ttu-id="2267b-118">値</span><span class="sxs-lookup"><span data-stu-id="2267b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2267b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2267b-119">Authorization</span></span>|<span data-ttu-id="2267b-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2267b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2267b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2267b-121">Accept</span></span>|<span data-ttu-id="2267b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2267b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2267b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2267b-123">Request body</span></span>
<span data-ttu-id="2267b-124">要求本文において、[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクト用の JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="2267b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_defaultmanagedappprotection.md) object.</span></span>

<span data-ttu-id="2267b-125">次の表に、[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2267b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2267b-126">Property</span></span>|<span data-ttu-id="2267b-127">型</span><span class="sxs-lookup"><span data-stu-id="2267b-127">Type</span></span>|<span data-ttu-id="2267b-128">説明</span><span class="sxs-lookup"><span data-stu-id="2267b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2267b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="2267b-129">displayName</span></span>|<span data-ttu-id="2267b-130">String</span><span class="sxs-lookup"><span data-stu-id="2267b-130">String</span></span>|<span data-ttu-id="2267b-131">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="2267b-131">Policy display name.</span></span> <span data-ttu-id="2267b-132">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2267b-133">description</span><span class="sxs-lookup"><span data-stu-id="2267b-133">description</span></span>|<span data-ttu-id="2267b-134">String</span><span class="sxs-lookup"><span data-stu-id="2267b-134">String</span></span>|<span data-ttu-id="2267b-135">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="2267b-135">The policy's description.</span></span> <span data-ttu-id="2267b-136">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2267b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2267b-137">createdDateTime</span></span>|<span data-ttu-id="2267b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2267b-138">DateTimeOffset</span></span>|<span data-ttu-id="2267b-139">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="2267b-139">The date and time when the page was created.</span></span> <span data-ttu-id="2267b-140">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2267b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2267b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="2267b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2267b-142">DateTimeOffset</span></span>|<span data-ttu-id="2267b-143">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="2267b-143">Last time the policy was modified.</span></span> <span data-ttu-id="2267b-144">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2267b-145">id</span><span class="sxs-lookup"><span data-stu-id="2267b-145">id</span></span>|<span data-ttu-id="2267b-146">String</span><span class="sxs-lookup"><span data-stu-id="2267b-146">String</span></span>|<span data-ttu-id="2267b-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2267b-147">Name of the entity.</span></span> <span data-ttu-id="2267b-148">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2267b-149">version</span><span class="sxs-lookup"><span data-stu-id="2267b-149">version</span></span>|<span data-ttu-id="2267b-150">String</span><span class="sxs-lookup"><span data-stu-id="2267b-150">String</span></span>|<span data-ttu-id="2267b-151">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2267b-151">Version of the entity.</span></span> <span data-ttu-id="2267b-152">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2267b-153">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="2267b-153">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="2267b-154">Duration</span><span class="sxs-lookup"><span data-stu-id="2267b-154">Duration</span></span>|<span data-ttu-id="2267b-155">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="2267b-155">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="2267b-156">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-156">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-157">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="2267b-157">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="2267b-158">Duration</span><span class="sxs-lookup"><span data-stu-id="2267b-158">Duration</span></span>|<span data-ttu-id="2267b-159">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="2267b-159">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="2267b-160">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-160">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-161">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="2267b-161">allowedInboundDataTransferSources</span></span>|<span data-ttu-id="2267b-162">String</span><span class="sxs-lookup"><span data-stu-id="2267b-162">String</span></span>|<span data-ttu-id="2267b-163">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="2267b-163">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="2267b-164">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="2267b-164">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="2267b-165">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="2267b-165">allowedOutboundDataTransferDestinations</span></span>|<span data-ttu-id="2267b-166">String</span><span class="sxs-lookup"><span data-stu-id="2267b-166">String</span></span>|<span data-ttu-id="2267b-167">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="2267b-167">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="2267b-168">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="2267b-168">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="2267b-169">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="2267b-169">organizationalCredentialsRequired</span></span>|<span data-ttu-id="2267b-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-170">Boolean</span></span>|<span data-ttu-id="2267b-171">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-171">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="2267b-172">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-172">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-173">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="2267b-173">allowedOutboundClipboardSharingLevel</span></span>|<span data-ttu-id="2267b-174">String</span><span class="sxs-lookup"><span data-stu-id="2267b-174">String</span></span>|<span data-ttu-id="2267b-175">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="2267b-175">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="2267b-176">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="2267b-176">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="2267b-177">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="2267b-177">dataBackupBlocked</span></span>|<span data-ttu-id="2267b-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-178">Boolean</span></span>|<span data-ttu-id="2267b-179">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-179">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="2267b-180">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-180">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-181">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="2267b-181">deviceComplianceRequired</span></span>|<span data-ttu-id="2267b-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-182">Boolean</span></span>|<span data-ttu-id="2267b-183">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-183">Indicates whether device compliance is required.</span></span> <span data-ttu-id="2267b-184">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-184">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-185">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="2267b-185">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="2267b-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-186">Boolean</span></span>|<span data-ttu-id="2267b-187">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-187">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="2267b-188">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-188">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-189">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="2267b-189">saveAsBlocked</span></span>|<span data-ttu-id="2267b-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-190">Boolean</span></span>|<span data-ttu-id="2267b-191">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-191">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="2267b-192">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-192">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-193">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="2267b-193">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="2267b-194">Duration</span><span class="sxs-lookup"><span data-stu-id="2267b-194">Duration</span></span>|<span data-ttu-id="2267b-195">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="2267b-195">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="2267b-196">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-196">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-197">pinRequired</span><span class="sxs-lookup"><span data-stu-id="2267b-197">pinRequired</span></span>|<span data-ttu-id="2267b-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-198">Boolean</span></span>|<span data-ttu-id="2267b-199">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-199">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="2267b-200">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-200">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-201">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="2267b-201">maximumPinRetries</span></span>|<span data-ttu-id="2267b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2267b-202">Int32</span></span>|<span data-ttu-id="2267b-203">正しくない pin の再試行の最大回数。この回数を超えると管理対象アプリが消去されます。</span><span class="sxs-lookup"><span data-stu-id="2267b-203">Maximum number of incorrect pin retry attempts before the managed app is wiped.</span></span> <span data-ttu-id="2267b-204">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-204">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-205">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="2267b-205">simplePinBlocked</span></span>|<span data-ttu-id="2267b-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-206">Boolean</span></span>|<span data-ttu-id="2267b-207">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-207">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="2267b-208">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-208">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-209">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="2267b-209">minimumPinLength</span></span>|<span data-ttu-id="2267b-210">Int32</span><span class="sxs-lookup"><span data-stu-id="2267b-210">Int32</span></span>|<span data-ttu-id="2267b-211">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2267b-211">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-212">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="2267b-212">pinCharacterSet</span></span>|<span data-ttu-id="2267b-213">String</span><span class="sxs-lookup"><span data-stu-id="2267b-213">String</span></span>|<span data-ttu-id="2267b-214">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="2267b-214">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="2267b-215">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="2267b-215">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="2267b-216">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="2267b-216">periodBeforePinReset</span></span>|<span data-ttu-id="2267b-217">Duration</span><span class="sxs-lookup"><span data-stu-id="2267b-217">Duration</span></span>|<span data-ttu-id="2267b-218">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2267b-218">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="2267b-219">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-219">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-220">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="2267b-220">allowedDataStorageLocations</span></span>|<span data-ttu-id="2267b-221">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2267b-221">String collection</span></span>|<span data-ttu-id="2267b-222">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="2267b-222">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="2267b-223">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。可能な値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="2267b-223">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="2267b-224">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="2267b-224">contactSyncBlocked</span></span>|<span data-ttu-id="2267b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-225">Boolean</span></span>|<span data-ttu-id="2267b-226">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-226">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="2267b-227">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-227">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-228">printBlocked</span><span class="sxs-lookup"><span data-stu-id="2267b-228">printBlocked</span></span>|<span data-ttu-id="2267b-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-229">Boolean</span></span>|<span data-ttu-id="2267b-230">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-230">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="2267b-231">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-231">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-232">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="2267b-232">fingerprintBlocked</span></span>|<span data-ttu-id="2267b-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-233">Boolean</span></span>|<span data-ttu-id="2267b-234">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-234">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="2267b-235">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-235">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-236">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="2267b-236">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="2267b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-237">Boolean</span></span>|<span data-ttu-id="2267b-238">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-238">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="2267b-239">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-239">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-240">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="2267b-240">minimumRequiredOsVersion</span></span>|<span data-ttu-id="2267b-241">String</span><span class="sxs-lookup"><span data-stu-id="2267b-241">String</span></span>|<span data-ttu-id="2267b-242">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2267b-242">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="2267b-243">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-243">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-244">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="2267b-244">minimumWarningOsVersion</span></span>|<span data-ttu-id="2267b-245">String</span><span class="sxs-lookup"><span data-stu-id="2267b-245">String</span></span>|<span data-ttu-id="2267b-246">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2267b-246">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="2267b-247">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-247">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-248">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="2267b-248">minimumRequiredAppVersion</span></span>|<span data-ttu-id="2267b-249">String</span><span class="sxs-lookup"><span data-stu-id="2267b-249">String</span></span>|<span data-ttu-id="2267b-250">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2267b-250">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="2267b-251">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-251">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-252">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="2267b-252">minimumWarningAppVersion</span></span>|<span data-ttu-id="2267b-253">String</span><span class="sxs-lookup"><span data-stu-id="2267b-253">String</span></span>|<span data-ttu-id="2267b-254">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2267b-254">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="2267b-255">[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2267b-255">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="2267b-256">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="2267b-256">appDataEncryptionType</span></span>|<span data-ttu-id="2267b-257">String</span><span class="sxs-lookup"><span data-stu-id="2267b-257">String</span></span>|<span data-ttu-id="2267b-258">管理対象アプリのデータに使用する暗号化の種類。</span><span class="sxs-lookup"><span data-stu-id="2267b-258">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="2267b-259">可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です (iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="2267b-259">(iOS Only) Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="2267b-260">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="2267b-260">screenCaptureBlocked</span></span>|<span data-ttu-id="2267b-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-261">Boolean</span></span>|<span data-ttu-id="2267b-262">画面キャプチャがブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-262">Indicates whether screen capture is blocked.</span></span>|
|<span data-ttu-id="2267b-263">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="2267b-263">encryptAppData</span></span>|<span data-ttu-id="2267b-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-264">Boolean</span></span>|<span data-ttu-id="2267b-265">管理対象アプリのデータを暗号化するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-265">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="2267b-266">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="2267b-266">(Android only)</span></span>|
|<span data-ttu-id="2267b-267">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="2267b-267">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="2267b-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-268">Boolean</span></span>|<span data-ttu-id="2267b-269">この設定が有効で、デバイス レベルの暗号化が有効な場合、アプリ レベルの暗号化は無効になります</span><span class="sxs-lookup"><span data-stu-id="2267b-269">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="2267b-270">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="2267b-270">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="2267b-271">String</span><span class="sxs-lookup"><span data-stu-id="2267b-271">String</span></span>|<span data-ttu-id="2267b-272">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2267b-272">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="2267b-273">customSettings</span><span class="sxs-lookup"><span data-stu-id="2267b-273">customSettings</span></span>|<span data-ttu-id="2267b-274">[keyValuePair](../resources/intune_mam_keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2267b-274">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="2267b-275">このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="2267b-275">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="2267b-276">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="2267b-276">deployedAppCount</span></span>|<span data-ttu-id="2267b-277">Int32</span><span class="sxs-lookup"><span data-stu-id="2267b-277">Int32</span></span>|<span data-ttu-id="2267b-278">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="2267b-278">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="2267b-279">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="2267b-279">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="2267b-280">String</span><span class="sxs-lookup"><span data-stu-id="2267b-280">String</span></span>|<span data-ttu-id="2267b-281">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="2267b-281">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="2267b-282">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="2267b-282">minimumWarningPatchVersion</span></span>|<span data-ttu-id="2267b-283">String</span><span class="sxs-lookup"><span data-stu-id="2267b-283">String</span></span>|<span data-ttu-id="2267b-284">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="2267b-284">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|
|<span data-ttu-id="2267b-285">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="2267b-285">faceIdBlocked</span></span>|<span data-ttu-id="2267b-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="2267b-286">Boolean</span></span>|<span data-ttu-id="2267b-287">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2267b-287">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|



## <a name="response"></a><span data-ttu-id="2267b-288">応答</span><span class="sxs-lookup"><span data-stu-id="2267b-288">Response</span></span>
<span data-ttu-id="2267b-289">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="2267b-289">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2267b-290">例</span><span class="sxs-lookup"><span data-stu-id="2267b-290">Example</span></span>
### <a name="request"></a><span data-ttu-id="2267b-291">要求</span><span class="sxs-lookup"><span data-stu-id="2267b-291">Request</span></span>
<span data-ttu-id="2267b-292">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2267b-292">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
Content-type: application/json
Content-length: 1969

{
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

### <a name="response"></a><span data-ttu-id="2267b-293">応答</span><span class="sxs-lookup"><span data-stu-id="2267b-293">Response</span></span>
<span data-ttu-id="2267b-p135">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2267b-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



