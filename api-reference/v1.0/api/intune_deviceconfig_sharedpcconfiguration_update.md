# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="1c89d-101">sharedPCConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="1c89d-101">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="1c89d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c89d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c89d-103">[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-103">Update the properties of a [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c89d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1c89d-104">Prerequisites</span></span>
<span data-ttu-id="1c89d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c89d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c89d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c89d-107">Permission type</span></span>|<span data-ttu-id="1c89d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c89d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c89d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c89d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1c89d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c89d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c89d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c89d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c89d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c89d-112">Not supported.</span></span>|
|<span data-ttu-id="1c89d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c89d-113">Application</span></span>|<span data-ttu-id="1c89d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c89d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c89d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c89d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1c89d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c89d-116">Request headers</span></span>
|<span data-ttu-id="1c89d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c89d-117">Header</span></span>|<span data-ttu-id="1c89d-118">値</span><span class="sxs-lookup"><span data-stu-id="1c89d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c89d-119">承認</span><span class="sxs-lookup"><span data-stu-id="1c89d-119">Authorization</span></span>|<span data-ttu-id="1c89d-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="1c89d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c89d-121">承諾</span><span class="sxs-lookup"><span data-stu-id="1c89d-121">Accept</span></span>|<span data-ttu-id="1c89d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1c89d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c89d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c89d-123">Request body</span></span>
<span data-ttu-id="1c89d-124">要求本文で、[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-124">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="1c89d-125">次の表に、[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-125">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="1c89d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c89d-126">Property</span></span>|<span data-ttu-id="1c89d-127">型</span><span class="sxs-lookup"><span data-stu-id="1c89d-127">Type</span></span>|<span data-ttu-id="1c89d-128">説明</span><span class="sxs-lookup"><span data-stu-id="1c89d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c89d-129">id</span><span class="sxs-lookup"><span data-stu-id="1c89d-129">id</span></span>|<span data-ttu-id="1c89d-130">String</span><span class="sxs-lookup"><span data-stu-id="1c89d-130">String</span></span>|<span data-ttu-id="1c89d-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1c89d-131">Key of the entity.</span></span> <span data-ttu-id="1c89d-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c89d-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c89d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c89d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1c89d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c89d-134">DateTimeOffset</span></span>|<span data-ttu-id="1c89d-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1c89d-135">DateTime the object was last modified.</span></span> <span data-ttu-id="1c89d-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c89d-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c89d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c89d-137">createdDateTime</span></span>|<span data-ttu-id="1c89d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c89d-138">DateTimeOffset</span></span>|<span data-ttu-id="1c89d-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1c89d-139">DateTime the object was created.</span></span> <span data-ttu-id="1c89d-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c89d-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c89d-141">description</span><span class="sxs-lookup"><span data-stu-id="1c89d-141">description</span></span>|<span data-ttu-id="1c89d-142">String</span><span class="sxs-lookup"><span data-stu-id="1c89d-142">String</span></span>|<span data-ttu-id="1c89d-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1c89d-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c89d-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c89d-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c89d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1c89d-145">displayName</span></span>|<span data-ttu-id="1c89d-146">String</span><span class="sxs-lookup"><span data-stu-id="1c89d-146">String</span></span>|<span data-ttu-id="1c89d-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1c89d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c89d-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c89d-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c89d-149">version</span><span class="sxs-lookup"><span data-stu-id="1c89d-149">version</span></span>|<span data-ttu-id="1c89d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1c89d-150">Int32</span></span>|<span data-ttu-id="1c89d-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1c89d-151">Version of the device configuration.</span></span> <span data-ttu-id="1c89d-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c89d-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c89d-153">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="1c89d-153">accountManagerPolicy</span></span>|[<span data-ttu-id="1c89d-154">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="1c89d-154">sharedPCAccountManagerPolicy</span></span>](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="1c89d-155">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-155">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="1c89d-156">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="1c89d-156">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="1c89d-157">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="1c89d-157">allowedAccounts</span></span>|[<span data-ttu-id="1c89d-158">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="1c89d-158">sharedPCAllowedAccountType</span></span>](../resources/intune_deviceconfig_sharedpcallowedaccounttype.md)|<span data-ttu-id="1c89d-159">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-159">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="1c89d-160">可能な値は、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="1c89d-160">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="1c89d-161">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="1c89d-161">allowLocalStorage</span></span>|<span data-ttu-id="1c89d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c89d-162">Boolean</span></span>|<span data-ttu-id="1c89d-163">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-163">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="1c89d-164">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="1c89d-164">disableAccountManager</span></span>|<span data-ttu-id="1c89d-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c89d-165">Boolean</span></span>|<span data-ttu-id="1c89d-166">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="1c89d-166">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="1c89d-167">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="1c89d-167">disableEduPolicies</span></span>|<span data-ttu-id="1c89d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c89d-168">Boolean</span></span>|<span data-ttu-id="1c89d-169">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-169">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="1c89d-170">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="1c89d-170">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="1c89d-171">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="1c89d-171">disablePowerPolicies</span></span>|<span data-ttu-id="1c89d-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c89d-172">Boolean</span></span>|<span data-ttu-id="1c89d-173">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-173">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="1c89d-174">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="1c89d-174">disableSignInOnResume</span></span>|<span data-ttu-id="1c89d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c89d-175">Boolean</span></span>|<span data-ttu-id="1c89d-176">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="1c89d-176">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="1c89d-177">enabled</span><span class="sxs-lookup"><span data-stu-id="1c89d-177">enabled</span></span>|<span data-ttu-id="1c89d-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c89d-178">Boolean</span></span>|<span data-ttu-id="1c89d-179">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-179">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="1c89d-180">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="1c89d-180">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="1c89d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="1c89d-181">Int32</span></span>|<span data-ttu-id="1c89d-182">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-182">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="1c89d-183">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="1c89d-183">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="1c89d-184">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="1c89d-184">kioskAppDisplayName</span></span>|<span data-ttu-id="1c89d-185">String</span><span class="sxs-lookup"><span data-stu-id="1c89d-185">String</span></span>|<span data-ttu-id="1c89d-186">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-186">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="1c89d-187">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="1c89d-187">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="1c89d-188">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="1c89d-188">kioskAppUserModelId</span></span>|<span data-ttu-id="1c89d-189">String</span><span class="sxs-lookup"><span data-stu-id="1c89d-189">String</span></span>|<span data-ttu-id="1c89d-190">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-190">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="1c89d-191">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="1c89d-191">maintenanceStartTime</span></span>|<span data-ttu-id="1c89d-192">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1c89d-192">TimeOfDay</span></span>|<span data-ttu-id="1c89d-193">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-193">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="1c89d-194">応答</span><span class="sxs-lookup"><span data-stu-id="1c89d-194">Response</span></span>
<span data-ttu-id="1c89d-195">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="1c89d-195">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c89d-196">例</span><span class="sxs-lookup"><span data-stu-id="1c89d-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c89d-197">要求</span><span class="sxs-lookup"><span data-stu-id="1c89d-197">Request</span></span>
<span data-ttu-id="1c89d-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c89d-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="1c89d-199">応答</span><span class="sxs-lookup"><span data-stu-id="1c89d-199">Response</span></span>
<span data-ttu-id="1c89d-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1c89d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```



