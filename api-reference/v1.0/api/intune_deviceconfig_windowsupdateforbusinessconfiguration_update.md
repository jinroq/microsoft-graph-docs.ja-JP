# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="5c2de-101">windowsUpdateForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="5c2de-101">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="5c2de-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c2de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c2de-103">[windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5c2de-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c2de-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5c2de-104">Prerequisites</span></span>
<span data-ttu-id="5c2de-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c2de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5c2de-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c2de-107">Permission type</span></span>|<span data-ttu-id="5c2de-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c2de-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c2de-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c2de-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5c2de-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c2de-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c2de-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c2de-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c2de-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c2de-112">Not supported.</span></span>|
|<span data-ttu-id="5c2de-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c2de-113">Application</span></span>|<span data-ttu-id="5c2de-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c2de-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c2de-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c2de-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5c2de-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c2de-116">Request headers</span></span>
|<span data-ttu-id="5c2de-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c2de-117">Header</span></span>|<span data-ttu-id="5c2de-118">値</span><span class="sxs-lookup"><span data-stu-id="5c2de-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c2de-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c2de-119">Authorization</span></span>|<span data-ttu-id="5c2de-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c2de-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5c2de-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5c2de-121">Accept</span></span>|<span data-ttu-id="5c2de-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5c2de-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c2de-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c2de-123">Request body</span></span>
<span data-ttu-id="5c2de-124">要求本文では、[windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c2de-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="5c2de-125">次の表に、[windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5c2de-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5c2de-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c2de-126">Property</span></span>|<span data-ttu-id="5c2de-127">型</span><span class="sxs-lookup"><span data-stu-id="5c2de-127">Type</span></span>|<span data-ttu-id="5c2de-128">説明</span><span class="sxs-lookup"><span data-stu-id="5c2de-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c2de-129">id</span><span class="sxs-lookup"><span data-stu-id="5c2de-129">id</span></span>|<span data-ttu-id="5c2de-130">String</span><span class="sxs-lookup"><span data-stu-id="5c2de-130">String</span></span>|<span data-ttu-id="5c2de-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5c2de-131">Name of the entity.</span></span> <span data-ttu-id="5c2de-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c2de-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c2de-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c2de-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5c2de-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c2de-134">DateTimeOffset</span></span>|<span data-ttu-id="5c2de-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="5c2de-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="5c2de-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c2de-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c2de-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c2de-137">createdDateTime</span></span>|<span data-ttu-id="5c2de-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c2de-138">DateTimeOffset</span></span>|<span data-ttu-id="5c2de-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5c2de-139">DateTime the object was created.</span></span> <span data-ttu-id="5c2de-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c2de-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c2de-141">description</span><span class="sxs-lookup"><span data-stu-id="5c2de-141">description</span></span>|<span data-ttu-id="5c2de-142">String</span><span class="sxs-lookup"><span data-stu-id="5c2de-142">String</span></span>|<span data-ttu-id="5c2de-143">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="5c2de-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c2de-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c2de-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c2de-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5c2de-145">displayName</span></span>|<span data-ttu-id="5c2de-146">String</span><span class="sxs-lookup"><span data-stu-id="5c2de-146">String</span></span>|<span data-ttu-id="5c2de-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="5c2de-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c2de-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c2de-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c2de-149">version</span><span class="sxs-lookup"><span data-stu-id="5c2de-149">version</span></span>|<span data-ttu-id="5c2de-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5c2de-150">Int32</span></span>|<span data-ttu-id="5c2de-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5c2de-151">Version of the device configuration.</span></span> <span data-ttu-id="5c2de-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c2de-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c2de-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="5c2de-153">deliveryOptimizationMode</span></span>|<span data-ttu-id="5c2de-154">String</span><span class="sxs-lookup"><span data-stu-id="5c2de-154">String</span></span>|<span data-ttu-id="5c2de-155">配信最適化モード。可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="5c2de-155">Delivery Optimization Mode Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="5c2de-156">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="5c2de-156">prereleaseFeatures</span></span>|<span data-ttu-id="5c2de-157">String</span><span class="sxs-lookup"><span data-stu-id="5c2de-157">String</span></span>|<span data-ttu-id="5c2de-158">プレリリース機能。</span><span class="sxs-lookup"><span data-stu-id="5c2de-158">The pre-release features.</span></span> <span data-ttu-id="5c2de-159">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="5c2de-159">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="5c2de-160">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="5c2de-160">automaticUpdateMode</span></span>|<span data-ttu-id="5c2de-161">String</span><span class="sxs-lookup"><span data-stu-id="5c2de-161">String</span></span>|<span data-ttu-id="5c2de-162">自動更新モード。</span><span class="sxs-lookup"><span data-stu-id="5c2de-162">Automatic update mode.</span></span> <span data-ttu-id="5c2de-163">可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` です。</span><span class="sxs-lookup"><span data-stu-id="5c2de-163">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="5c2de-164">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="5c2de-164">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="5c2de-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c2de-165">Boolean</span></span>|<span data-ttu-id="5c2de-166">Microsoft Update サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="5c2de-166">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="5c2de-167">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="5c2de-167">driversExcluded</span></span>|<span data-ttu-id="5c2de-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c2de-168">Boolean</span></span>|<span data-ttu-id="5c2de-169">Windows Update のドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="5c2de-169">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="5c2de-170">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="5c2de-170">installationSchedule</span></span>|[<span data-ttu-id="5c2de-171">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="5c2de-171">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="5c2de-172">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="5c2de-172">Installation schedule</span></span>|
|<span data-ttu-id="5c2de-173">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="5c2de-173">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="5c2de-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5c2de-174">Int32</span></span>|<span data-ttu-id="5c2de-175">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="5c2de-175">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="5c2de-176">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="5c2de-176">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="5c2de-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5c2de-177">Int32</span></span>|<span data-ttu-id="5c2de-178">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="5c2de-178">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="5c2de-179">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="5c2de-179">qualityUpdatesPaused</span></span>|<span data-ttu-id="5c2de-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c2de-180">Boolean</span></span>|<span data-ttu-id="5c2de-181">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="5c2de-181">Pause Quality Updates</span></span>|
|<span data-ttu-id="5c2de-182">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="5c2de-182">featureUpdatesPaused</span></span>|<span data-ttu-id="5c2de-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c2de-183">Boolean</span></span>|<span data-ttu-id="5c2de-184">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="5c2de-184">Pause Feature Updates</span></span>|
|<span data-ttu-id="5c2de-185">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="5c2de-185">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="5c2de-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c2de-186">DateTimeOffset</span></span>|<span data-ttu-id="5c2de-187">品質更新プログラムの一時停止が終了する日時</span><span class="sxs-lookup"><span data-stu-id="5c2de-187">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="5c2de-188">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="5c2de-188">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="5c2de-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c2de-189">DateTimeOffset</span></span>|<span data-ttu-id="5c2de-190">機能更新プログラムの一時停止が終了する日時</span><span class="sxs-lookup"><span data-stu-id="5c2de-190">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="5c2de-191">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="5c2de-191">businessReadyUpdatesOnly</span></span>|<span data-ttu-id="5c2de-192">String</span><span class="sxs-lookup"><span data-stu-id="5c2de-192">String</span></span>|<span data-ttu-id="5c2de-193">デバイスが、どのブランチから更新プログラムを受け取るかを決定します。可能な値は、`userDefined`、`all`、`businessReadyOnly` です。</span><span class="sxs-lookup"><span data-stu-id="5c2de-193">Determines which branch devices will receive their updates from Possible values are: `userDefined`, `all`, `businessReadyOnly`.</span></span>|



## <a name="response"></a><span data-ttu-id="5c2de-194">応答</span><span class="sxs-lookup"><span data-stu-id="5c2de-194">Response</span></span>
<span data-ttu-id="5c2de-195">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5c2de-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c2de-196">例</span><span class="sxs-lookup"><span data-stu-id="5c2de-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c2de-197">要求</span><span class="sxs-lookup"><span data-stu-id="5c2de-197">Request</span></span>
<span data-ttu-id="5c2de-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5c2de-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 898

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```

### <a name="response"></a><span data-ttu-id="5c2de-199">応答</span><span class="sxs-lookup"><span data-stu-id="5c2de-199">Response</span></span>
<span data-ttu-id="5c2de-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5c2de-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```



