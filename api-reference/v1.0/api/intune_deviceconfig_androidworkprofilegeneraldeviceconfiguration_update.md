# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="0cba1-101">AndroidWorkProfileGeneralDeviceConfiguration を更新する</span><span class="sxs-lookup"><span data-stu-id="0cba1-101">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="0cba1-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0cba1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cba1-103">[AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-103">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0cba1-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0cba1-104">Prerequisites</span></span>
<span data-ttu-id="0cba1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0cba1-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cba1-107">Permission type</span></span>|<span data-ttu-id="0cba1-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cba1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cba1-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cba1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0cba1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cba1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cba1-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cba1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cba1-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cba1-112">Not supported.</span></span>|
|<span data-ttu-id="0cba1-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cba1-113">Application</span></span>|<span data-ttu-id="0cba1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cba1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cba1-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cba1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0cba1-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cba1-116">Request headers</span></span>
|<span data-ttu-id="0cba1-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cba1-117">Header</span></span>|<span data-ttu-id="0cba1-118">値</span><span class="sxs-lookup"><span data-stu-id="0cba1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cba1-119">承認</span><span class="sxs-lookup"><span data-stu-id="0cba1-119">Authorization</span></span>|<span data-ttu-id="0cba1-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0cba1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cba1-121">承諾</span><span class="sxs-lookup"><span data-stu-id="0cba1-121">Accept</span></span>|<span data-ttu-id="0cba1-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="0cba1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cba1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cba1-123">Request body</span></span>
<span data-ttu-id="0cba1-124">要求本文で、[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) オブジェクトに JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="0cba1-125">次の表に、[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-125">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="0cba1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cba1-126">Property</span></span>|<span data-ttu-id="0cba1-127">型</span><span class="sxs-lookup"><span data-stu-id="0cba1-127">Type</span></span>|<span data-ttu-id="0cba1-128">説明</span><span class="sxs-lookup"><span data-stu-id="0cba1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cba1-129">id</span><span class="sxs-lookup"><span data-stu-id="0cba1-129">id</span></span>|<span data-ttu-id="0cba1-130">文字列</span><span class="sxs-lookup"><span data-stu-id="0cba1-130">String</span></span>|<span data-ttu-id="0cba1-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0cba1-131">Key of the entity.</span></span> <span data-ttu-id="0cba1-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0cba1-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cba1-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cba1-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0cba1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cba1-134">DateTimeOffset</span></span>|<span data-ttu-id="0cba1-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0cba1-135">DateTime the object was last modified.</span></span> <span data-ttu-id="0cba1-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0cba1-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cba1-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cba1-137">createdDateTime</span></span>|<span data-ttu-id="0cba1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cba1-138">DateTimeOffset</span></span>|<span data-ttu-id="0cba1-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0cba1-139">DateTime the object was created.</span></span> <span data-ttu-id="0cba1-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0cba1-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cba1-141">description</span><span class="sxs-lookup"><span data-stu-id="0cba1-141">description</span></span>|<span data-ttu-id="0cba1-142">文字列</span><span class="sxs-lookup"><span data-stu-id="0cba1-142">String</span></span>|<span data-ttu-id="0cba1-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0cba1-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0cba1-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0cba1-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cba1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0cba1-145">displayName</span></span>|<span data-ttu-id="0cba1-146">文字列</span><span class="sxs-lookup"><span data-stu-id="0cba1-146">String</span></span>|<span data-ttu-id="0cba1-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0cba1-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0cba1-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0cba1-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cba1-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="0cba1-149">version</span></span>|<span data-ttu-id="0cba1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-150">Int32</span></span>|<span data-ttu-id="0cba1-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0cba1-151">Version of the device configuration.</span></span> <span data-ttu-id="0cba1-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0cba1-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cba1-153">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="0cba1-153">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="0cba1-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="0cba1-154">Boolean</span></span>|<span data-ttu-id="0cba1-155">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-155">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="0cba1-156">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="0cba1-156">passwordBlockTrustAgents</span></span>|<span data-ttu-id="0cba1-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="0cba1-157">Boolean</span></span>|<span data-ttu-id="0cba1-158">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-158">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="0cba1-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0cba1-159">passwordExpirationDays</span></span>|<span data-ttu-id="0cba1-160">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-160">Int32</span></span>|<span data-ttu-id="0cba1-161">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="0cba1-161">Number of days before the password expires.</span></span> <span data-ttu-id="0cba1-162">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-162">Valid values 1 to 365</span></span>|
|<span data-ttu-id="0cba1-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0cba1-163">passwordMinimumLength</span></span>|<span data-ttu-id="0cba1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-164">Int32</span></span>|<span data-ttu-id="0cba1-165">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="0cba1-165">Minimum length of passwords.</span></span> <span data-ttu-id="0cba1-166">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="0cba1-167">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0cba1-167">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0cba1-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-168">Int32</span></span>|<span data-ttu-id="0cba1-169">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="0cba1-169">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="0cba1-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0cba1-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0cba1-171">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-171">Int32</span></span>|<span data-ttu-id="0cba1-172">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="0cba1-172">Number of previous passwords to block.</span></span> <span data-ttu-id="0cba1-173">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-173">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0cba1-174">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="0cba1-174">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="0cba1-175">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-175">Int32</span></span>|<span data-ttu-id="0cba1-176">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="0cba1-176">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="0cba1-177">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-177">Valid values 4 to 11</span></span>|
|<span data-ttu-id="0cba1-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0cba1-178">passwordRequiredType</span></span>|[<span data-ttu-id="0cba1-179">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0cba1-179">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="0cba1-180">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="0cba1-180">Type of password that is required.</span></span> <span data-ttu-id="0cba1-181">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-181">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="0cba1-182">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="0cba1-182">workProfileDataSharingType</span></span>|[<span data-ttu-id="0cba1-183">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="0cba1-183">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="0cba1-184">許可されるデータ共有の種類。</span><span class="sxs-lookup"><span data-stu-id="0cba1-184">Type of data sharing that is allowed.</span></span> <span data-ttu-id="0cba1-185">可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-185">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="0cba1-186">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="0cba1-186">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="0cba1-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-187">Boolean</span></span>|<span data-ttu-id="0cba1-188">デバイスがロックされているときに通知をブロックするかどうかを表示します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-188">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="0cba1-189">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="0cba1-189">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="0cba1-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-190">Boolean</span></span>|<span data-ttu-id="0cba1-191">ユーザーが作業プロファイル内のアカウントを追加/削除できないようにブロックします。</span><span class="sxs-lookup"><span data-stu-id="0cba1-191">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="0cba1-192">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="0cba1-192">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="0cba1-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-193">Boolean</span></span>|<span data-ttu-id="0cba1-194">Bluetooth デバイスで企業の連絡先にアクセスすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-194">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="0cba1-195">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="0cba1-195">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="0cba1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-196">Boolean</span></span>|<span data-ttu-id="0cba1-197">作業プロファイルで、画面キャプチャをブロックします。</span><span class="sxs-lookup"><span data-stu-id="0cba1-197">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="0cba1-198">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="0cba1-198">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="0cba1-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-199">Boolean</span></span>|<span data-ttu-id="0cba1-200">個人プロファイルに作業プロファイルの呼び出し元 ID が表示されないようにします。</span><span class="sxs-lookup"><span data-stu-id="0cba1-200">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="0cba1-201">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="0cba1-201">workProfileBlockCamera</span></span>|<span data-ttu-id="0cba1-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-202">Boolean</span></span>|<span data-ttu-id="0cba1-203">作業プロファイルのカメラをブロックします。</span><span class="sxs-lookup"><span data-stu-id="0cba1-203">Block work profile camera.</span></span>|
|<span data-ttu-id="0cba1-204">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="0cba1-204">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="0cba1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-205">Boolean</span></span>|<span data-ttu-id="0cba1-206">個人プロファイルでの作業プロファイルの連絡先の利用をブロックします。</span><span class="sxs-lookup"><span data-stu-id="0cba1-206">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="0cba1-207">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="0cba1-207">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="0cba1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-208">Boolean</span></span>|<span data-ttu-id="0cba1-209">クロス プロファイルのコピー/貼り付けが許可されていない設定が有効になっているかどうかを表示するブール値です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-209">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="0cba1-210">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="0cba1-210">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="0cba1-211">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="0cba1-211">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="0cba1-212">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="0cba1-212">Type of password that is required.</span></span> <span data-ttu-id="0cba1-213">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-213">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="0cba1-214">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="0cba1-214">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="0cba1-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-215">Boolean</span></span>|<span data-ttu-id="0cba1-216">作業プロファイルで指紋によるロック解除をブロックするかどうかを表示します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-216">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="0cba1-217">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="0cba1-217">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="0cba1-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-218">Boolean</span></span>|<span data-ttu-id="0cba1-219">作業プロファイルでスマートロックや他の信頼エージェントをブロックするかどうかを表示します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-219">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="0cba1-220">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0cba1-220">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="0cba1-221">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-221">Int32</span></span>|<span data-ttu-id="0cba1-222">作業プロファイルのパスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="0cba1-222">Number of days before the password expires.</span></span> <span data-ttu-id="0cba1-223">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="0cba1-224">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0cba1-224">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="0cba1-225">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-225">Int32</span></span>|<span data-ttu-id="0cba1-226">作業プロファイル パスワードの最小長。</span><span class="sxs-lookup"><span data-stu-id="0cba1-226">Minimum length of work profile password.</span></span> <span data-ttu-id="0cba1-227">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-227">Valid values 4 to 16</span></span>|
|<span data-ttu-id="0cba1-228">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="0cba1-228">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="0cba1-229">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-229">Int32</span></span>|<span data-ttu-id="0cba1-230">作業プロファイルのパスワードに必要な数字の最小数です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-230">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="0cba1-231">有効な値は 1 から 10 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-231">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0cba1-232">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="0cba1-232">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="0cba1-233">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-233">Int32</span></span>|<span data-ttu-id="0cba1-234">作業プロファイルのパスワードに必要なアルファベット以外の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-234">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="0cba1-235">有効な値は 1 から 10 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-235">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0cba1-236">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="0cba1-236">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="0cba1-237">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-237">Int32</span></span>|<span data-ttu-id="0cba1-238">作業プロファイルのパスワードに必要な文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-238">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="0cba1-239">有効な値は 1 から 10 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-239">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0cba1-240">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="0cba1-240">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="0cba1-241">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-241">Int32</span></span>|<span data-ttu-id="0cba1-242">作業プロファイルのパスワードに必要な小文字の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-242">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="0cba1-243">有効な値は 1 から 10 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-243">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0cba1-244">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="0cba1-244">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="0cba1-245">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-245">Int32</span></span>|<span data-ttu-id="0cba1-246">作業プロファイルのパスワードに必要な大文字の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-246">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="0cba1-247">有効な値は 1 から 10 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-247">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0cba1-248">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="0cba1-248">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="0cba1-249">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-249">Int32</span></span>|<span data-ttu-id="0cba1-250">作業プロファイルのパスワードに必要なシンボル数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-250">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="0cba1-251">有効な値は 1 から 10 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-251">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0cba1-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0cba1-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0cba1-253">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-253">Int32</span></span>|<span data-ttu-id="0cba1-254">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="0cba1-254">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="0cba1-255">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0cba1-255">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0cba1-256">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-256">Int32</span></span>|<span data-ttu-id="0cba1-257">ブロックする、以前の作業プロファイルのパスワード数。</span><span class="sxs-lookup"><span data-stu-id="0cba1-257">Number of previous passwords to block.</span></span> <span data-ttu-id="0cba1-258">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-258">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0cba1-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="0cba1-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="0cba1-260">Int32</span><span class="sxs-lookup"><span data-stu-id="0cba1-260">Int32</span></span>|<span data-ttu-id="0cba1-261">作業プロファイルが削除され、すべての企業データが消去される前に許容されるサインイン失敗の回数。</span><span class="sxs-lookup"><span data-stu-id="0cba1-261">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="0cba1-262">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="0cba1-262">Valid values 4 to 11</span></span>|
|<span data-ttu-id="0cba1-263">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0cba1-263">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="0cba1-264">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0cba1-264">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="0cba1-265">必要な作業プロファイル パスワードの種類です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-265">Type of password that is required.</span></span> <span data-ttu-id="0cba1-266">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-266">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="0cba1-267">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="0cba1-267">workProfileRequirePassword</span></span>|<span data-ttu-id="0cba1-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cba1-268">Boolean</span></span>|<span data-ttu-id="0cba1-269">作業プロファイルにパスワードが必要かどうか</span><span class="sxs-lookup"><span data-stu-id="0cba1-269">Password is required or not for work profile</span></span>|
|<span data-ttu-id="0cba1-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="0cba1-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="0cba1-271">ブール値</span><span class="sxs-lookup"><span data-stu-id="0cba1-271">Boolean</span></span>|<span data-ttu-id="0cba1-272">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-272">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="0cba1-273">応答</span><span class="sxs-lookup"><span data-stu-id="0cba1-273">Response</span></span>
<span data-ttu-id="0cba1-274">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0cba1-274">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cba1-275">例</span><span class="sxs-lookup"><span data-stu-id="0cba1-275">Example</span></span>
### <a name="request"></a><span data-ttu-id="0cba1-276">要求</span><span class="sxs-lookup"><span data-stu-id="0cba1-276">Request</span></span>
<span data-ttu-id="0cba1-277">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0cba1-277">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1812

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="0cba1-278">応答</span><span class="sxs-lookup"><span data-stu-id="0cba1-278">Response</span></span>
<span data-ttu-id="0cba1-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0cba1-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








