# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="7acc6-101">Create androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7acc6-101">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="7acc6-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7acc6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7acc6-103">新しい [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7acc6-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7acc6-104">Prerequisites</span></span>
<span data-ttu-id="7acc6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7acc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7acc6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7acc6-107">Permission type</span></span>|<span data-ttu-id="7acc6-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7acc6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7acc6-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="7acc6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7acc6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7acc6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7acc6-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7acc6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7acc6-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7acc6-112">Not supported.</span></span>|
|<span data-ttu-id="7acc6-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7acc6-113">Application</span></span>|<span data-ttu-id="7acc6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7acc6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7acc6-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7acc6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7acc6-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7acc6-116">Request headers</span></span>
|<span data-ttu-id="7acc6-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7acc6-117">Header</span></span>|<span data-ttu-id="7acc6-118">値</span><span class="sxs-lookup"><span data-stu-id="7acc6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7acc6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7acc6-119">Authorization</span></span>|<span data-ttu-id="7acc6-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7acc6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7acc6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7acc6-121">Accept</span></span>|<span data-ttu-id="7acc6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7acc6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7acc6-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7acc6-123">Request body</span></span>
<span data-ttu-id="7acc6-124">要求本文で、androidGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="7acc6-125">次の表に、androidGeneralDeviceConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7acc6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7acc6-126">Property</span></span>|<span data-ttu-id="7acc6-127">型</span><span class="sxs-lookup"><span data-stu-id="7acc6-127">Type</span></span>|<span data-ttu-id="7acc6-128">説明</span><span class="sxs-lookup"><span data-stu-id="7acc6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7acc6-129">id</span><span class="sxs-lookup"><span data-stu-id="7acc6-129">id</span></span>|<span data-ttu-id="7acc6-130">String</span><span class="sxs-lookup"><span data-stu-id="7acc6-130">String</span></span>|<span data-ttu-id="7acc6-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7acc6-131">Name of the entity.</span></span> <span data-ttu-id="7acc6-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7acc6-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7acc6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7acc6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7acc6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7acc6-134">DateTimeOffset</span></span>|<span data-ttu-id="7acc6-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7acc6-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="7acc6-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7acc6-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7acc6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7acc6-137">createdDateTime</span></span>|<span data-ttu-id="7acc6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7acc6-138">DateTimeOffset</span></span>|<span data-ttu-id="7acc6-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7acc6-139">DateTime the object was created.</span></span> <span data-ttu-id="7acc6-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7acc6-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7acc6-141">description</span><span class="sxs-lookup"><span data-stu-id="7acc6-141">description</span></span>|<span data-ttu-id="7acc6-142">String</span><span class="sxs-lookup"><span data-stu-id="7acc6-142">String</span></span>|<span data-ttu-id="7acc6-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7acc6-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7acc6-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7acc6-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7acc6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7acc6-145">displayName</span></span>|<span data-ttu-id="7acc6-146">String</span><span class="sxs-lookup"><span data-stu-id="7acc6-146">String</span></span>|<span data-ttu-id="7acc6-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7acc6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7acc6-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7acc6-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7acc6-149">version</span><span class="sxs-lookup"><span data-stu-id="7acc6-149">version</span></span>|<span data-ttu-id="7acc6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc6-150">Int32</span></span>|<span data-ttu-id="7acc6-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7acc6-151">Version of the device configuration.</span></span> <span data-ttu-id="7acc6-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7acc6-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7acc6-153">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="7acc6-153">appsBlockClipboardSharing</span></span>|<span data-ttu-id="7acc6-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-154">Boolean</span></span>|<span data-ttu-id="7acc6-155">アプリケーション間でコピー/貼り付けを行うためのクリップボードの共有をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-155">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="7acc6-156">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="7acc6-156">appsBlockCopyPaste</span></span>|<span data-ttu-id="7acc6-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-157">Boolean</span></span>|<span data-ttu-id="7acc6-158">アプリケーション内でのコピー/貼り付けをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-158">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="7acc6-159">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="7acc6-159">appsBlockYouTube</span></span>|<span data-ttu-id="7acc6-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-160">Boolean</span></span>|<span data-ttu-id="7acc6-161">YouTube アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-161">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="7acc6-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-162">bluetoothBlocked</span></span>|<span data-ttu-id="7acc6-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-163">Boolean</span></span>|<span data-ttu-id="7acc6-164">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-164">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="7acc6-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-165">cameraBlocked</span></span>|<span data-ttu-id="7acc6-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-166">Boolean</span></span>|<span data-ttu-id="7acc6-167">カメラの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-167">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="7acc6-168">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="7acc6-168">cellularBlockDataRoaming</span></span>|<span data-ttu-id="7acc6-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-169">Boolean</span></span>|<span data-ttu-id="7acc6-170">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-170">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="7acc6-171">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="7acc6-171">cellularBlockMessaging</span></span>|<span data-ttu-id="7acc6-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-172">Boolean</span></span>|<span data-ttu-id="7acc6-173">SMS/MMS メッセージングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-173">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="7acc6-174">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="7acc6-174">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="7acc6-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-175">Boolean</span></span>|<span data-ttu-id="7acc6-176">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-176">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="7acc6-177">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="7acc6-177">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="7acc6-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-178">Boolean</span></span>|<span data-ttu-id="7acc6-179">Wi-Fi テザリングの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-179">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="7acc6-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="7acc6-180">compliantAppsList</span></span>|<span data-ttu-id="7acc6-181">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7acc6-181">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="7acc6-182">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="7acc6-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="7acc6-183">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7acc6-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7acc6-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="7acc6-184">compliantAppListType</span></span>|<span data-ttu-id="7acc6-185">String</span><span class="sxs-lookup"><span data-stu-id="7acc6-185">String</span></span>|<span data-ttu-id="7acc6-186">CompliantAppsList 内にあるリストの種類。</span><span class="sxs-lookup"><span data-stu-id="7acc6-186">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="7acc6-187">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="7acc6-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="7acc6-188">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="7acc6-188">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="7acc6-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-189">Boolean</span></span>|<span data-ttu-id="7acc6-190">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-190">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="7acc6-191">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-191">locationServicesBlocked</span></span>|<span data-ttu-id="7acc6-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-192">Boolean</span></span>|<span data-ttu-id="7acc6-193">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-193">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="7acc6-194">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="7acc6-194">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="7acc6-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-195">Boolean</span></span>|<span data-ttu-id="7acc6-196">Google アカウントの自動同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-196">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="7acc6-197">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-197">googlePlayStoreBlocked</span></span>|<span data-ttu-id="7acc6-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-198">Boolean</span></span>|<span data-ttu-id="7acc6-199">Google Play ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-199">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="7acc6-200">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="7acc6-200">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="7acc6-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-201">Boolean</span></span>|<span data-ttu-id="7acc6-202">キオスク モード中に画面スリープ ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-202">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="7acc6-203">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="7acc6-203">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="7acc6-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-204">Boolean</span></span>|<span data-ttu-id="7acc6-205">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-205">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="7acc6-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="7acc6-206">kioskModeApps</span></span>|<span data-ttu-id="7acc6-207">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7acc6-207">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="7acc6-208">デバイスがキオスク モードのときに実行できるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="7acc6-208">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="7acc6-209">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7acc6-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7acc6-210">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-210">nfcBlocked</span></span>|<span data-ttu-id="7acc6-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-211">Boolean</span></span>|<span data-ttu-id="7acc6-212">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-212">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="7acc6-213">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="7acc6-213">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="7acc6-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-214">Boolean</span></span>|<span data-ttu-id="7acc6-215">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-215">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="7acc6-216">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="7acc6-216">passwordBlockTrustAgents</span></span>|<span data-ttu-id="7acc6-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-217">Boolean</span></span>|<span data-ttu-id="7acc6-218">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-218">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="7acc6-219">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7acc6-219">passwordExpirationDays</span></span>|<span data-ttu-id="7acc6-220">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc6-220">Int32</span></span>|<span data-ttu-id="7acc6-221">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="7acc6-221">Number of days before the password expires.</span></span> <span data-ttu-id="7acc6-222">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="7acc6-222">Valid values 1 to 365</span></span>|
|<span data-ttu-id="7acc6-223">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7acc6-223">passwordMinimumLength</span></span>|<span data-ttu-id="7acc6-224">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc6-224">Int32</span></span>|<span data-ttu-id="7acc6-225">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="7acc6-225">Minimum length of passwords.</span></span> <span data-ttu-id="7acc6-226">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="7acc6-226">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7acc6-227">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7acc6-227">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7acc6-228">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc6-228">Int32</span></span>|<span data-ttu-id="7acc6-229">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="7acc6-229">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7acc6-230">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7acc6-230">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7acc6-231">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc6-231">Int32</span></span>|<span data-ttu-id="7acc6-232">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="7acc6-232">Number of previous passwords to block.</span></span> <span data-ttu-id="7acc6-233">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="7acc6-233">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7acc6-234">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7acc6-234">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7acc6-235">Int32</span><span class="sxs-lookup"><span data-stu-id="7acc6-235">Int32</span></span>|<span data-ttu-id="7acc6-236">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="7acc6-236">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="7acc6-237">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="7acc6-237">Valid values 4 to 11</span></span>|
|<span data-ttu-id="7acc6-238">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7acc6-238">passwordRequiredType</span></span>|<span data-ttu-id="7acc6-239">String</span><span class="sxs-lookup"><span data-stu-id="7acc6-239">String</span></span>|<span data-ttu-id="7acc6-240">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="7acc6-240">Type of password that is required.</span></span> <span data-ttu-id="7acc6-241">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="7acc6-241">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`.</span></span>|
|<span data-ttu-id="7acc6-242">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7acc6-242">passwordRequired</span></span>|<span data-ttu-id="7acc6-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-243">Boolean</span></span>|<span data-ttu-id="7acc6-244">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-244">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="7acc6-245">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-245">powerOffBlocked</span></span>|<span data-ttu-id="7acc6-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-246">Boolean</span></span>|<span data-ttu-id="7acc6-247">デバイスの電源オフをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-247">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="7acc6-248">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-248">factoryResetBlocked</span></span>|<span data-ttu-id="7acc6-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-249">Boolean</span></span>|<span data-ttu-id="7acc6-250">ユーザーが出荷時の設定にリセットできないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-250">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="7acc6-251">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-251">screenCaptureBlocked</span></span>|<span data-ttu-id="7acc6-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-252">Boolean</span></span>|<span data-ttu-id="7acc6-253">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-253">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="7acc6-254">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="7acc6-254">deviceSharingAllowed</span></span>|<span data-ttu-id="7acc6-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-255">Boolean</span></span>|<span data-ttu-id="7acc6-256">デバイスの共有モードを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-256">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="7acc6-257">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="7acc6-257">storageBlockGoogleBackup</span></span>|<span data-ttu-id="7acc6-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-258">Boolean</span></span>|<span data-ttu-id="7acc6-259">Google バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-259">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="7acc6-260">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="7acc6-260">storageBlockRemovableStorage</span></span>|<span data-ttu-id="7acc6-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-261">Boolean</span></span>|<span data-ttu-id="7acc6-262">リムーバブル記憶域の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-262">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="7acc6-263">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="7acc6-263">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="7acc6-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-264">Boolean</span></span>|<span data-ttu-id="7acc6-265">デバイスの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-265">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="7acc6-266">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="7acc6-266">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="7acc6-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-267">Boolean</span></span>|<span data-ttu-id="7acc6-268">リムーバブル記憶域の暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-268">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="7acc6-269">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-269">voiceAssistantBlocked</span></span>|<span data-ttu-id="7acc6-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-270">Boolean</span></span>|<span data-ttu-id="7acc6-271">音声アシスタントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-271">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="7acc6-272">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-272">voiceDialingBlocked</span></span>|<span data-ttu-id="7acc6-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-273">Boolean</span></span>|<span data-ttu-id="7acc6-274">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-274">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="7acc6-275">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="7acc6-275">webBrowserBlockPopups</span></span>|<span data-ttu-id="7acc6-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-276">Boolean</span></span>|<span data-ttu-id="7acc6-277">Web ブラウザー内のポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-277">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="7acc6-278">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="7acc6-278">webBrowserBlockAutofill</span></span>|<span data-ttu-id="7acc6-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-279">Boolean</span></span>|<span data-ttu-id="7acc6-280">Web ブラウザーの自動塗りつぶし機能をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-280">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="7acc6-281">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="7acc6-281">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="7acc6-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-282">Boolean</span></span>|<span data-ttu-id="7acc6-283">Web ブラウザー内の JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-283">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="7acc6-284">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-284">webBrowserBlocked</span></span>|<span data-ttu-id="7acc6-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-285">Boolean</span></span>|<span data-ttu-id="7acc6-286">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-286">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="7acc6-287">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="7acc6-287">webBrowserCookieSettings</span></span>|<span data-ttu-id="7acc6-288">String</span><span class="sxs-lookup"><span data-stu-id="7acc6-288">String</span></span>|<span data-ttu-id="7acc6-289">Web ブラウザー内の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="7acc6-289">Cookie settings within the web browser.</span></span> <span data-ttu-id="7acc6-290">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="7acc6-290">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="7acc6-291">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="7acc6-291">wiFiBlocked</span></span>|<span data-ttu-id="7acc6-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-292">Boolean</span></span>|<span data-ttu-id="7acc6-293">Wi-Fi の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-293">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="7acc6-294">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="7acc6-294">appsInstallAllowList</span></span>|<span data-ttu-id="7acc6-295">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7acc6-295">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="7acc6-296">KNOX デバイス上にインストールできるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="7acc6-296">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="7acc6-297">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7acc6-297">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7acc6-298">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="7acc6-298">appsLaunchBlockList</span></span>|<span data-ttu-id="7acc6-299">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7acc6-299">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="7acc6-300">KNOX デバイス上での起動がブロックされているアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="7acc6-300">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="7acc6-301">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7acc6-301">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7acc6-302">appsHideList</span><span class="sxs-lookup"><span data-stu-id="7acc6-302">appsHideList</span></span>|<span data-ttu-id="7acc6-303">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7acc6-303">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="7acc6-304">KNOX デバイス上で非表示にするアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="7acc6-304">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="7acc6-305">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7acc6-305">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7acc6-306">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="7acc6-306">securityRequireVerifyApps</span></span>|<span data-ttu-id="7acc6-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="7acc6-307">Boolean</span></span>|<span data-ttu-id="7acc6-308">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-308">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="7acc6-309">応答</span><span class="sxs-lookup"><span data-stu-id="7acc6-309">Response</span></span>
<span data-ttu-id="7acc6-310">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7acc6-310">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7acc6-311">例</span><span class="sxs-lookup"><span data-stu-id="7acc6-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="7acc6-312">要求</span><span class="sxs-lookup"><span data-stu-id="7acc6-312">Request</span></span>
<span data-ttu-id="7acc6-313">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7acc6-313">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3097

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="7acc6-314">応答</span><span class="sxs-lookup"><span data-stu-id="7acc6-314">Response</span></span>
<span data-ttu-id="7acc6-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7acc6-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```



