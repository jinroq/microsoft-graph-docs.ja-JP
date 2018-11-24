# <a name="update-manageddevice"></a><span data-ttu-id="5bf9a-101">managedDevice の更新
</span><span class="sxs-lookup"><span data-stu-id="5bf9a-101">Update managedDevice</span></span>

> <span data-ttu-id="5bf9a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5bf9a-103">[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-103">Update the properties of a [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5bf9a-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5bf9a-104">Prerequisites</span></span>
<span data-ttu-id="5bf9a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5bf9a-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5bf9a-107">Permission type</span></span>|<span data-ttu-id="5bf9a-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5bf9a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bf9a-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bf9a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5bf9a-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bf9a-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5bf9a-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bf9a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bf9a-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-112">Not supported.</span></span>|
|<span data-ttu-id="5bf9a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5bf9a-113">Application</span></span>|<span data-ttu-id="5bf9a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bf9a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bf9a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="5bf9a-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bf9a-116">Request headers</span></span>
|<span data-ttu-id="5bf9a-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bf9a-117">Header</span></span>|<span data-ttu-id="5bf9a-118">値</span><span class="sxs-lookup"><span data-stu-id="5bf9a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bf9a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bf9a-119">Authorization</span></span>|<span data-ttu-id="5bf9a-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bf9a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5bf9a-121">Accept</span></span>|<span data-ttu-id="5bf9a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5bf9a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bf9a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bf9a-123">Request body</span></span>
<span data-ttu-id="5bf9a-124">要求本文で、[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-124">In the request body, supply a JSON representation for the [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>

<span data-ttu-id="5bf9a-125">次の表に、[managedDevice](../resources/intune_devices_manageddevice.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-125">The following table shows the properties that are required when you create the [managedDevice](../resources/intune_devices_manageddevice.md).</span></span>

|<span data-ttu-id="5bf9a-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bf9a-126">Property</span></span>|<span data-ttu-id="5bf9a-127">型</span><span class="sxs-lookup"><span data-stu-id="5bf9a-127">Type</span></span>|<span data-ttu-id="5bf9a-128">説明</span><span class="sxs-lookup"><span data-stu-id="5bf9a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bf9a-129">id</span><span class="sxs-lookup"><span data-stu-id="5bf9a-129">id</span></span>|<span data-ttu-id="5bf9a-130">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-130">String</span></span>|<span data-ttu-id="5bf9a-131">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="5bf9a-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="5bf9a-132">userId</span><span class="sxs-lookup"><span data-stu-id="5bf9a-132">userId</span></span>|<span data-ttu-id="5bf9a-133">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-133">String</span></span>|<span data-ttu-id="5bf9a-134">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="5bf9a-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="5bf9a-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="5bf9a-135">deviceName</span></span>|<span data-ttu-id="5bf9a-136">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-136">String</span></span>|<span data-ttu-id="5bf9a-137">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="5bf9a-137">Name of the device</span></span>|
|<span data-ttu-id="5bf9a-138">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="5bf9a-138">managedDeviceOwnerType</span></span>|[<span data-ttu-id="5bf9a-139">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="5bf9a-139">managedDeviceOwnerType</span></span>](../resources/intune_devices_manageddeviceownertype.md)|<span data-ttu-id="5bf9a-140">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-140">Ownership of the device.</span></span> <span data-ttu-id="5bf9a-141">'会社' または '個人' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-141">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="5bf9a-142">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-142">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="5bf9a-143">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="5bf9a-143">deviceActionResults</span></span>|<span data-ttu-id="5bf9a-144">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5bf9a-144">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="5bf9a-145">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-145">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="5bf9a-146">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="5bf9a-146">enrolledDateTime</span></span>|<span data-ttu-id="5bf9a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bf9a-147">DateTimeOffset</span></span>|<span data-ttu-id="5bf9a-148">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-148">Enrollment time of the device.</span></span>|
|<span data-ttu-id="5bf9a-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5bf9a-149">lastSyncDateTime</span></span>|<span data-ttu-id="5bf9a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bf9a-150">DateTimeOffset</span></span>|<span data-ttu-id="5bf9a-151">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-151">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="5bf9a-152">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="5bf9a-152">operatingSystem</span></span>|<span data-ttu-id="5bf9a-153">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-153">String</span></span>|<span data-ttu-id="5bf9a-154">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-154">Operating system of the device.</span></span> <span data-ttu-id="5bf9a-155">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-155">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="5bf9a-156">complianceState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-156">complianceState</span></span>|[<span data-ttu-id="5bf9a-157">complianceState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-157">complianceState</span></span>](../resources/intune_devices_compliancestate.md)|<span data-ttu-id="5bf9a-158">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-158">Compliance state of the device.</span></span> <span data-ttu-id="5bf9a-159">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-159">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="5bf9a-160">jailBroken</span><span class="sxs-lookup"><span data-stu-id="5bf9a-160">jailBroken</span></span>|<span data-ttu-id="5bf9a-161">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-161">String</span></span>|<span data-ttu-id="5bf9a-162">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-162">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="5bf9a-163">managementAgent</span><span class="sxs-lookup"><span data-stu-id="5bf9a-163">managementAgent</span></span>|[<span data-ttu-id="5bf9a-164">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="5bf9a-164">managementAgentType</span></span>](../resources/intune_devices_managementagenttype.md)|<span data-ttu-id="5bf9a-165">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-165">Management channel of the device.</span></span> <span data-ttu-id="5bf9a-166">Intune、EAS など。可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController` です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-166">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="5bf9a-167">osVersion</span><span class="sxs-lookup"><span data-stu-id="5bf9a-167">osVersion</span></span>|<span data-ttu-id="5bf9a-168">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-168">String</span></span>|<span data-ttu-id="5bf9a-169">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-169">Operating system version of the device.</span></span>|
|<span data-ttu-id="5bf9a-170">easActivated</span><span class="sxs-lookup"><span data-stu-id="5bf9a-170">easActivated</span></span>|<span data-ttu-id="5bf9a-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bf9a-171">Boolean</span></span>|<span data-ttu-id="5bf9a-172">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-172">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="5bf9a-173">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="5bf9a-173">easDeviceId</span></span>|<span data-ttu-id="5bf9a-174">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-174">String</span></span>|<span data-ttu-id="5bf9a-175">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-175">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="5bf9a-176">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="5bf9a-176">easActivationDateTime</span></span>|<span data-ttu-id="5bf9a-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bf9a-177">DateTimeOffset</span></span>|<span data-ttu-id="5bf9a-178">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-178">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="5bf9a-179">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="5bf9a-179">azureADRegistered</span></span>|<span data-ttu-id="5bf9a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bf9a-180">Boolean</span></span>|<span data-ttu-id="5bf9a-181">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-181">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="5bf9a-182">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5bf9a-182">deviceEnrollmentType</span></span>|[<span data-ttu-id="5bf9a-183">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5bf9a-183">deviceEnrollmentType</span></span>](../resources/intune_devices_deviceenrollmenttype.md)|<span data-ttu-id="5bf9a-184">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-184">Enrollment type of the device.</span></span> <span data-ttu-id="5bf9a-185">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-185">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="5bf9a-186">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="5bf9a-186">activationLockBypassCode</span></span>|<span data-ttu-id="5bf9a-187">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-187">String</span></span>|<span data-ttu-id="5bf9a-188">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-188">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="5bf9a-189">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5bf9a-189">emailAddress</span></span>|<span data-ttu-id="5bf9a-190">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-190">String</span></span>|<span data-ttu-id="5bf9a-191">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="5bf9a-191">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="5bf9a-192">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="5bf9a-192">azureADDeviceId</span></span>|<span data-ttu-id="5bf9a-193">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-193">String</span></span>|<span data-ttu-id="5bf9a-194">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-194">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="5bf9a-195">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-195">Read only.</span></span>|
|<span data-ttu-id="5bf9a-196">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-196">deviceRegistrationState</span></span>|[<span data-ttu-id="5bf9a-197">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-197">deviceRegistrationState</span></span>](../resources/intune_devices_deviceregistrationstate.md)|<span data-ttu-id="5bf9a-198">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-198">Device registration state.</span></span> <span data-ttu-id="5bf9a-199">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-199">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="5bf9a-200">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="5bf9a-200">deviceCategoryDisplayName</span></span>|<span data-ttu-id="5bf9a-201">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-201">String</span></span>|<span data-ttu-id="5bf9a-202">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="5bf9a-202">Device category display name</span></span>|
|<span data-ttu-id="5bf9a-203">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5bf9a-203">isSupervised</span></span>|<span data-ttu-id="5bf9a-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bf9a-204">Boolean</span></span>|<span data-ttu-id="5bf9a-205">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="5bf9a-205">Device supervised status</span></span>|
|<span data-ttu-id="5bf9a-206">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5bf9a-206">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="5bf9a-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bf9a-207">DateTimeOffset</span></span>|<span data-ttu-id="5bf9a-208">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-208">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="5bf9a-209">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-209">exchangeAccessState</span></span>|[<span data-ttu-id="5bf9a-210">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-210">deviceManagementExchangeAccessState</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|<span data-ttu-id="5bf9a-211">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-211">The Access State of the device in Exchange.</span></span> <span data-ttu-id="5bf9a-212">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-212">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="5bf9a-213">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="5bf9a-213">exchangeAccessStateReason</span></span>|[<span data-ttu-id="5bf9a-214">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="5bf9a-214">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="5bf9a-215">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="5bf9a-215">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="5bf9a-216">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-216">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="5bf9a-217">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="5bf9a-217">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="5bf9a-218">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-218">String</span></span>|<span data-ttu-id="5bf9a-219">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-219">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="5bf9a-220">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5bf9a-220">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="5bf9a-221">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-221">String</span></span>|<span data-ttu-id="5bf9a-222">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-222">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="5bf9a-223">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="5bf9a-223">isEncrypted</span></span>|<span data-ttu-id="5bf9a-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bf9a-224">Boolean</span></span>|<span data-ttu-id="5bf9a-225">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="5bf9a-225">Device encryption status</span></span>|
|<span data-ttu-id="5bf9a-226">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5bf9a-226">userPrincipalName</span></span>|<span data-ttu-id="5bf9a-227">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-227">String</span></span>|<span data-ttu-id="5bf9a-228">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-228">Device user principal name</span></span>|
|<span data-ttu-id="5bf9a-229">model</span><span class="sxs-lookup"><span data-stu-id="5bf9a-229">model</span></span>|<span data-ttu-id="5bf9a-230">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-230">String</span></span>|<span data-ttu-id="5bf9a-231">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="5bf9a-231">Model of the device</span></span>|
|<span data-ttu-id="5bf9a-232">manufacturer</span><span class="sxs-lookup"><span data-stu-id="5bf9a-232">manufacturer</span></span>|<span data-ttu-id="5bf9a-233">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-233">String</span></span>|<span data-ttu-id="5bf9a-234">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="5bf9a-234">Manufacturer of the device</span></span>|
|<span data-ttu-id="5bf9a-235">imei</span><span class="sxs-lookup"><span data-stu-id="5bf9a-235">imei</span></span>|<span data-ttu-id="5bf9a-236">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-236">String</span></span>|<span data-ttu-id="5bf9a-237">IMEI</span><span class="sxs-lookup"><span data-stu-id="5bf9a-237">IMEI</span></span>|
|<span data-ttu-id="5bf9a-238">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5bf9a-238">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5bf9a-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bf9a-239">DateTimeOffset</span></span>|<span data-ttu-id="5bf9a-240">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="5bf9a-240">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="5bf9a-241">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5bf9a-241">serialNumber</span></span>|<span data-ttu-id="5bf9a-242">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-242">String</span></span>|<span data-ttu-id="5bf9a-243">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="5bf9a-243">SerialNumber</span></span>|
|<span data-ttu-id="5bf9a-244">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="5bf9a-244">phoneNumber</span></span>|<span data-ttu-id="5bf9a-245">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-245">String</span></span>|<span data-ttu-id="5bf9a-246">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="5bf9a-246">Phone number of the device</span></span>|
|<span data-ttu-id="5bf9a-247">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="5bf9a-247">androidSecurityPatchLevel</span></span>|<span data-ttu-id="5bf9a-248">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-248">String</span></span>|<span data-ttu-id="5bf9a-249">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="5bf9a-249">Android security patch level</span></span>|
|<span data-ttu-id="5bf9a-250">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5bf9a-250">userDisplayName</span></span>|<span data-ttu-id="5bf9a-251">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-251">String</span></span>|<span data-ttu-id="5bf9a-252">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="5bf9a-252">User display name</span></span>|
|<span data-ttu-id="5bf9a-253">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5bf9a-253">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="5bf9a-254">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5bf9a-254">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="5bf9a-255">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="5bf9a-255">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="5bf9a-256">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="5bf9a-256">wiFiMacAddress</span></span>|<span data-ttu-id="5bf9a-257">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-257">String</span></span>|<span data-ttu-id="5bf9a-258">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="5bf9a-258">Wi-Fi MAC</span></span>|
|<span data-ttu-id="5bf9a-259">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-259">deviceHealthAttestationState</span></span>|[<span data-ttu-id="5bf9a-260">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-260">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="5bf9a-261">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-261">The device health attestation state.</span></span>|
|<span data-ttu-id="5bf9a-262">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="5bf9a-262">subscriberCarrier</span></span>|<span data-ttu-id="5bf9a-263">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-263">String</span></span>|<span data-ttu-id="5bf9a-264">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="5bf9a-264">Subscriber Carrier</span></span>|
|<span data-ttu-id="5bf9a-265">meid</span><span class="sxs-lookup"><span data-stu-id="5bf9a-265">meid</span></span>|<span data-ttu-id="5bf9a-266">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-266">String</span></span>|<span data-ttu-id="5bf9a-267">MEID</span><span class="sxs-lookup"><span data-stu-id="5bf9a-267">MEID</span></span>|
|<span data-ttu-id="5bf9a-268">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="5bf9a-268">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="5bf9a-269">Int64</span><span class="sxs-lookup"><span data-stu-id="5bf9a-269">Int64</span></span>|<span data-ttu-id="5bf9a-270">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="5bf9a-270">Total Storage in Bytes</span></span>|
|<span data-ttu-id="5bf9a-271">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="5bf9a-271">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="5bf9a-272">Int64</span><span class="sxs-lookup"><span data-stu-id="5bf9a-272">Int64</span></span>|<span data-ttu-id="5bf9a-273">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="5bf9a-273">Free Storage in Bytes</span></span>|
|<span data-ttu-id="5bf9a-274">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="5bf9a-274">managedDeviceName</span></span>|<span data-ttu-id="5bf9a-275">String</span><span class="sxs-lookup"><span data-stu-id="5bf9a-275">String</span></span>|<span data-ttu-id="5bf9a-276">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-276">Automatically generated name to identify a device.</span></span> <span data-ttu-id="5bf9a-277">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-277">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="5bf9a-278">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-278">partnerReportedThreatState</span></span>|[<span data-ttu-id="5bf9a-279">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="5bf9a-279">managedDevicePartnerReportedHealthState</span></span>](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="5bf9a-280">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-280">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="5bf9a-281">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-281">Read Only.</span></span> <span data-ttu-id="5bf9a-282">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-282">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="5bf9a-283">応答</span><span class="sxs-lookup"><span data-stu-id="5bf9a-283">Response</span></span>
<span data-ttu-id="5bf9a-284">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-284">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bf9a-285">例</span><span class="sxs-lookup"><span data-stu-id="5bf9a-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bf9a-286">要求</span><span class="sxs-lookup"><span data-stu-id="5bf9a-286">Request</span></span>
<span data-ttu-id="5bf9a-287">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-287">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4656

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="5bf9a-288">応答</span><span class="sxs-lookup"><span data-stu-id="5bf9a-288">Response</span></span>
<span data-ttu-id="5bf9a-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5bf9a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4705

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```



