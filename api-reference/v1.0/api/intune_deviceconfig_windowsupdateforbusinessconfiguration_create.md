# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="94238-101">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="94238-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="94238-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="94238-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94238-103">新しい [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="94238-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94238-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="94238-104">Prerequisites</span></span>
<span data-ttu-id="94238-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94238-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94238-107">Permission type</span></span>|<span data-ttu-id="94238-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="94238-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94238-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="94238-109">Delegated (work or school account)</span></span>|<span data-ttu-id="94238-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94238-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94238-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94238-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94238-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94238-112">Not supported.</span></span>|
|<span data-ttu-id="94238-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94238-113">Application</span></span>|<span data-ttu-id="94238-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94238-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94238-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94238-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="94238-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94238-116">Request headers</span></span>
|<span data-ttu-id="94238-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94238-117">Header</span></span>|<span data-ttu-id="94238-118">値</span><span class="sxs-lookup"><span data-stu-id="94238-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94238-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="94238-119">Authorization</span></span>|<span data-ttu-id="94238-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="94238-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="94238-121">Accept</span><span class="sxs-lookup"><span data-stu-id="94238-121">Accept</span></span>|<span data-ttu-id="94238-122">application/json</span><span class="sxs-lookup"><span data-stu-id="94238-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94238-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="94238-123">Request body</span></span>
<span data-ttu-id="94238-124">要求本文で、windowsUpdateForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94238-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="94238-125">次の表に、windowsUpdateForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="94238-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="94238-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94238-126">Property</span></span>|<span data-ttu-id="94238-127">型</span><span class="sxs-lookup"><span data-stu-id="94238-127">Type</span></span>|<span data-ttu-id="94238-128">説明</span><span class="sxs-lookup"><span data-stu-id="94238-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94238-129">id</span><span class="sxs-lookup"><span data-stu-id="94238-129">id</span></span>|<span data-ttu-id="94238-130">String</span><span class="sxs-lookup"><span data-stu-id="94238-130">String</span></span>|<span data-ttu-id="94238-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="94238-131">Name of the entity.</span></span> <span data-ttu-id="94238-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94238-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94238-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94238-133">lastModifiedDateTime</span></span>|<span data-ttu-id="94238-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94238-134">DateTimeOffset</span></span>|<span data-ttu-id="94238-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="94238-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="94238-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94238-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94238-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94238-137">createdDateTime</span></span>|<span data-ttu-id="94238-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94238-138">DateTimeOffset</span></span>|<span data-ttu-id="94238-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="94238-139">DateTime the object was created.</span></span> <span data-ttu-id="94238-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94238-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94238-141">description</span><span class="sxs-lookup"><span data-stu-id="94238-141">description</span></span>|<span data-ttu-id="94238-142">String</span><span class="sxs-lookup"><span data-stu-id="94238-142">String</span></span>|<span data-ttu-id="94238-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="94238-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="94238-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94238-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94238-145">displayName</span><span class="sxs-lookup"><span data-stu-id="94238-145">displayName</span></span>|<span data-ttu-id="94238-146">String</span><span class="sxs-lookup"><span data-stu-id="94238-146">String</span></span>|<span data-ttu-id="94238-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="94238-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="94238-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94238-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94238-149">version</span><span class="sxs-lookup"><span data-stu-id="94238-149">version</span></span>|<span data-ttu-id="94238-150">Int32</span><span class="sxs-lookup"><span data-stu-id="94238-150">Int32</span></span>|<span data-ttu-id="94238-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="94238-151">Version of the device configuration.</span></span> <span data-ttu-id="94238-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94238-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94238-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="94238-153">deliveryOptimizationMode</span></span>|<span data-ttu-id="94238-154">String</span><span class="sxs-lookup"><span data-stu-id="94238-154">String</span></span>|<span data-ttu-id="94238-155">配信最適化モードです。可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="94238-155">Delivery Optimization Mode Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="94238-156">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="94238-156">prereleaseFeatures</span></span>|<span data-ttu-id="94238-157">String</span><span class="sxs-lookup"><span data-stu-id="94238-157">String</span></span>|<span data-ttu-id="94238-158">プレリリース機能です。</span><span class="sxs-lookup"><span data-stu-id="94238-158">The pre-release features.</span></span> <span data-ttu-id="94238-159">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="94238-159">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="94238-160">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="94238-160">automaticUpdateMode</span></span>|<span data-ttu-id="94238-161">String</span><span class="sxs-lookup"><span data-stu-id="94238-161">String</span></span>|<span data-ttu-id="94238-162">自動更新モードです。</span><span class="sxs-lookup"><span data-stu-id="94238-162">Automatic update mode.</span></span> <span data-ttu-id="94238-163">可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` です。</span><span class="sxs-lookup"><span data-stu-id="94238-163">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="94238-164">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="94238-164">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="94238-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="94238-165">Boolean</span></span>|<span data-ttu-id="94238-166">Microsoft の更新サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="94238-166">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="94238-167">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="94238-167">driversExcluded</span></span>|<span data-ttu-id="94238-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="94238-168">Boolean</span></span>|<span data-ttu-id="94238-169">Windows 更新ドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="94238-169">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="94238-170">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="94238-170">installationSchedule</span></span>|[<span data-ttu-id="94238-171">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="94238-171">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="94238-172">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="94238-172">Installation schedule</span></span>|
|<span data-ttu-id="94238-173">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="94238-173">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="94238-174">Int32</span><span class="sxs-lookup"><span data-stu-id="94238-174">Int32</span></span>|<span data-ttu-id="94238-175">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="94238-175">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="94238-176">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="94238-176">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="94238-177">Int32</span><span class="sxs-lookup"><span data-stu-id="94238-177">Int32</span></span>|<span data-ttu-id="94238-178">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="94238-178">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="94238-179">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="94238-179">qualityUpdatesPaused</span></span>|<span data-ttu-id="94238-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="94238-180">Boolean</span></span>|<span data-ttu-id="94238-181">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="94238-181">Pause Quality Updates</span></span>|
|<span data-ttu-id="94238-182">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="94238-182">featureUpdatesPaused</span></span>|<span data-ttu-id="94238-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="94238-183">Boolean</span></span>|<span data-ttu-id="94238-184">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="94238-184">Pause Feature Updates</span></span>|
|<span data-ttu-id="94238-185">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="94238-185">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="94238-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94238-186">DateTimeOffset</span></span>|<span data-ttu-id="94238-187">品質更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="94238-187">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="94238-188">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="94238-188">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="94238-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94238-189">DateTimeOffset</span></span>|<span data-ttu-id="94238-190">機能更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="94238-190">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="94238-191">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="94238-191">businessReadyUpdatesOnly</span></span>|<span data-ttu-id="94238-192">String</span><span class="sxs-lookup"><span data-stu-id="94238-192">String</span></span>|<span data-ttu-id="94238-193">デバイスが、どのブランチから更新を受け取るかを決定します。可能な値は、`userDefined`、`all`、`businessReadyOnly` です。</span><span class="sxs-lookup"><span data-stu-id="94238-193">Determines which branch devices will receive their updates from Possible values are: `userDefined`, `all`, `businessReadyOnly`.</span></span>|



## <a name="response"></a><span data-ttu-id="94238-194">応答</span><span class="sxs-lookup"><span data-stu-id="94238-194">Response</span></span>
<span data-ttu-id="94238-195">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94238-195">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94238-196">例</span><span class="sxs-lookup"><span data-stu-id="94238-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="94238-197">要求</span><span class="sxs-lookup"><span data-stu-id="94238-197">Request</span></span>
<span data-ttu-id="94238-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94238-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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

### <a name="response"></a><span data-ttu-id="94238-199">応答</span><span class="sxs-lookup"><span data-stu-id="94238-199">Response</span></span>
<span data-ttu-id="94238-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94238-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



