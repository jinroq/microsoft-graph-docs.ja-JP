# <a name="create-manageddevice"></a><span data-ttu-id="3b0be-101">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="3b0be-101">Create managedDevice</span></span>

> <span data-ttu-id="3b0be-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b0be-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b0be-103">新しい [managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3b0be-103">Create a new [plannerBucket](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b0be-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="3b0be-104">Prerequisites</span></span>
<span data-ttu-id="3b0be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b0be-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b0be-107">Permission type</span></span>|<span data-ttu-id="3b0be-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b0be-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b0be-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b0be-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3b0be-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0be-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b0be-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b0be-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b0be-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b0be-112">Not supported.</span></span>|
|<span data-ttu-id="3b0be-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b0be-113">Application</span></span>|<span data-ttu-id="3b0be-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b0be-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b0be-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b0be-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="3b0be-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b0be-116">Request headers</span></span>
|<span data-ttu-id="3b0be-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b0be-117">Header</span></span>|<span data-ttu-id="3b0be-118">値</span><span class="sxs-lookup"><span data-stu-id="3b0be-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b0be-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b0be-119">Authorization</span></span>|<span data-ttu-id="3b0be-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3b0be-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3b0be-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3b0be-121">Accept</span></span>|<span data-ttu-id="3b0be-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3b0be-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b0be-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b0be-123">Request body</span></span>
<span data-ttu-id="3b0be-124">要求本文で、managedDevice オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3b0be-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="3b0be-125">次の表に、managedDevice の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3b0be-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="3b0be-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b0be-126">Property</span></span>|<span data-ttu-id="3b0be-127">型</span><span class="sxs-lookup"><span data-stu-id="3b0be-127">Type</span></span>|<span data-ttu-id="3b0be-128">説明</span><span class="sxs-lookup"><span data-stu-id="3b0be-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b0be-129">id</span><span class="sxs-lookup"><span data-stu-id="3b0be-129">id</span></span>|<span data-ttu-id="3b0be-130">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-130">String</span></span>|<span data-ttu-id="3b0be-131">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="3b0be-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="3b0be-132">userId</span><span class="sxs-lookup"><span data-stu-id="3b0be-132">userId</span></span>|<span data-ttu-id="3b0be-133">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-133">String</span></span>|<span data-ttu-id="3b0be-134">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="3b0be-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="3b0be-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="3b0be-135">DeviceName</span></span>|<span data-ttu-id="3b0be-136">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-136">String</span></span>|<span data-ttu-id="3b0be-137">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="3b0be-137">Name of the device</span></span>|
|<span data-ttu-id="3b0be-138">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="3b0be-138">deviceActionResults</span></span>|<span data-ttu-id="3b0be-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3b0be-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="3b0be-140">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="3b0be-140">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="3b0be-141">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0be-141">enrolledDateTime</span></span>|<span data-ttu-id="3b0be-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0be-142">DateTimeOffset</span></span>|<span data-ttu-id="3b0be-143">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="3b0be-143">Enrollment time of the device.</span></span>|
|<span data-ttu-id="3b0be-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0be-144">lastSyncDateTime</span></span>|<span data-ttu-id="3b0be-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0be-145">DateTimeOffset</span></span>|<span data-ttu-id="3b0be-146">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="3b0be-146">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="3b0be-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b0be-147">operatingSystem</span></span>|<span data-ttu-id="3b0be-148">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-148">String</span></span>|<span data-ttu-id="3b0be-149">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="3b0be-149">Operating system of the device.</span></span> <span data-ttu-id="3b0be-150">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="3b0be-150">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="3b0be-151">complianceState</span><span class="sxs-lookup"><span data-stu-id="3b0be-151">complianceState</span></span>|<span data-ttu-id="3b0be-152">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-152">String</span></span>|<span data-ttu-id="3b0be-153">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="3b0be-153">Compliance state of the device.</span></span> <span data-ttu-id="3b0be-154">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-154">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="3b0be-155">jailBroken</span><span class="sxs-lookup"><span data-stu-id="3b0be-155">jailBroken</span></span>|<span data-ttu-id="3b0be-156">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-156">String</span></span>|<span data-ttu-id="3b0be-157">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3b0be-157">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="3b0be-158">managementAgent</span><span class="sxs-lookup"><span data-stu-id="3b0be-158">managementAgent</span></span>|<span data-ttu-id="3b0be-159">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-159">String</span></span>|<span data-ttu-id="3b0be-160">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="3b0be-160">Management channel of the device.</span></span> <span data-ttu-id="3b0be-161">Intune、EAS など。可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController` です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-161">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="3b0be-162">osVersion</span><span class="sxs-lookup"><span data-stu-id="3b0be-162">osVersion</span></span>|<span data-ttu-id="3b0be-163">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-163">String</span></span>|<span data-ttu-id="3b0be-164">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="3b0be-164">Operating system version of the device.</span></span>|
|<span data-ttu-id="3b0be-165">easActivated</span><span class="sxs-lookup"><span data-stu-id="3b0be-165">easActivated</span></span>|<span data-ttu-id="3b0be-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0be-166">Boolean</span></span>|<span data-ttu-id="3b0be-167">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3b0be-167">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="3b0be-168">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="3b0be-168">easDeviceId</span></span>|<span data-ttu-id="3b0be-169">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-169">String</span></span>|<span data-ttu-id="3b0be-170">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="3b0be-170">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="3b0be-171">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0be-171">easActivationDateTime</span></span>|<span data-ttu-id="3b0be-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0be-172">DateTimeOffset</span></span>|<span data-ttu-id="3b0be-173">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="3b0be-173">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="3b0be-174">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="3b0be-174">azureADRegistered</span></span>|<span data-ttu-id="3b0be-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0be-175">Boolean</span></span>|<span data-ttu-id="3b0be-176">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3b0be-176">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="3b0be-177">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3b0be-177">deviceEnrollmentType</span></span>|<span data-ttu-id="3b0be-178">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-178">String</span></span>|<span data-ttu-id="3b0be-179">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="3b0be-179">Enrollment type of the device.</span></span> <span data-ttu-id="3b0be-180">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-180">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="3b0be-181">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="3b0be-181">activationLockBypassCode</span></span>|<span data-ttu-id="3b0be-182">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-182">String</span></span>|<span data-ttu-id="3b0be-183">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="3b0be-183">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="3b0be-184">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3b0be-184">emailAddress</span></span>|<span data-ttu-id="3b0be-185">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-185">String</span></span>|<span data-ttu-id="3b0be-186">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="3b0be-186">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="3b0be-187">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="3b0be-187">azureADDeviceId</span></span>|<span data-ttu-id="3b0be-188">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-188">String</span></span>|<span data-ttu-id="3b0be-189">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3b0be-189">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="3b0be-190">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-190">Read only.</span></span>|
|<span data-ttu-id="3b0be-191">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3b0be-191">deviceRegistrationState</span></span>|<span data-ttu-id="3b0be-192">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-192">String</span></span>|<span data-ttu-id="3b0be-193">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="3b0be-193">Device registration state.</span></span> <span data-ttu-id="3b0be-194">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-194">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`.</span></span>|
|<span data-ttu-id="3b0be-195">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="3b0be-195">deviceCategoryDisplayName</span></span>|<span data-ttu-id="3b0be-196">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-196">String</span></span>|<span data-ttu-id="3b0be-197">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="3b0be-197">Device category display name</span></span>|
|<span data-ttu-id="3b0be-198">isSupervised</span><span class="sxs-lookup"><span data-stu-id="3b0be-198">isSupervised</span></span>|<span data-ttu-id="3b0be-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0be-199">Boolean</span></span>|<span data-ttu-id="3b0be-200">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="3b0be-200">Device supervised status</span></span>|
|<span data-ttu-id="3b0be-201">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0be-201">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="3b0be-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0be-202">DateTimeOffset</span></span>|<span data-ttu-id="3b0be-203">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="3b0be-203">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="3b0be-204">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="3b0be-204">exchangeAccessState</span></span>|<span data-ttu-id="3b0be-205">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-205">String</span></span>|<span data-ttu-id="3b0be-206">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="3b0be-206">The Access State of the device in Exchange.</span></span> <span data-ttu-id="3b0be-207">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-207">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="3b0be-208">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="3b0be-208">exchangeAccessStateReason</span></span>|<span data-ttu-id="3b0be-209">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-209">String</span></span>|<span data-ttu-id="3b0be-210">Exchange でのデバイスの状態の理由。</span><span class="sxs-lookup"><span data-stu-id="3b0be-210">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="3b0be-211">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-211">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="3b0be-212">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="3b0be-212">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="3b0be-213">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-213">String</span></span>|<span data-ttu-id="3b0be-214">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="3b0be-214">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="3b0be-215">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3b0be-215">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="3b0be-216">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-216">String</span></span>|<span data-ttu-id="3b0be-217">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="3b0be-217">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="3b0be-218">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="3b0be-218">IsEncrypted</span></span>|<span data-ttu-id="3b0be-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0be-219">Boolean</span></span>|<span data-ttu-id="3b0be-220">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="3b0be-220">Device encryption status</span></span>|
|<span data-ttu-id="3b0be-221">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3b0be-221">userPrincipalName</span></span>|<span data-ttu-id="3b0be-222">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-222">String</span></span>|<span data-ttu-id="3b0be-223">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="3b0be-223">The user principal name.</span></span>|
|<span data-ttu-id="3b0be-224">model</span><span class="sxs-lookup"><span data-stu-id="3b0be-224">model</span></span>|<span data-ttu-id="3b0be-225">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-225">String</span></span>|<span data-ttu-id="3b0be-226">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="3b0be-226">Model of the device</span></span>|
|<span data-ttu-id="3b0be-227">manufacturer</span><span class="sxs-lookup"><span data-stu-id="3b0be-227">Camera manufacturer.</span></span>|<span data-ttu-id="3b0be-228">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-228">String</span></span>|<span data-ttu-id="3b0be-229">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="3b0be-229">Manufacturer of the device</span></span>|
|<span data-ttu-id="3b0be-230">imei</span><span class="sxs-lookup"><span data-stu-id="3b0be-230">imei</span></span>|<span data-ttu-id="3b0be-231">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-231">String</span></span>|<span data-ttu-id="3b0be-232">IMEI</span><span class="sxs-lookup"><span data-stu-id="3b0be-232">IMEI</span></span>|
|<span data-ttu-id="3b0be-233">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0be-233">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3b0be-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0be-234">DateTimeOffset</span></span>|<span data-ttu-id="3b0be-235">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="3b0be-235">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="3b0be-236">serialNumber</span><span class="sxs-lookup"><span data-stu-id="3b0be-236">serialNumber</span></span>|<span data-ttu-id="3b0be-237">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-237">String</span></span>|<span data-ttu-id="3b0be-238">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="3b0be-238">object  . SerialNumber</span></span>|
|<span data-ttu-id="3b0be-239">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="3b0be-239">PhoneNumber</span></span>|<span data-ttu-id="3b0be-240">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-240">String</span></span>|<span data-ttu-id="3b0be-241">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="3b0be-241">Phone number of the device</span></span>|
|<span data-ttu-id="3b0be-242">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="3b0be-242">androidSecurityPatchLevel</span></span>|<span data-ttu-id="3b0be-243">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-243">String</span></span>|<span data-ttu-id="3b0be-244">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="3b0be-244">Android security patch level</span></span>|
|<span data-ttu-id="3b0be-245">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3b0be-245">userDisplayName</span></span>|<span data-ttu-id="3b0be-246">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-246">String</span></span>|<span data-ttu-id="3b0be-247">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="3b0be-247">user display name</span></span>|
|<span data-ttu-id="3b0be-248">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3b0be-248">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="3b0be-249">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3b0be-249">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="3b0be-250">ConfigrMgr クライアントが有効になっている機能</span><span class="sxs-lookup"><span data-stu-id="3b0be-250">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="3b0be-251">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="3b0be-251">wiFiMacAddress</span></span>|<span data-ttu-id="3b0be-252">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-252">String</span></span>|<span data-ttu-id="3b0be-253">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="3b0be-253">Wi-Fi MAC</span></span>|
|<span data-ttu-id="3b0be-254">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3b0be-254">deviceHealthAttestationState</span></span>|[<span data-ttu-id="3b0be-255">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3b0be-255">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="3b0be-256">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="3b0be-256">The device health attestation state.</span></span>|
|<span data-ttu-id="3b0be-257">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="3b0be-257">subscriberCarrier</span></span>|<span data-ttu-id="3b0be-258">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-258">String</span></span>|<span data-ttu-id="3b0be-259">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="3b0be-259">Subscriber Carrier</span></span>|
|<span data-ttu-id="3b0be-260">meid</span><span class="sxs-lookup"><span data-stu-id="3b0be-260">meid</span></span>|<span data-ttu-id="3b0be-261">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-261">String</span></span>|<span data-ttu-id="3b0be-262">MEID</span><span class="sxs-lookup"><span data-stu-id="3b0be-262">MEID</span></span>|
|<span data-ttu-id="3b0be-263">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3b0be-263">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="3b0be-264">Int64</span><span class="sxs-lookup"><span data-stu-id="3b0be-264">Int64</span></span>|<span data-ttu-id="3b0be-265">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="3b0be-265">Total Storage in Bytes</span></span>|
|<span data-ttu-id="3b0be-266">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3b0be-266">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="3b0be-267">Int64</span><span class="sxs-lookup"><span data-stu-id="3b0be-267">Int64</span></span>|<span data-ttu-id="3b0be-268">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="3b0be-268">Free Storage in Bytes</span></span>|
|<span data-ttu-id="3b0be-269">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="3b0be-269">managedDeviceName</span></span>|<span data-ttu-id="3b0be-270">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-270">String</span></span>|<span data-ttu-id="3b0be-271">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="3b0be-271">Automatically generated name to identify a device.</span></span> <span data-ttu-id="3b0be-272">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="3b0be-272">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="3b0be-273">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="3b0be-273">partnerReportedThreatState</span></span>|<span data-ttu-id="3b0be-274">String</span><span class="sxs-lookup"><span data-stu-id="3b0be-274">String</span></span>|<span data-ttu-id="3b0be-275">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="3b0be-275">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="3b0be-276">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-276">Read Only</span></span> <span data-ttu-id="3b0be-277">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-277">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`.</span></span>|



## <a name="response"></a><span data-ttu-id="3b0be-278">応答</span><span class="sxs-lookup"><span data-stu-id="3b0be-278">Response</span></span>
<span data-ttu-id="3b0be-279">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3b0be-279">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b0be-280">例</span><span class="sxs-lookup"><span data-stu-id="3b0be-280">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b0be-281">要求</span><span class="sxs-lookup"><span data-stu-id="3b0be-281">Request</span></span>
<span data-ttu-id="3b0be-282">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3b0be-282">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4616

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
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

### <a name="response"></a><span data-ttu-id="3b0be-283">応答</span><span class="sxs-lookup"><span data-stu-id="3b0be-283">Response</span></span>
<span data-ttu-id="3b0be-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b0be-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4665

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
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



