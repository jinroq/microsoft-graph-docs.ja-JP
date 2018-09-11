# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="7c220-101">windowsUpdateForBusinessConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="7c220-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="7c220-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c220-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c220-103">新しい [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7c220-103">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c220-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c220-104">Prerequisites</span></span>
<span data-ttu-id="7c220-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c220-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c220-107">Permission type</span></span>|<span data-ttu-id="7c220-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c220-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c220-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c220-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7c220-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c220-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c220-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c220-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c220-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c220-112">Not supported.</span></span>|
|<span data-ttu-id="7c220-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c220-113">Application</span></span>|<span data-ttu-id="7c220-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c220-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c220-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c220-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7c220-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c220-116">Request headers</span></span>
|<span data-ttu-id="7c220-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c220-117">Header</span></span>|<span data-ttu-id="7c220-118">値</span><span class="sxs-lookup"><span data-stu-id="7c220-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c220-119">承認</span><span class="sxs-lookup"><span data-stu-id="7c220-119">Authorization</span></span>|<span data-ttu-id="7c220-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7c220-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c220-121">承諾</span><span class="sxs-lookup"><span data-stu-id="7c220-121">Accept</span></span>|<span data-ttu-id="7c220-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="7c220-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c220-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c220-123">Request body</span></span>
<span data-ttu-id="7c220-124">要求本文で、windowsUpdateForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c220-124">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="7c220-125">次の表に、windowsUpdateForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7c220-125">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="7c220-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c220-126">Property</span></span>|<span data-ttu-id="7c220-127">型</span><span class="sxs-lookup"><span data-stu-id="7c220-127">Type</span></span>|<span data-ttu-id="7c220-128">説明</span><span class="sxs-lookup"><span data-stu-id="7c220-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c220-129">ID</span><span class="sxs-lookup"><span data-stu-id="7c220-129">id</span></span>|<span data-ttu-id="7c220-130">文字列</span><span class="sxs-lookup"><span data-stu-id="7c220-130">String</span></span>|<span data-ttu-id="7c220-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7c220-131">Key of the entity.</span></span> <span data-ttu-id="7c220-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7c220-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c220-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c220-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7c220-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c220-134">DateTimeOffset</span></span>|<span data-ttu-id="7c220-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7c220-135">DateTime the object was last modified.</span></span> <span data-ttu-id="7c220-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7c220-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c220-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c220-137">createdDateTime</span></span>|<span data-ttu-id="7c220-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c220-138">DateTimeOffset</span></span>|<span data-ttu-id="7c220-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7c220-139">DateTime the object was created.</span></span> <span data-ttu-id="7c220-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7c220-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c220-141">説明</span><span class="sxs-lookup"><span data-stu-id="7c220-141">description</span></span>|<span data-ttu-id="7c220-142">文字列</span><span class="sxs-lookup"><span data-stu-id="7c220-142">String</span></span>|<span data-ttu-id="7c220-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7c220-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7c220-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7c220-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c220-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7c220-145">displayName</span></span>|<span data-ttu-id="7c220-146">文字列</span><span class="sxs-lookup"><span data-stu-id="7c220-146">String</span></span>|<span data-ttu-id="7c220-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7c220-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7c220-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7c220-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c220-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="7c220-149">version</span></span>|<span data-ttu-id="7c220-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7c220-150">Int32</span></span>|<span data-ttu-id="7c220-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7c220-151">Version of the device configuration.</span></span> <span data-ttu-id="7c220-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7c220-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c220-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="7c220-153">deliveryOptimizationMode</span></span>|[<span data-ttu-id="7c220-154">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="7c220-154">windowsDeliveryOptimizationMode</span></span>](../resources/intune_deviceconfig_windowsdeliveryoptimizationmode.md)|<span data-ttu-id="7c220-155">配信最適化モードです。</span><span class="sxs-lookup"><span data-stu-id="7c220-155">Delivery Optimization Mode Possible values are: , , , , , , .</span></span> <span data-ttu-id="7c220-156">使用可能な値は`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="7c220-156">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="7c220-157">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="7c220-157">prereleaseFeatures</span></span>|[<span data-ttu-id="7c220-158">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="7c220-158">prereleaseFeatures</span></span>](../resources/intune_deviceconfig_prereleasefeatures.md)|<span data-ttu-id="7c220-159">プレリリース機能です。</span><span class="sxs-lookup"><span data-stu-id="7c220-159">The pre-release features.</span></span> <span data-ttu-id="7c220-160">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="7c220-160">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="7c220-161">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="7c220-161">automaticUpdateMode</span></span>|[<span data-ttu-id="7c220-162">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="7c220-162">automaticUpdateMode</span></span>](../resources/intune_deviceconfig_automaticupdatemode.md)|<span data-ttu-id="7c220-163">自動更新モードです。</span><span class="sxs-lookup"><span data-stu-id="7c220-163">Automatic update mode.</span></span> <span data-ttu-id="7c220-164">使用可能な値は`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` です。</span><span class="sxs-lookup"><span data-stu-id="7c220-164">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="7c220-165">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="7c220-165">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="7c220-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="7c220-166">Boolean</span></span>|<span data-ttu-id="7c220-167">Microsoft の更新サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="7c220-167">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="7c220-168">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="7c220-168">driversExcluded</span></span>|<span data-ttu-id="7c220-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="7c220-169">Boolean</span></span>|<span data-ttu-id="7c220-170">Windows 更新ドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="7c220-170">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="7c220-171">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="7c220-171">installationSchedule</span></span>|[<span data-ttu-id="7c220-172">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="7c220-172">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="7c220-173">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="7c220-173">Installation schedule</span></span>|
|<span data-ttu-id="7c220-174">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="7c220-174">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="7c220-175">Int32</span><span class="sxs-lookup"><span data-stu-id="7c220-175">Int32</span></span>|<span data-ttu-id="7c220-176">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="7c220-176">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="7c220-177">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="7c220-177">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="7c220-178">Int32</span><span class="sxs-lookup"><span data-stu-id="7c220-178">Int32</span></span>|<span data-ttu-id="7c220-179">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="7c220-179">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="7c220-180">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="7c220-180">qualityUpdatesPaused</span></span>|<span data-ttu-id="7c220-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="7c220-181">Boolean</span></span>|<span data-ttu-id="7c220-182">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="7c220-182">Pause Quality Updates</span></span>|
|<span data-ttu-id="7c220-183">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="7c220-183">featureUpdatesPaused</span></span>|<span data-ttu-id="7c220-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="7c220-184">Boolean</span></span>|<span data-ttu-id="7c220-185">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="7c220-185">Pause Feature Updates</span></span>|
|<span data-ttu-id="7c220-186">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="7c220-186">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="7c220-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c220-187">DateTimeOffset</span></span>|<span data-ttu-id="7c220-188">品質更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="7c220-188">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="7c220-189">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="7c220-189">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="7c220-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c220-190">DateTimeOffset</span></span>|<span data-ttu-id="7c220-191">機能更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="7c220-191">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="7c220-192">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="7c220-192">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="7c220-193">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="7c220-193">windowsUpdateType</span></span>](../resources/intune_deviceconfig_windowsupdatetype.md)|<span data-ttu-id="7c220-194">デバイスがどのブランチから更新を受け取るかを決定します。</span><span class="sxs-lookup"><span data-stu-id="7c220-194">Determines which branch devices will receive their updates from Possible values are: , , .</span></span> <span data-ttu-id="7c220-195">使用可能な値は`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease` です。</span><span class="sxs-lookup"><span data-stu-id="7c220-195">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="7c220-196">応答</span><span class="sxs-lookup"><span data-stu-id="7c220-196">Response</span></span>
<span data-ttu-id="7c220-197">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c220-197">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c220-198">例</span><span class="sxs-lookup"><span data-stu-id="7c220-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c220-199">要求</span><span class="sxs-lookup"><span data-stu-id="7c220-199">Request</span></span>
<span data-ttu-id="7c220-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c220-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c220-201">応答</span><span class="sxs-lookup"><span data-stu-id="7c220-201">Response</span></span>
<span data-ttu-id="7c220-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c220-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








