# <a name="update-manageddevice"></a><span data-ttu-id="186ae-101">managedDevice の更新
</span><span class="sxs-lookup"><span data-stu-id="186ae-101">Update managedDevice</span></span>

> <span data-ttu-id="186ae-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="186ae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="186ae-103">[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="186ae-103">Update the properties of a [calendar](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="186ae-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="186ae-104">Prerequisites</span></span>
<span data-ttu-id="186ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="186ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="186ae-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="186ae-107">Permission type</span></span>|<span data-ttu-id="186ae-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="186ae-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="186ae-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="186ae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="186ae-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="186ae-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="186ae-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="186ae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="186ae-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="186ae-112">Not supported.</span></span>|
|<span data-ttu-id="186ae-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="186ae-113">Application</span></span>|<span data-ttu-id="186ae-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="186ae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="186ae-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="186ae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="186ae-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="186ae-116">Request headers</span></span>
|<span data-ttu-id="186ae-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="186ae-117">Header</span></span>|<span data-ttu-id="186ae-118">値</span><span class="sxs-lookup"><span data-stu-id="186ae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="186ae-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="186ae-119">Authorization</span></span>|<span data-ttu-id="186ae-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="186ae-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="186ae-121">Accept</span><span class="sxs-lookup"><span data-stu-id="186ae-121">Accept</span></span>|<span data-ttu-id="186ae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="186ae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="186ae-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="186ae-123">Request body</span></span>
<span data-ttu-id="186ae-124">要求本文で、[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="186ae-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_manageddevice.md) object.</span></span>

<span data-ttu-id="186ae-125">次の表に、[managedDevice](../resources/intune_devices_manageddevice.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="186ae-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="186ae-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="186ae-126">Property</span></span>|<span data-ttu-id="186ae-127">型</span><span class="sxs-lookup"><span data-stu-id="186ae-127">Type</span></span>|<span data-ttu-id="186ae-128">説明</span><span class="sxs-lookup"><span data-stu-id="186ae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="186ae-129">id</span><span class="sxs-lookup"><span data-stu-id="186ae-129">id</span></span>|<span data-ttu-id="186ae-130">String</span><span class="sxs-lookup"><span data-stu-id="186ae-130">String</span></span>|<span data-ttu-id="186ae-131">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="186ae-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="186ae-132">userId</span><span class="sxs-lookup"><span data-stu-id="186ae-132">userId</span></span>|<span data-ttu-id="186ae-133">String</span><span class="sxs-lookup"><span data-stu-id="186ae-133">String</span></span>|<span data-ttu-id="186ae-134">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="186ae-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="186ae-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="186ae-135">DeviceName</span></span>|<span data-ttu-id="186ae-136">String</span><span class="sxs-lookup"><span data-stu-id="186ae-136">String</span></span>|<span data-ttu-id="186ae-137">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="186ae-137">Name of the device</span></span>|
|<span data-ttu-id="186ae-138">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="186ae-138">deviceActionResults</span></span>|<span data-ttu-id="186ae-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="186ae-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="186ae-140">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="186ae-140">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="186ae-141">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="186ae-141">enrolledDateTime</span></span>|<span data-ttu-id="186ae-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186ae-142">DateTimeOffset</span></span>|<span data-ttu-id="186ae-143">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="186ae-143">Enrollment time of the device.</span></span>|
|<span data-ttu-id="186ae-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="186ae-144">lastSyncDateTime</span></span>|<span data-ttu-id="186ae-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186ae-145">DateTimeOffset</span></span>|<span data-ttu-id="186ae-146">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="186ae-146">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="186ae-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="186ae-147">operatingSystem</span></span>|<span data-ttu-id="186ae-148">String</span><span class="sxs-lookup"><span data-stu-id="186ae-148">String</span></span>|<span data-ttu-id="186ae-149">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="186ae-149">Operating system of the device.</span></span> <span data-ttu-id="186ae-150">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="186ae-150">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="186ae-151">complianceState</span><span class="sxs-lookup"><span data-stu-id="186ae-151">complianceState</span></span>|<span data-ttu-id="186ae-152">String</span><span class="sxs-lookup"><span data-stu-id="186ae-152">String</span></span>|<span data-ttu-id="186ae-153">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="186ae-153">Compliance state of the device.</span></span> <span data-ttu-id="186ae-154">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="186ae-154">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="186ae-155">jailBroken</span><span class="sxs-lookup"><span data-stu-id="186ae-155">jailBroken</span></span>|<span data-ttu-id="186ae-156">String</span><span class="sxs-lookup"><span data-stu-id="186ae-156">String</span></span>|<span data-ttu-id="186ae-157">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="186ae-157">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="186ae-158">managementAgent</span><span class="sxs-lookup"><span data-stu-id="186ae-158">managementAgent</span></span>|<span data-ttu-id="186ae-159">String</span><span class="sxs-lookup"><span data-stu-id="186ae-159">String</span></span>|<span data-ttu-id="186ae-160">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="186ae-160">Management channel of the device.</span></span> <span data-ttu-id="186ae-161">Intune、EAS など。可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController` です。</span><span class="sxs-lookup"><span data-stu-id="186ae-161">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="186ae-162">osVersion</span><span class="sxs-lookup"><span data-stu-id="186ae-162">osVersion</span></span>|<span data-ttu-id="186ae-163">String</span><span class="sxs-lookup"><span data-stu-id="186ae-163">String</span></span>|<span data-ttu-id="186ae-164">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="186ae-164">Operating system version of the device.</span></span>|
|<span data-ttu-id="186ae-165">easActivated</span><span class="sxs-lookup"><span data-stu-id="186ae-165">easActivated</span></span>|<span data-ttu-id="186ae-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="186ae-166">Boolean</span></span>|<span data-ttu-id="186ae-167">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="186ae-167">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="186ae-168">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="186ae-168">easDeviceId</span></span>|<span data-ttu-id="186ae-169">String</span><span class="sxs-lookup"><span data-stu-id="186ae-169">String</span></span>|<span data-ttu-id="186ae-170">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="186ae-170">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="186ae-171">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="186ae-171">easActivationDateTime</span></span>|<span data-ttu-id="186ae-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186ae-172">DateTimeOffset</span></span>|<span data-ttu-id="186ae-173">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="186ae-173">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="186ae-174">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="186ae-174">azureADRegistered</span></span>|<span data-ttu-id="186ae-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="186ae-175">Boolean</span></span>|<span data-ttu-id="186ae-176">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="186ae-176">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="186ae-177">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="186ae-177">deviceEnrollmentType</span></span>|<span data-ttu-id="186ae-178">String</span><span class="sxs-lookup"><span data-stu-id="186ae-178">String</span></span>|<span data-ttu-id="186ae-179">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="186ae-179">Enrollment type of the device.</span></span> <span data-ttu-id="186ae-180">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="186ae-180">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="186ae-181">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="186ae-181">activationLockBypassCode</span></span>|<span data-ttu-id="186ae-182">String</span><span class="sxs-lookup"><span data-stu-id="186ae-182">String</span></span>|<span data-ttu-id="186ae-183">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="186ae-183">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="186ae-184">emailAddress</span><span class="sxs-lookup"><span data-stu-id="186ae-184">emailAddress</span></span>|<span data-ttu-id="186ae-185">String</span><span class="sxs-lookup"><span data-stu-id="186ae-185">String</span></span>|<span data-ttu-id="186ae-186">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="186ae-186">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="186ae-187">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="186ae-187">azureADDeviceId</span></span>|<span data-ttu-id="186ae-188">String</span><span class="sxs-lookup"><span data-stu-id="186ae-188">String</span></span>|<span data-ttu-id="186ae-189">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="186ae-189">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="186ae-190">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="186ae-190">Read only.</span></span>|
|<span data-ttu-id="186ae-191">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="186ae-191">deviceRegistrationState</span></span>|<span data-ttu-id="186ae-192">String</span><span class="sxs-lookup"><span data-stu-id="186ae-192">String</span></span>|<span data-ttu-id="186ae-193">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="186ae-193">Device registration state.</span></span> <span data-ttu-id="186ae-194">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="186ae-194">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`.</span></span>|
|<span data-ttu-id="186ae-195">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="186ae-195">deviceCategoryDisplayName</span></span>|<span data-ttu-id="186ae-196">String</span><span class="sxs-lookup"><span data-stu-id="186ae-196">String</span></span>|<span data-ttu-id="186ae-197">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="186ae-197">Device category display name</span></span>|
|<span data-ttu-id="186ae-198">isSupervised</span><span class="sxs-lookup"><span data-stu-id="186ae-198">isSupervised</span></span>|<span data-ttu-id="186ae-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="186ae-199">Boolean</span></span>|<span data-ttu-id="186ae-200">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="186ae-200">Device supervised status</span></span>|
|<span data-ttu-id="186ae-201">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="186ae-201">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="186ae-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186ae-202">DateTimeOffset</span></span>|<span data-ttu-id="186ae-203">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="186ae-203">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="186ae-204">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="186ae-204">exchangeAccessState</span></span>|<span data-ttu-id="186ae-205">String</span><span class="sxs-lookup"><span data-stu-id="186ae-205">String</span></span>|<span data-ttu-id="186ae-206">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="186ae-206">The Access State of the device in Exchange.</span></span> <span data-ttu-id="186ae-207">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="186ae-207">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="186ae-208">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="186ae-208">exchangeAccessStateReason</span></span>|<span data-ttu-id="186ae-209">String</span><span class="sxs-lookup"><span data-stu-id="186ae-209">String</span></span>|<span data-ttu-id="186ae-210">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="186ae-210">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="186ae-211">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="186ae-211">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="186ae-212">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="186ae-212">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="186ae-213">String</span><span class="sxs-lookup"><span data-stu-id="186ae-213">String</span></span>|<span data-ttu-id="186ae-214">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="186ae-214">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="186ae-215">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="186ae-215">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="186ae-216">String</span><span class="sxs-lookup"><span data-stu-id="186ae-216">String</span></span>|<span data-ttu-id="186ae-217">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="186ae-217">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="186ae-218">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="186ae-218">IsEncrypted</span></span>|<span data-ttu-id="186ae-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="186ae-219">Boolean</span></span>|<span data-ttu-id="186ae-220">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="186ae-220">Device encryption status</span></span>|
|<span data-ttu-id="186ae-221">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="186ae-221">userPrincipalName</span></span>|<span data-ttu-id="186ae-222">String</span><span class="sxs-lookup"><span data-stu-id="186ae-222">String</span></span>|<span data-ttu-id="186ae-223">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="186ae-223">The user principal name.</span></span>|
|<span data-ttu-id="186ae-224">model</span><span class="sxs-lookup"><span data-stu-id="186ae-224">model</span></span>|<span data-ttu-id="186ae-225">String</span><span class="sxs-lookup"><span data-stu-id="186ae-225">String</span></span>|<span data-ttu-id="186ae-226">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="186ae-226">Model of the device</span></span>|
|<span data-ttu-id="186ae-227">manufacturer</span><span class="sxs-lookup"><span data-stu-id="186ae-227">Camera manufacturer.</span></span>|<span data-ttu-id="186ae-228">String</span><span class="sxs-lookup"><span data-stu-id="186ae-228">String</span></span>|<span data-ttu-id="186ae-229">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="186ae-229">Manufacturer of the device</span></span>|
|<span data-ttu-id="186ae-230">imei</span><span class="sxs-lookup"><span data-stu-id="186ae-230">imei</span></span>|<span data-ttu-id="186ae-231">String</span><span class="sxs-lookup"><span data-stu-id="186ae-231">String</span></span>|<span data-ttu-id="186ae-232">IMEI</span><span class="sxs-lookup"><span data-stu-id="186ae-232">IMEI</span></span>|
|<span data-ttu-id="186ae-233">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="186ae-233">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="186ae-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186ae-234">DateTimeOffset</span></span>|<span data-ttu-id="186ae-235">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="186ae-235">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="186ae-236">serialNumber</span><span class="sxs-lookup"><span data-stu-id="186ae-236">serialNumber</span></span>|<span data-ttu-id="186ae-237">String</span><span class="sxs-lookup"><span data-stu-id="186ae-237">String</span></span>|<span data-ttu-id="186ae-238">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="186ae-238">object  . SerialNumber</span></span>|
|<span data-ttu-id="186ae-239">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="186ae-239">PhoneNumber</span></span>|<span data-ttu-id="186ae-240">String</span><span class="sxs-lookup"><span data-stu-id="186ae-240">String</span></span>|<span data-ttu-id="186ae-241">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="186ae-241">Phone number of the device</span></span>|
|<span data-ttu-id="186ae-242">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="186ae-242">androidSecurityPatchLevel</span></span>|<span data-ttu-id="186ae-243">String</span><span class="sxs-lookup"><span data-stu-id="186ae-243">String</span></span>|<span data-ttu-id="186ae-244">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="186ae-244">Android security patch level</span></span>|
|<span data-ttu-id="186ae-245">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="186ae-245">userDisplayName</span></span>|<span data-ttu-id="186ae-246">String</span><span class="sxs-lookup"><span data-stu-id="186ae-246">String</span></span>|<span data-ttu-id="186ae-247">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="186ae-247">user display name</span></span>|
|<span data-ttu-id="186ae-248">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="186ae-248">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="186ae-249">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="186ae-249">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="186ae-250">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="186ae-250">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="186ae-251">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="186ae-251">wiFiMacAddress</span></span>|<span data-ttu-id="186ae-252">String</span><span class="sxs-lookup"><span data-stu-id="186ae-252">String</span></span>|<span data-ttu-id="186ae-253">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="186ae-253">Wi-Fi MAC</span></span>|
|<span data-ttu-id="186ae-254">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="186ae-254">deviceHealthAttestationState</span></span>|[<span data-ttu-id="186ae-255">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="186ae-255">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="186ae-256">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="186ae-256">The device health attestation state.</span></span>|
|<span data-ttu-id="186ae-257">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="186ae-257">subscriberCarrier</span></span>|<span data-ttu-id="186ae-258">String</span><span class="sxs-lookup"><span data-stu-id="186ae-258">String</span></span>|<span data-ttu-id="186ae-259">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="186ae-259">Subscriber Carrier</span></span>|
|<span data-ttu-id="186ae-260">meid</span><span class="sxs-lookup"><span data-stu-id="186ae-260">meid</span></span>|<span data-ttu-id="186ae-261">String</span><span class="sxs-lookup"><span data-stu-id="186ae-261">String</span></span>|<span data-ttu-id="186ae-262">MEID</span><span class="sxs-lookup"><span data-stu-id="186ae-262">MEID</span></span>|
|<span data-ttu-id="186ae-263">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="186ae-263">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="186ae-264">Int64</span><span class="sxs-lookup"><span data-stu-id="186ae-264">Int64</span></span>|<span data-ttu-id="186ae-265">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="186ae-265">Total Storage in Bytes</span></span>|
|<span data-ttu-id="186ae-266">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="186ae-266">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="186ae-267">Int64</span><span class="sxs-lookup"><span data-stu-id="186ae-267">Int64</span></span>|<span data-ttu-id="186ae-268">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="186ae-268">Free Storage in Bytes</span></span>|
|<span data-ttu-id="186ae-269">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="186ae-269">managedDeviceName</span></span>|<span data-ttu-id="186ae-270">String</span><span class="sxs-lookup"><span data-stu-id="186ae-270">String</span></span>|<span data-ttu-id="186ae-271">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="186ae-271">Automatically generated name to identify a device.</span></span> <span data-ttu-id="186ae-272">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="186ae-272">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="186ae-273">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="186ae-273">partnerReportedThreatState</span></span>|<span data-ttu-id="186ae-274">String</span><span class="sxs-lookup"><span data-stu-id="186ae-274">String</span></span>|<span data-ttu-id="186ae-275">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="186ae-275">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="186ae-276">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="186ae-276">Read Only</span></span> <span data-ttu-id="186ae-277">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="186ae-277">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`.</span></span>|



## <a name="response"></a><span data-ttu-id="186ae-278">応答</span><span class="sxs-lookup"><span data-stu-id="186ae-278">Response</span></span>
<span data-ttu-id="186ae-279">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="186ae-279">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="186ae-280">例</span><span class="sxs-lookup"><span data-stu-id="186ae-280">Example</span></span>
### <a name="request"></a><span data-ttu-id="186ae-281">要求</span><span class="sxs-lookup"><span data-stu-id="186ae-281">Request</span></span>
<span data-ttu-id="186ae-282">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="186ae-282">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4564

{
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

### <a name="response"></a><span data-ttu-id="186ae-283">応答</span><span class="sxs-lookup"><span data-stu-id="186ae-283">Response</span></span>
<span data-ttu-id="186ae-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="186ae-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



