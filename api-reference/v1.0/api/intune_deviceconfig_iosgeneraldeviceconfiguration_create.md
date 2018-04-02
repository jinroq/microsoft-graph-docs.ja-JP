# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="ac539-101">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac539-101">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="ac539-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac539-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac539-103">新しい [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac539-103">Create a new [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac539-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ac539-104">Prerequisites</span></span>
<span data-ttu-id="ac539-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac539-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac539-107">Permission type</span></span>|<span data-ttu-id="ac539-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac539-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac539-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac539-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ac539-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac539-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac539-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac539-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac539-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac539-112">Not supported.</span></span>|
|<span data-ttu-id="ac539-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac539-113">Application</span></span>|<span data-ttu-id="ac539-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac539-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac539-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac539-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ac539-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac539-116">Request headers</span></span>
|<span data-ttu-id="ac539-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac539-117">Header</span></span>|<span data-ttu-id="ac539-118">値</span><span class="sxs-lookup"><span data-stu-id="ac539-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac539-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac539-119">Authorization</span></span>|<span data-ttu-id="ac539-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ac539-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac539-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ac539-121">Accept</span></span>|<span data-ttu-id="ac539-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ac539-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac539-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac539-123">Request body</span></span>
<span data-ttu-id="ac539-124">要求本文で、iosGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ac539-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="ac539-125">次の表に、iosGeneralDeviceConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-125">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="ac539-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac539-126">Property</span></span>|<span data-ttu-id="ac539-127">型</span><span class="sxs-lookup"><span data-stu-id="ac539-127">Type</span></span>|<span data-ttu-id="ac539-128">説明</span><span class="sxs-lookup"><span data-stu-id="ac539-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac539-129">id</span><span class="sxs-lookup"><span data-stu-id="ac539-129">id</span></span>|<span data-ttu-id="ac539-130">String</span><span class="sxs-lookup"><span data-stu-id="ac539-130">String</span></span>|<span data-ttu-id="ac539-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ac539-131">Key of the entity.</span></span> <span data-ttu-id="ac539-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac539-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac539-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac539-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ac539-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac539-134">DateTimeOffset</span></span>|<span data-ttu-id="ac539-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ac539-135">DateTime the object was last modified.</span></span> <span data-ttu-id="ac539-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac539-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac539-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac539-137">createdDateTime</span></span>|<span data-ttu-id="ac539-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac539-138">DateTimeOffset</span></span>|<span data-ttu-id="ac539-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ac539-139">DateTime the object was created.</span></span> <span data-ttu-id="ac539-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac539-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac539-141">description</span><span class="sxs-lookup"><span data-stu-id="ac539-141">description</span></span>|<span data-ttu-id="ac539-142">String</span><span class="sxs-lookup"><span data-stu-id="ac539-142">String</span></span>|<span data-ttu-id="ac539-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="ac539-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ac539-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac539-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac539-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ac539-145">displayName</span></span>|<span data-ttu-id="ac539-146">String</span><span class="sxs-lookup"><span data-stu-id="ac539-146">String</span></span>|<span data-ttu-id="ac539-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="ac539-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ac539-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac539-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac539-149">version</span><span class="sxs-lookup"><span data-stu-id="ac539-149">version</span></span>|<span data-ttu-id="ac539-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ac539-150">Int32</span></span>|<span data-ttu-id="ac539-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ac539-151">Version of the device configuration.</span></span> <span data-ttu-id="ac539-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac539-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac539-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="ac539-153">accountBlockModification</span></span>|<span data-ttu-id="ac539-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-154">Boolean</span></span>|<span data-ttu-id="ac539-155">デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="ac539-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="ac539-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-157">Boolean</span></span>|<span data-ttu-id="ac539-158">デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="ac539-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-159">airDropBlocked</span></span>|<span data-ttu-id="ac539-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-160">Boolean</span></span>|<span data-ttu-id="ac539-161">デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="ac539-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="ac539-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-163">Boolean</span></span>|<span data-ttu-id="ac539-164">AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ac539-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="ac539-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="ac539-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-166">Boolean</span></span>|<span data-ttu-id="ac539-167">ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="ac539-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="ac539-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="ac539-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-169">Boolean</span></span>|<span data-ttu-id="ac539-170">デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ac539-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="ac539-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="ac539-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-172">Boolean</span></span>|<span data-ttu-id="ac539-173">ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="ac539-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-174">appleNewsBlocked</span></span>|<span data-ttu-id="ac539-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-175">Boolean</span></span>|<span data-ttu-id="ac539-176">デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ac539-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="ac539-177">appsSingleAppModeList</span></span>|<span data-ttu-id="ac539-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ac539-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ac539-179">単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="ac539-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="ac539-180">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="ac539-180">Supervised only.</span></span> <span data-ttu-id="ac539-181">iOS 7.0 以降。</span><span class="sxs-lookup"><span data-stu-id="ac539-181">iOS 7.0 and later.</span></span> <span data-ttu-id="ac539-182">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ac539-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ac539-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="ac539-183">appsVisibilityList</span></span>|<span data-ttu-id="ac539-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ac539-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ac539-185">可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。</span><span class="sxs-lookup"><span data-stu-id="ac539-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="ac539-186">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ac539-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ac539-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="ac539-187">appsVisibilityListType</span></span>|<span data-ttu-id="ac539-188">String</span><span class="sxs-lookup"><span data-stu-id="ac539-188">String</span></span>|<span data-ttu-id="ac539-189">AppsVisibilityList 内にあるリストの種類です。</span><span class="sxs-lookup"><span data-stu-id="ac539-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="ac539-190">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="ac539-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ac539-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="ac539-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="ac539-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-192">Boolean</span></span>|<span data-ttu-id="ac539-193">デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ac539-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-194">appStoreBlocked</span></span>|<span data-ttu-id="ac539-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-195">Boolean</span></span>|<span data-ttu-id="ac539-196">ユーザーによる App Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="ac539-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="ac539-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="ac539-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-198">Boolean</span></span>|<span data-ttu-id="ac539-199">ユーザーによるアプリの購入を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="ac539-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ac539-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="ac539-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-201">Boolean</span></span>|<span data-ttu-id="ac539-202">ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="ac539-203">監視モードのみに適用されます (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ac539-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="ac539-204">appStoreRequirePassword</span></span>|<span data-ttu-id="ac539-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-205">Boolean</span></span>|<span data-ttu-id="ac539-206">App Store 使用時に、パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac539-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="ac539-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="ac539-207">bluetoothBlockModification</span></span>|<span data-ttu-id="ac539-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-208">Boolean</span></span>|<span data-ttu-id="ac539-209">デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="ac539-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-210">cameraBlocked</span></span>|<span data-ttu-id="ac539-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-211">Boolean</span></span>|<span data-ttu-id="ac539-212">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="ac539-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ac539-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ac539-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-214">Boolean</span></span>|<span data-ttu-id="ac539-215">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ac539-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="ac539-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="ac539-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-217">Boolean</span></span>|<span data-ttu-id="ac539-218">ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="ac539-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="ac539-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="ac539-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-220">Boolean</span></span>|<span data-ttu-id="ac539-221">デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="ac539-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="ac539-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-223">Boolean</span></span>|<span data-ttu-id="ac539-224">個人用ホットスポットをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="ac539-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="ac539-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="ac539-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-226">Boolean</span></span>|<span data-ttu-id="ac539-227">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="ac539-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="ac539-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="ac539-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-229">Boolean</span></span>|<span data-ttu-id="ac539-230">信頼されていない TLS の証明書をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="ac539-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ac539-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="ac539-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-232">Boolean</span></span>|<span data-ttu-id="ac539-233">デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ac539-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ac539-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="ac539-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-235">Boolean</span></span>|<span data-ttu-id="ac539-236">デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="ac539-237">compliantAppsList</span></span>|<span data-ttu-id="ac539-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ac539-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ac539-239">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="ac539-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="ac539-240">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ac539-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ac539-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="ac539-241">compliantAppListType</span></span>|<span data-ttu-id="ac539-242">String</span><span class="sxs-lookup"><span data-stu-id="ac539-242">String</span></span>|<span data-ttu-id="ac539-243">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="ac539-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="ac539-244">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="ac539-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ac539-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="ac539-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="ac539-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-246">Boolean</span></span>|<span data-ttu-id="ac539-247">デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-248">definitionLookupBlocked</span></span>|<span data-ttu-id="ac539-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-249">Boolean</span></span>|<span data-ttu-id="ac539-250">デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="ac539-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="ac539-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="ac539-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-252">Boolean</span></span>|<span data-ttu-id="ac539-253">デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="ac539-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="ac539-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-255">Boolean</span></span>|<span data-ttu-id="ac539-256">デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="ac539-257">deviceBlockNameModification</span></span>|<span data-ttu-id="ac539-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-258">Boolean</span></span>|<span data-ttu-id="ac539-259">デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ac539-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="ac539-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="ac539-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-261">Boolean</span></span>|<span data-ttu-id="ac539-262">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ac539-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="ac539-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="ac539-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-264">Boolean</span></span>|<span data-ttu-id="ac539-265">デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="ac539-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="ac539-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="ac539-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-267">Boolean</span></span>|<span data-ttu-id="ac539-268">ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="ac539-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="ac539-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="ac539-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-270">Boolean</span></span>|<span data-ttu-id="ac539-271">ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="ac539-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="ac539-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="ac539-273">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ac539-273">String collection</span></span>|<span data-ttu-id="ac539-274">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="ac539-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="ac539-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="ac539-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="ac539-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-276">Boolean</span></span>|<span data-ttu-id="ac539-277">ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="ac539-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="ac539-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="ac539-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-279">Boolean</span></span>|<span data-ttu-id="ac539-280">ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="ac539-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-281">faceTimeBlocked</span></span>|<span data-ttu-id="ac539-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-282">Boolean</span></span>|<span data-ttu-id="ac539-283">ユーザーによる FaceTime の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="ac539-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="ac539-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-285">Boolean</span></span>|<span data-ttu-id="ac539-286">デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="ac539-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="ac539-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-288">Boolean</span></span>|<span data-ttu-id="ac539-289">ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="ac539-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="ac539-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="ac539-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-291">Boolean</span></span>|<span data-ttu-id="ac539-292">ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="ac539-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-293">gameCenterBlocked</span></span>|<span data-ttu-id="ac539-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-294">Boolean</span></span>|<span data-ttu-id="ac539-295">デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-296">hostPairingBlocked</span></span>|<span data-ttu-id="ac539-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-297">Boolean</span></span>|<span data-ttu-id="ac539-298">iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="ac539-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-300">Boolean</span></span>|<span data-ttu-id="ac539-301">デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="ac539-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="ac539-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-303">Boolean</span></span>|<span data-ttu-id="ac539-304">アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="ac539-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="ac539-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="ac539-306">ブール型</span><span class="sxs-lookup"><span data-stu-id="ac539-306">Boolean</span></span>|<span data-ttu-id="ac539-307">iOS デバイスで起動した作業の、別の iOS デバイスまたは macOS デバイスでの継続実施をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="ac539-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ac539-308">iCloudBlockBackup</span></span>|<span data-ttu-id="ac539-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-309">Boolean</span></span>|<span data-ttu-id="ac539-310">iCloud バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="ac539-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="ac539-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="ac539-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-312">Boolean</span></span>|<span data-ttu-id="ac539-313">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="ac539-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="ac539-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="ac539-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-315">Boolean</span></span>|<span data-ttu-id="ac539-316">管理対象アプリのクラウドの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="ac539-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="ac539-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="ac539-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-318">Boolean</span></span>|<span data-ttu-id="ac539-319">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="ac539-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="ac539-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="ac539-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-321">Boolean</span></span>|<span data-ttu-id="ac539-322">iCloud フォトのストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="ac539-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="ac539-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="ac539-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-324">Boolean</span></span>|<span data-ttu-id="ac539-325">共有フォト ストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="ac539-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="ac539-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="ac539-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-327">Boolean</span></span>|<span data-ttu-id="ac539-328">iCloud のバックアップを暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="ac539-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="ac539-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="ac539-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-330">Boolean</span></span>|<span data-ttu-id="ac539-331">ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac539-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="ac539-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="ac539-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="ac539-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-333">Boolean</span></span>|<span data-ttu-id="ac539-334">デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ac539-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="ac539-335">iTunesBlockRadio</span></span>|<span data-ttu-id="ac539-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-336">Boolean</span></span>|<span data-ttu-id="ac539-337">デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ac539-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="ac539-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="ac539-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-339">Boolean</span></span>|<span data-ttu-id="ac539-340">デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ac539-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="ac539-341">keyboardBlockDictation</span></span>|<span data-ttu-id="ac539-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-342">Boolean</span></span>|<span data-ttu-id="ac539-343">デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ac539-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="ac539-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="ac539-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-345">Boolean</span></span>|<span data-ttu-id="ac539-346">デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ac539-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="ac539-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="ac539-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-348">Boolean</span></span>|<span data-ttu-id="ac539-349">デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ac539-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="ac539-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="ac539-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-351">Boolean</span></span>|<span data-ttu-id="ac539-352">デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ac539-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="ac539-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="ac539-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-354">Boolean</span></span>|<span data-ttu-id="ac539-355">キオスク モード時の補助音声を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="ac539-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="ac539-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-357">Boolean</span></span>|<span data-ttu-id="ac539-358">キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="ac539-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="ac539-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-360">Boolean</span></span>|<span data-ttu-id="ac539-361">キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="ac539-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="ac539-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-363">Boolean</span></span>|<span data-ttu-id="ac539-364">キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ac539-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="ac539-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-366">Boolean</span></span>|<span data-ttu-id="ac539-367">キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ac539-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="ac539-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-369">Boolean</span></span>|<span data-ttu-id="ac539-370">キオスク モード時の画面の回転を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="ac539-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="ac539-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-372">Boolean</span></span>|<span data-ttu-id="ac539-373">キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ac539-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="ac539-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-375">Boolean</span></span>|<span data-ttu-id="ac539-376">キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="ac539-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="ac539-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-378">Boolean</span></span>|<span data-ttu-id="ac539-379">キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ac539-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="ac539-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-381">Boolean</span></span>|<span data-ttu-id="ac539-382">キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="ac539-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="ac539-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-384">Boolean</span></span>|<span data-ttu-id="ac539-385">キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ac539-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="ac539-387">String</span><span class="sxs-lookup"><span data-stu-id="ac539-387">String</span></span>|<span data-ttu-id="ac539-388">キオスク モード用に使用するアプリへの、App Store 内の URL。</span><span class="sxs-lookup"><span data-stu-id="ac539-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="ac539-389">KioskModeManagedAppId が不明な場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="ac539-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="ac539-390">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="ac539-390">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="ac539-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-391">Boolean</span></span>|<span data-ttu-id="ac539-392">キオスク モード時に Assistive Touch が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-392">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-393">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="ac539-393">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="ac539-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-394">Boolean</span></span>|<span data-ttu-id="ac539-395">キオスク モード時に色反転が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-395">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-396">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="ac539-396">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="ac539-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-397">Boolean</span></span>|<span data-ttu-id="ac539-398">キオスク モード時にモノラル オーディオが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-398">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-399">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="ac539-399">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="ac539-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-400">Boolean</span></span>|<span data-ttu-id="ac539-401">キオスク モード時にボイス オーバーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-401">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-402">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="ac539-402">kioskModeRequireZoom</span></span>|<span data-ttu-id="ac539-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-403">Boolean</span></span>|<span data-ttu-id="ac539-404">キオスク モード時にズームが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-404">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="ac539-405">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="ac539-405">kioskModeManagedAppId</span></span>|<span data-ttu-id="ac539-406">String</span><span class="sxs-lookup"><span data-stu-id="ac539-406">String</span></span>|<span data-ttu-id="ac539-407">キオスク モード用に使用するアプリの管理対象アプリ ID。</span><span class="sxs-lookup"><span data-stu-id="ac539-407">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="ac539-408">KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。</span><span class="sxs-lookup"><span data-stu-id="ac539-408">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="ac539-409">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="ac539-409">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="ac539-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-410">Boolean</span></span>|<span data-ttu-id="ac539-411">ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-411">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="ac539-412">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="ac539-412">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="ac539-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-413">Boolean</span></span>|<span data-ttu-id="ac539-414">ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-414">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="ac539-415">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="ac539-415">lockScreenBlockPassbook</span></span>|<span data-ttu-id="ac539-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-416">Boolean</span></span>|<span data-ttu-id="ac539-417">デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-417">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="ac539-418">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="ac539-418">lockScreenBlockTodayView</span></span>|<span data-ttu-id="ac539-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-419">Boolean</span></span>|<span data-ttu-id="ac539-420">ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-420">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="ac539-421">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ac539-421">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="ac539-422">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ac539-422">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="ac539-423">メディア コンテンツの評価の設定 (オーストラリア向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-423">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="ac539-424">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ac539-424">mediaContentRatingCanada</span></span>|[<span data-ttu-id="ac539-425">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ac539-425">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="ac539-426">メディア コンテンツの評価の設定 (カナダ向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-426">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="ac539-427">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ac539-427">mediaContentRatingFrance</span></span>|[<span data-ttu-id="ac539-428">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ac539-428">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="ac539-429">メディア コンテンツの評価の設定 (フランス向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-429">Media content rating settings for France</span></span>|
|<span data-ttu-id="ac539-430">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ac539-430">mediaContentRatingGermany</span></span>|[<span data-ttu-id="ac539-431">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ac539-431">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="ac539-432">メディア コンテンツの評価の設定 (ドイツ向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-432">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="ac539-433">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ac539-433">mediaContentRatingIreland</span></span>|[<span data-ttu-id="ac539-434">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ac539-434">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="ac539-435">メディア コンテンツの評価の設定 (アイルランド向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-435">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="ac539-436">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ac539-436">mediaContentRatingJapan</span></span>|[<span data-ttu-id="ac539-437">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ac539-437">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="ac539-438">メディア コンテンツの評価の設定 (日本向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-438">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="ac539-439">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ac539-439">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="ac539-440">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ac539-440">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="ac539-441">メディア コンテンツの評価の設定 (ニュージーランド向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-441">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="ac539-442">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ac539-442">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="ac539-443">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ac539-443">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="ac539-444">メディア コンテンツの評価の設定 (英国向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-444">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="ac539-445">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ac539-445">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="ac539-446">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ac539-446">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="ac539-447">メディア コンテンツの評価の設定 (米国向け)</span><span class="sxs-lookup"><span data-stu-id="ac539-447">Media content rating settings for United States</span></span>|
|<span data-ttu-id="ac539-448">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="ac539-448">networkUsageRules</span></span>|<span data-ttu-id="ac539-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ac539-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="ac539-450">管理対象アプリと、それらに適用されるネットワーク ルールのリストです。</span><span class="sxs-lookup"><span data-stu-id="ac539-450">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="ac539-451">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ac539-451">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ac539-452">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="ac539-452">mediaContentRatingApps</span></span>|<span data-ttu-id="ac539-453">String</span><span class="sxs-lookup"><span data-stu-id="ac539-453">String</span></span>|<span data-ttu-id="ac539-454">アプリのメディア コンテンツの評価の設定。可能な値は、`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17` です。</span><span class="sxs-lookup"><span data-stu-id="ac539-454">Media content rating settings for Apps Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="ac539-455">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-455">messagesBlocked</span></span>|<span data-ttu-id="ac539-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-456">Boolean</span></span>|<span data-ttu-id="ac539-457">ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-457">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="ac539-458">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="ac539-458">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="ac539-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-459">Boolean</span></span>|<span data-ttu-id="ac539-460">通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-460">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ac539-461">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ac539-461">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="ac539-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-462">Boolean</span></span>|<span data-ttu-id="ac539-463">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-463">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ac539-464">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="ac539-464">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="ac539-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-465">Boolean</span></span>|<span data-ttu-id="ac539-466">監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。</span><span class="sxs-lookup"><span data-stu-id="ac539-466">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="ac539-467">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="ac539-467">passcodeBlockModification</span></span>|<span data-ttu-id="ac539-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-468">Boolean</span></span>|<span data-ttu-id="ac539-469">監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-469">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ac539-470">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ac539-470">passcodeBlockSimple</span></span>|<span data-ttu-id="ac539-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-471">Boolean</span></span>|<span data-ttu-id="ac539-472">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-472">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ac539-473">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ac539-473">passcodeExpirationDays</span></span>|<span data-ttu-id="ac539-474">Int32</span><span class="sxs-lookup"><span data-stu-id="ac539-474">Int32</span></span>|<span data-ttu-id="ac539-475">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="ac539-475">Number of days before the passcode expires.</span></span> <span data-ttu-id="ac539-476">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="ac539-476">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ac539-477">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ac539-477">passcodeMinimumLength</span></span>|<span data-ttu-id="ac539-478">Int32</span><span class="sxs-lookup"><span data-stu-id="ac539-478">Int32</span></span>|<span data-ttu-id="ac539-479">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="ac539-479">Minimum length of passcode.</span></span> <span data-ttu-id="ac539-480">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="ac539-480">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ac539-481">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ac539-481">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ac539-482">Int32</span><span class="sxs-lookup"><span data-stu-id="ac539-482">Int32</span></span>|<span data-ttu-id="ac539-483">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="ac539-483">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ac539-484">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ac539-484">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ac539-485">Int32</span><span class="sxs-lookup"><span data-stu-id="ac539-485">Int32</span></span>|<span data-ttu-id="ac539-486">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="ac539-486">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ac539-487">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ac539-487">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ac539-488">Int32</span><span class="sxs-lookup"><span data-stu-id="ac539-488">Int32</span></span>|<span data-ttu-id="ac539-489">パスコードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="ac539-489">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="ac539-490">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="ac539-490">Valid values 0 to 4</span></span>|
|<span data-ttu-id="ac539-491">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ac539-491">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ac539-492">Int32</span><span class="sxs-lookup"><span data-stu-id="ac539-492">Int32</span></span>|<span data-ttu-id="ac539-493">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="ac539-493">Number of previous passcodes to block.</span></span> <span data-ttu-id="ac539-494">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="ac539-494">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ac539-495">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="ac539-495">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="ac539-496">Int32</span><span class="sxs-lookup"><span data-stu-id="ac539-496">Int32</span></span>|<span data-ttu-id="ac539-497">デバイスをワイプするまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="ac539-497">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="ac539-498">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="ac539-498">Valid values 4 to 11</span></span>|
|<span data-ttu-id="ac539-499">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ac539-499">passcodeRequiredType</span></span>|<span data-ttu-id="ac539-500">String</span><span class="sxs-lookup"><span data-stu-id="ac539-500">String</span></span>|<span data-ttu-id="ac539-501">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="ac539-501">Type of passcode that is required.</span></span> <span data-ttu-id="ac539-502">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="ac539-502">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ac539-503">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ac539-503">passcodeRequired</span></span>|<span data-ttu-id="ac539-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-504">Boolean</span></span>|<span data-ttu-id="ac539-505">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac539-505">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ac539-506">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-506">podcastsBlocked</span></span>|<span data-ttu-id="ac539-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-507">Boolean</span></span>|<span data-ttu-id="ac539-508">ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-508">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="ac539-509">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ac539-509">safariBlockAutofill</span></span>|<span data-ttu-id="ac539-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-510">Boolean</span></span>|<span data-ttu-id="ac539-511">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-511">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="ac539-512">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ac539-512">safariBlockJavaScript</span></span>|<span data-ttu-id="ac539-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-513">Boolean</span></span>|<span data-ttu-id="ac539-514">Safari 内で JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-514">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="ac539-515">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ac539-515">safariBlockPopups</span></span>|<span data-ttu-id="ac539-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-516">Boolean</span></span>|<span data-ttu-id="ac539-517">Safari 内でポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-517">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="ac539-518">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-518">safariBlocked</span></span>|<span data-ttu-id="ac539-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-519">Boolean</span></span>|<span data-ttu-id="ac539-520">ユーザーによる Safari の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-520">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="ac539-521">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ac539-521">safariCookieSettings</span></span>|<span data-ttu-id="ac539-522">String</span><span class="sxs-lookup"><span data-stu-id="ac539-522">String</span></span>|<span data-ttu-id="ac539-523">Safari の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="ac539-523">Cookie settings for Safari.</span></span> <span data-ttu-id="ac539-524">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="ac539-524">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="ac539-525">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="ac539-525">safariManagedDomains</span></span>|<span data-ttu-id="ac539-526">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ac539-526">String collection</span></span>|<span data-ttu-id="ac539-527">ここに記載されているパターンに一致する URL は管理対象と見なされます。</span><span class="sxs-lookup"><span data-stu-id="ac539-527">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="ac539-528">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="ac539-528">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="ac539-529">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ac539-529">String collection</span></span>|<span data-ttu-id="ac539-530">ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。</span><span class="sxs-lookup"><span data-stu-id="ac539-530">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="ac539-531">監視モードのデバイスに適用されます (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-531">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ac539-532">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ac539-532">safariRequireFraudWarning</span></span>|<span data-ttu-id="ac539-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-533">Boolean</span></span>|<span data-ttu-id="ac539-534">Safari での不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-534">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="ac539-535">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-535">screenCaptureBlocked</span></span>|<span data-ttu-id="ac539-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-536">Boolean</span></span>|<span data-ttu-id="ac539-537">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-537">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ac539-538">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-538">siriBlocked</span></span>|<span data-ttu-id="ac539-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-539">Boolean</span></span>|<span data-ttu-id="ac539-540">ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-540">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="ac539-541">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="ac539-541">siriBlockedWhenLocked</span></span>|<span data-ttu-id="ac539-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-542">Boolean</span></span>|<span data-ttu-id="ac539-543">ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-543">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="ac539-544">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="ac539-544">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="ac539-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-545">Boolean</span></span>|<span data-ttu-id="ac539-546">監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-546">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="ac539-547">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="ac539-547">siriRequireProfanityFilter</span></span>|<span data-ttu-id="ac539-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-548">Boolean</span></span>|<span data-ttu-id="ac539-549">Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-549">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="ac539-550">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="ac539-550">spotlightBlockInternetResults</span></span>|<span data-ttu-id="ac539-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-551">Boolean</span></span>|<span data-ttu-id="ac539-552">監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-552">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="ac539-553">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="ac539-553">voiceDialingBlocked</span></span>|<span data-ttu-id="ac539-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-554">Boolean</span></span>|<span data-ttu-id="ac539-555">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-555">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="ac539-556">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="ac539-556">wallpaperBlockModification</span></span>|<span data-ttu-id="ac539-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-557">Boolean</span></span>|<span data-ttu-id="ac539-558">監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="ac539-558">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="ac539-559">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="ac539-559">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="ac539-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac539-560">Boolean</span></span>|<span data-ttu-id="ac539-561">デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac539-561">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="ac539-562">応答</span><span class="sxs-lookup"><span data-stu-id="ac539-562">Response</span></span>
<span data-ttu-id="ac539-563">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ac539-563">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac539-564">例</span><span class="sxs-lookup"><span data-stu-id="ac539-564">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac539-565">要求</span><span class="sxs-lookup"><span data-stu-id="ac539-565">Request</span></span>
<span data-ttu-id="ac539-566">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac539-566">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="ac539-567">応答</span><span class="sxs-lookup"><span data-stu-id="ac539-567">Response</span></span>
<span data-ttu-id="ac539-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac539-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7949

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```



