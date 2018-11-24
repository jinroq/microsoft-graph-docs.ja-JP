# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="d366d-101">AndroidWorkProfileGeneralDeviceConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="d366d-101">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="d366d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d366d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d366d-103">新しい[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d366d-103">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d366d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d366d-104">Prerequisites</span></span>
<span data-ttu-id="d366d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d366d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d366d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d366d-107">Permission type</span></span>|<span data-ttu-id="d366d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d366d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d366d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d366d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d366d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d366d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d366d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d366d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d366d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d366d-112">Not supported.</span></span>|
|<span data-ttu-id="d366d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d366d-113">Application</span></span>|<span data-ttu-id="d366d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d366d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d366d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d366d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d366d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d366d-116">Request headers</span></span>
|<span data-ttu-id="d366d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d366d-117">Header</span></span>|<span data-ttu-id="d366d-118">値</span><span class="sxs-lookup"><span data-stu-id="d366d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d366d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d366d-119">Authorization</span></span>|<span data-ttu-id="d366d-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d366d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d366d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d366d-121">Accept</span></span>|<span data-ttu-id="d366d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d366d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d366d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d366d-123">Request body</span></span>
<span data-ttu-id="d366d-124">要求の本文に androidWorkProfileGeneralDeviceConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d366d-124">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="d366d-125">次の表は、androidWorkProfileGeneralDeviceConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d366d-125">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="d366d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d366d-126">Property</span></span>|<span data-ttu-id="d366d-127">型</span><span class="sxs-lookup"><span data-stu-id="d366d-127">Type</span></span>|<span data-ttu-id="d366d-128">説明</span><span class="sxs-lookup"><span data-stu-id="d366d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d366d-129">id</span><span class="sxs-lookup"><span data-stu-id="d366d-129">id</span></span>|<span data-ttu-id="d366d-130">String</span><span class="sxs-lookup"><span data-stu-id="d366d-130">String</span></span>|<span data-ttu-id="d366d-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d366d-131">Key of the entity.</span></span> <span data-ttu-id="d366d-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d366d-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d366d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d366d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d366d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d366d-134">DateTimeOffset</span></span>|<span data-ttu-id="d366d-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d366d-135">DateTime the object was last modified.</span></span> <span data-ttu-id="d366d-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d366d-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d366d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d366d-137">createdDateTime</span></span>|<span data-ttu-id="d366d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d366d-138">DateTimeOffset</span></span>|<span data-ttu-id="d366d-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d366d-139">DateTime the object was created.</span></span> <span data-ttu-id="d366d-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d366d-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d366d-141">説明</span><span class="sxs-lookup"><span data-stu-id="d366d-141">description</span></span>|<span data-ttu-id="d366d-142">String</span><span class="sxs-lookup"><span data-stu-id="d366d-142">String</span></span>|<span data-ttu-id="d366d-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d366d-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d366d-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d366d-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d366d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d366d-145">displayName</span></span>|<span data-ttu-id="d366d-146">String</span><span class="sxs-lookup"><span data-stu-id="d366d-146">String</span></span>|<span data-ttu-id="d366d-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d366d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d366d-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d366d-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d366d-149">version</span><span class="sxs-lookup"><span data-stu-id="d366d-149">version</span></span>|<span data-ttu-id="d366d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-150">Int32</span></span>|<span data-ttu-id="d366d-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d366d-151">Version of the device configuration.</span></span> <span data-ttu-id="d366d-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d366d-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d366d-153">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d366d-153">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d366d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-154">Boolean</span></span>|<span data-ttu-id="d366d-155">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d366d-155">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d366d-156">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d366d-156">passwordBlockTrustAgents</span></span>|<span data-ttu-id="d366d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-157">Boolean</span></span>|<span data-ttu-id="d366d-158">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d366d-158">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="d366d-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d366d-159">passwordExpirationDays</span></span>|<span data-ttu-id="d366d-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-160">Int32</span></span>|<span data-ttu-id="d366d-161">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="d366d-161">Number of days before the password expires.</span></span> <span data-ttu-id="d366d-162">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="d366d-162">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d366d-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d366d-163">passwordMinimumLength</span></span>|<span data-ttu-id="d366d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-164">Int32</span></span>|<span data-ttu-id="d366d-165">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="d366d-165">Minimum length of passwords.</span></span> <span data-ttu-id="d366d-166">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="d366d-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d366d-167">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d366d-167">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d366d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-168">Int32</span></span>|<span data-ttu-id="d366d-169">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="d366d-169">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d366d-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d366d-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d366d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-171">Int32</span></span>|<span data-ttu-id="d366d-172">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="d366d-172">Number of previous passwords to block.</span></span> <span data-ttu-id="d366d-173">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="d366d-173">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d366d-174">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d366d-174">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d366d-175">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-175">Int32</span></span>|<span data-ttu-id="d366d-176">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="d366d-176">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="d366d-177">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="d366d-177">Valid values 4 to 11</span></span>|
|<span data-ttu-id="d366d-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d366d-178">passwordRequiredType</span></span>|[<span data-ttu-id="d366d-179">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d366d-179">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="d366d-180">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="d366d-180">Type of password that is required.</span></span> <span data-ttu-id="d366d-181">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="d366d-181">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="d366d-182">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="d366d-182">workProfileDataSharingType</span></span>|[<span data-ttu-id="d366d-183">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="d366d-183">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="d366d-184">共有するデータの種類を許可します。</span><span class="sxs-lookup"><span data-stu-id="d366d-184">Type of data sharing that is allowed.</span></span> <span data-ttu-id="d366d-185">可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="d366d-185">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="d366d-186">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="d366d-186">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="d366d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-187">Boolean</span></span>|<span data-ttu-id="d366d-188">デバイスがロックされているときに通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d366d-188">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="d366d-189">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="d366d-189">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="d366d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-190">Boolean</span></span>|<span data-ttu-id="d366d-191">作業プロファイル内のアカウントを追加または削除したり、ユーザーをブロックします。</span><span class="sxs-lookup"><span data-stu-id="d366d-191">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="d366d-192">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="d366d-192">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="d366d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-193">Boolean</span></span>|<span data-ttu-id="d366d-194">企業の連絡先にアクセスするための bluetooth デバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d366d-194">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="d366d-195">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="d366d-195">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="d366d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-196">Boolean</span></span>|<span data-ttu-id="d366d-197">作業プロファイルで、画面の取り込みをブロックします。</span><span class="sxs-lookup"><span data-stu-id="d366d-197">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="d366d-198">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="d366d-198">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="d366d-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-199">Boolean</span></span>|<span data-ttu-id="d366d-200">ブロックでは、作業プロファイル呼び出し元 ID を表示個人プロファイルにします。</span><span class="sxs-lookup"><span data-stu-id="d366d-200">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="d366d-201">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="d366d-201">workProfileBlockCamera</span></span>|<span data-ttu-id="d366d-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-202">Boolean</span></span>|<span data-ttu-id="d366d-203">ブロック プロファイル カメラが動作します。</span><span class="sxs-lookup"><span data-stu-id="d366d-203">Block work profile camera.</span></span>|
|<span data-ttu-id="d366d-204">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="d366d-204">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="d366d-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-205">Boolean</span></span>|<span data-ttu-id="d366d-206">個人プロファイルでは、作業プロファイルの連絡先可用性ブロックです。</span><span class="sxs-lookup"><span data-stu-id="d366d-206">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="d366d-207">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="d366d-207">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="d366d-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-208">Boolean</span></span>|<span data-ttu-id="d366d-209">プロファイルのコピーと貼り付けが有効になっている間の設定を許可しない場合を示すブール値です。</span><span class="sxs-lookup"><span data-stu-id="d366d-209">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="d366d-210">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="d366d-210">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="d366d-211">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="d366d-211">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="d366d-212">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="d366d-212">Type of password that is required.</span></span> <span data-ttu-id="d366d-213">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="d366d-213">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="d366d-214">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d366d-214">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d366d-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-215">Boolean</span></span>|<span data-ttu-id="d366d-216">指紋をブロックするかどうかを示す作業プロファイルのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="d366d-216">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="d366d-217">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d366d-217">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="d366d-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-218">Boolean</span></span>|<span data-ttu-id="d366d-219">スマート ロックと作業プロファイルを他の信頼のエージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d366d-219">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="d366d-220">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d366d-220">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="d366d-221">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-221">Int32</span></span>|<span data-ttu-id="d366d-222">日前作業プロファイルのパスワードに、の有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="d366d-222">Number of days before the work profile password expires.</span></span> <span data-ttu-id="d366d-223">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="d366d-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d366d-224">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d366d-224">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="d366d-225">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-225">Int32</span></span>|<span data-ttu-id="d366d-226">作業プロファイル パスワードの最小長。</span><span class="sxs-lookup"><span data-stu-id="d366d-226">Minimum length of work profile password.</span></span> <span data-ttu-id="d366d-227">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="d366d-227">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d366d-228">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="d366d-228">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="d366d-229">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-229">Int32</span></span>|<span data-ttu-id="d366d-230">プロファイル パスワードの作業に必要な数字の最小数です。</span><span class="sxs-lookup"><span data-stu-id="d366d-230">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="d366d-231">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="d366d-231">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d366d-232">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="d366d-232">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="d366d-233">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-233">Int32</span></span>|<span data-ttu-id="d366d-234">プロファイル パスワードの作業に必要なアルファベット以外の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="d366d-234">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="d366d-235">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="d366d-235">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d366d-236">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="d366d-236">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="d366d-237">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-237">Int32</span></span>|<span data-ttu-id="d366d-238">プロファイル パスワードの作業で必要な文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="d366d-238">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="d366d-239">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="d366d-239">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d366d-240">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="d366d-240">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="d366d-241">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-241">Int32</span></span>|<span data-ttu-id="d366d-242">作業プロファイルのパスワードに必要な小文字の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="d366d-242">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="d366d-243">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="d366d-243">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d366d-244">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="d366d-244">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="d366d-245">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-245">Int32</span></span>|<span data-ttu-id="d366d-246">プロファイル パスワードの作業に必要な大文字の文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="d366d-246">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="d366d-247">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="d366d-247">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d366d-248">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="d366d-248">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="d366d-249">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-249">Int32</span></span>|<span data-ttu-id="d366d-250">プロファイル パスワードの作業で必要なシンボル数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="d366d-250">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="d366d-251">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="d366d-251">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d366d-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d366d-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d366d-253">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-253">Int32</span></span>|<span data-ttu-id="d366d-254">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="d366d-254">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d366d-255">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d366d-255">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d366d-256">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-256">Int32</span></span>|<span data-ttu-id="d366d-257">ブロックする前の作業プロファイル パスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="d366d-257">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="d366d-258">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="d366d-258">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d366d-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d366d-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d366d-260">Int32</span><span class="sxs-lookup"><span data-stu-id="d366d-260">Int32</span></span>|<span data-ttu-id="d366d-261">作業プロファイルが削除されるまでに許容される障害および削除されたすべての企業データの記号の数です。</span><span class="sxs-lookup"><span data-stu-id="d366d-261">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="d366d-262">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="d366d-262">Valid values 4 to 11</span></span>|
|<span data-ttu-id="d366d-263">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d366d-263">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="d366d-264">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d366d-264">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="d366d-265">必要な作業プロファイル パスワードの種類です。</span><span class="sxs-lookup"><span data-stu-id="d366d-265">Type of work profile password that is required.</span></span> <span data-ttu-id="d366d-266">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="d366d-266">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="d366d-267">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d366d-267">workProfileRequirePassword</span></span>|<span data-ttu-id="d366d-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-268">Boolean</span></span>|<span data-ttu-id="d366d-269">パスワードが必要な作業プロファイルを</span><span class="sxs-lookup"><span data-stu-id="d366d-269">Password is required or not for work profile</span></span>|
|<span data-ttu-id="d366d-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="d366d-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="d366d-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="d366d-271">Boolean</span></span>|<span data-ttu-id="d366d-272">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="d366d-272">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="d366d-273">応答</span><span class="sxs-lookup"><span data-stu-id="d366d-273">Response</span></span>
<span data-ttu-id="d366d-274">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d366d-274">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d366d-275">例</span><span class="sxs-lookup"><span data-stu-id="d366d-275">Example</span></span>
### <a name="request"></a><span data-ttu-id="d366d-276">要求</span><span class="sxs-lookup"><span data-stu-id="d366d-276">Request</span></span>
<span data-ttu-id="d366d-277">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d366d-277">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="d366d-278">応答</span><span class="sxs-lookup"><span data-stu-id="d366d-278">Response</span></span>
<span data-ttu-id="d366d-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d366d-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



