# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="22896-101">iosGeneralDeviceConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="22896-101">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="22896-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="22896-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22896-103">新しい [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="22896-103">Create a new [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22896-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="22896-104">Prerequisites</span></span>
<span data-ttu-id="22896-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22896-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="22896-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22896-107">Permission type</span></span>|<span data-ttu-id="22896-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22896-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22896-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22896-109">Delegated (work or school account)</span></span>|<span data-ttu-id="22896-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22896-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22896-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22896-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22896-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22896-112">Not supported.</span></span>|
|<span data-ttu-id="22896-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22896-113">Application</span></span>|<span data-ttu-id="22896-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22896-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22896-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22896-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22896-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22896-116">Request headers</span></span>
|<span data-ttu-id="22896-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22896-117">Header</span></span>|<span data-ttu-id="22896-118">値</span><span class="sxs-lookup"><span data-stu-id="22896-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22896-119">承認</span><span class="sxs-lookup"><span data-stu-id="22896-119">Authorization</span></span>|<span data-ttu-id="22896-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="22896-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22896-121">承諾</span><span class="sxs-lookup"><span data-stu-id="22896-121">Accept</span></span>|<span data-ttu-id="22896-122">アプリケーション / json</span><span class="sxs-lookup"><span data-stu-id="22896-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22896-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="22896-123">Request body</span></span>
<span data-ttu-id="22896-124">要求本文で、iosGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22896-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="22896-125">次の表に、iosGeneralDeviceConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-125">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="22896-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22896-126">Property</span></span>|<span data-ttu-id="22896-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="22896-127">Type</span></span>|<span data-ttu-id="22896-128">説明</span><span class="sxs-lookup"><span data-stu-id="22896-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22896-129">ID</span><span class="sxs-lookup"><span data-stu-id="22896-129">id</span></span>|<span data-ttu-id="22896-130">文字列</span><span class="sxs-lookup"><span data-stu-id="22896-130">String</span></span>|<span data-ttu-id="22896-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="22896-131">Key of the entity.</span></span> <span data-ttu-id="22896-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22896-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22896-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22896-133">lastModifiedDateTime</span></span>|<span data-ttu-id="22896-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22896-134">DateTimeOffset</span></span>|<span data-ttu-id="22896-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="22896-135">DateTime the object was last modified.</span></span> <span data-ttu-id="22896-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22896-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22896-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22896-137">createdDateTime</span></span>|<span data-ttu-id="22896-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22896-138">DateTimeOffset</span></span>|<span data-ttu-id="22896-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="22896-139">DateTime the object was created.</span></span> <span data-ttu-id="22896-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22896-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22896-141">説明</span><span class="sxs-lookup"><span data-stu-id="22896-141">description</span></span>|<span data-ttu-id="22896-142">文字列</span><span class="sxs-lookup"><span data-stu-id="22896-142">String</span></span>|<span data-ttu-id="22896-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="22896-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22896-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22896-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22896-145">displayName</span><span class="sxs-lookup"><span data-stu-id="22896-145">displayName</span></span>|<span data-ttu-id="22896-146">文字列</span><span class="sxs-lookup"><span data-stu-id="22896-146">String</span></span>|<span data-ttu-id="22896-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="22896-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22896-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22896-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22896-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="22896-149">version</span></span>|<span data-ttu-id="22896-150">Int32</span><span class="sxs-lookup"><span data-stu-id="22896-150">Int32</span></span>|<span data-ttu-id="22896-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="22896-151">Version of the device configuration.</span></span> <span data-ttu-id="22896-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22896-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22896-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="22896-153">accountBlockModification</span></span>|<span data-ttu-id="22896-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-154">Boolean</span></span>|<span data-ttu-id="22896-155">デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="22896-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="22896-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-157">Boolean</span></span>|<span data-ttu-id="22896-158">デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="22896-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-159">airDropBlocked</span></span>|<span data-ttu-id="22896-160">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-160">Boolean</span></span>|<span data-ttu-id="22896-161">デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="22896-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="22896-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-163">Boolean</span></span>|<span data-ttu-id="22896-164">AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="22896-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="22896-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="22896-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-166">Boolean</span></span>|<span data-ttu-id="22896-167">ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="22896-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="22896-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="22896-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-169">Boolean</span></span>|<span data-ttu-id="22896-170">デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="22896-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="22896-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="22896-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-172">Boolean</span></span>|<span data-ttu-id="22896-173">ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="22896-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-174">appleNewsBlocked</span></span>|<span data-ttu-id="22896-175">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-175">Boolean</span></span>|<span data-ttu-id="22896-176">デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="22896-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="22896-177">appsSingleAppModeList</span></span>|<span data-ttu-id="22896-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22896-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="22896-179">単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="22896-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="22896-180">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="22896-180">Supervised only.</span></span> <span data-ttu-id="22896-181">iOS 7.0 以降。</span><span class="sxs-lookup"><span data-stu-id="22896-181">iOS 7.0 and later.</span></span> <span data-ttu-id="22896-182">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="22896-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="22896-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="22896-183">appsVisibilityList</span></span>|<span data-ttu-id="22896-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22896-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="22896-185">可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。</span><span class="sxs-lookup"><span data-stu-id="22896-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="22896-186">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="22896-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="22896-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="22896-187">appsVisibilityListType</span></span>|[<span data-ttu-id="22896-188">appListType</span><span class="sxs-lookup"><span data-stu-id="22896-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="22896-189">AppsVisibilityList 内にあるリストの種類です。</span><span class="sxs-lookup"><span data-stu-id="22896-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="22896-190">指定できる値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="22896-190">The possible values are `none`, `appsInListCompliant`, or `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="22896-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="22896-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="22896-192">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-192">Boolean</span></span>|<span data-ttu-id="22896-193">デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="22896-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-194">appStoreBlocked</span></span>|<span data-ttu-id="22896-195">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-195">Boolean</span></span>|<span data-ttu-id="22896-196">ユーザーによる App Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="22896-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="22896-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="22896-198">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-198">Boolean</span></span>|<span data-ttu-id="22896-199">ユーザーによるアプリの購入を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="22896-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="22896-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="22896-201">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-201">Boolean</span></span>|<span data-ttu-id="22896-202">ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="22896-203">監視モードのみに適用されます (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="22896-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="22896-204">appStoreRequirePassword</span></span>|<span data-ttu-id="22896-205">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-205">Boolean</span></span>|<span data-ttu-id="22896-206">App Store 使用時に、パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="22896-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="22896-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="22896-207">bluetoothBlockModification</span></span>|<span data-ttu-id="22896-208">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-208">Boolean</span></span>|<span data-ttu-id="22896-209">デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="22896-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-210">cameraBlocked</span></span>|<span data-ttu-id="22896-211">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-211">Boolean</span></span>|<span data-ttu-id="22896-212">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="22896-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="22896-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="22896-214">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-214">Boolean</span></span>|<span data-ttu-id="22896-215">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="22896-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="22896-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="22896-217">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-217">Boolean</span></span>|<span data-ttu-id="22896-218">ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="22896-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="22896-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="22896-220">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-220">Boolean</span></span>|<span data-ttu-id="22896-221">デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="22896-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="22896-223">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-223">Boolean</span></span>|<span data-ttu-id="22896-224">個人用ホットスポットをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="22896-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="22896-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="22896-226">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-226">Boolean</span></span>|<span data-ttu-id="22896-227">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="22896-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="22896-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="22896-229">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-229">Boolean</span></span>|<span data-ttu-id="22896-230">信頼されていない TLS の証明書をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="22896-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="22896-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="22896-232">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-232">Boolean</span></span>|<span data-ttu-id="22896-233">デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="22896-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="22896-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="22896-235">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-235">Boolean</span></span>|<span data-ttu-id="22896-236">デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="22896-237">compliantAppsList</span></span>|<span data-ttu-id="22896-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22896-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="22896-239">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="22896-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="22896-240">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="22896-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="22896-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="22896-241">compliantAppListType</span></span>|[<span data-ttu-id="22896-242">appListType</span><span class="sxs-lookup"><span data-stu-id="22896-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="22896-243">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="22896-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="22896-244">指定できる値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="22896-244">The possible values are `none`, `appsInListCompliant`, or `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="22896-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="22896-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="22896-246">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-246">Boolean</span></span>|<span data-ttu-id="22896-247">デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-248">definitionLookupBlocked</span></span>|<span data-ttu-id="22896-249">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-249">Boolean</span></span>|<span data-ttu-id="22896-250">デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="22896-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="22896-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="22896-252">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-252">Boolean</span></span>|<span data-ttu-id="22896-253">デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="22896-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="22896-255">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-255">Boolean</span></span>|<span data-ttu-id="22896-256">デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="22896-257">deviceBlockNameModification</span></span>|<span data-ttu-id="22896-258">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-258">Boolean</span></span>|<span data-ttu-id="22896-259">デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="22896-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="22896-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="22896-261">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-261">Boolean</span></span>|<span data-ttu-id="22896-262">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="22896-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="22896-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="22896-264">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-264">Boolean</span></span>|<span data-ttu-id="22896-265">デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="22896-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="22896-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="22896-267">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-267">Boolean</span></span>|<span data-ttu-id="22896-268">ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="22896-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="22896-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="22896-270">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-270">Boolean</span></span>|<span data-ttu-id="22896-271">ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="22896-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="22896-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="22896-273">String コレクション</span><span class="sxs-lookup"><span data-stu-id="22896-273">String collection</span></span>|<span data-ttu-id="22896-274">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="22896-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="22896-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="22896-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="22896-276">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-276">Boolean</span></span>|<span data-ttu-id="22896-277">ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="22896-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="22896-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="22896-279">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-279">Boolean</span></span>|<span data-ttu-id="22896-280">ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="22896-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-281">faceTimeBlocked</span></span>|<span data-ttu-id="22896-282">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-282">Boolean</span></span>|<span data-ttu-id="22896-283">ユーザーによる FaceTime の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="22896-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="22896-285">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-285">Boolean</span></span>|<span data-ttu-id="22896-286">デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="22896-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="22896-288">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-288">Boolean</span></span>|<span data-ttu-id="22896-289">ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="22896-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="22896-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="22896-291">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-291">Boolean</span></span>|<span data-ttu-id="22896-292">ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="22896-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-293">gameCenterBlocked</span></span>|<span data-ttu-id="22896-294">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-294">Boolean</span></span>|<span data-ttu-id="22896-295">デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-296">hostPairingBlocked</span></span>|<span data-ttu-id="22896-297">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-297">Boolean</span></span>|<span data-ttu-id="22896-298">iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="22896-300">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-300">Boolean</span></span>|<span data-ttu-id="22896-301">デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="22896-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="22896-303">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-303">Boolean</span></span>|<span data-ttu-id="22896-304">アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="22896-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="22896-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="22896-306">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-306">Boolean</span></span>|<span data-ttu-id="22896-307">iOS デバイスで起動した作業の、別の iOS デバイスまたは macOS デバイスでの継続実施をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="22896-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="22896-308">iCloudBlockBackup</span></span>|<span data-ttu-id="22896-309">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-309">Boolean</span></span>|<span data-ttu-id="22896-310">iCloud バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="22896-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="22896-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="22896-312">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-312">Boolean</span></span>|<span data-ttu-id="22896-313">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="22896-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="22896-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="22896-315">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-315">Boolean</span></span>|<span data-ttu-id="22896-316">管理対象アプリのクラウドの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="22896-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="22896-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="22896-318">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-318">Boolean</span></span>|<span data-ttu-id="22896-319">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="22896-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="22896-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="22896-321">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-321">Boolean</span></span>|<span data-ttu-id="22896-322">iCloud フォトのストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="22896-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="22896-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="22896-324">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-324">Boolean</span></span>|<span data-ttu-id="22896-325">共有フォト ストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="22896-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="22896-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="22896-327">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-327">Boolean</span></span>|<span data-ttu-id="22896-328">iCloud のバックアップを暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="22896-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="22896-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="22896-330">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-330">Boolean</span></span>|<span data-ttu-id="22896-331">ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="22896-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="22896-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="22896-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="22896-333">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-333">Boolean</span></span>|<span data-ttu-id="22896-334">デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="22896-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="22896-335">iTunesBlockRadio</span></span>|<span data-ttu-id="22896-336">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-336">Boolean</span></span>|<span data-ttu-id="22896-337">デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="22896-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="22896-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="22896-339">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-339">Boolean</span></span>|<span data-ttu-id="22896-340">デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="22896-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="22896-341">keyboardBlockDictation</span></span>|<span data-ttu-id="22896-342">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-342">Boolean</span></span>|<span data-ttu-id="22896-343">デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="22896-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="22896-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="22896-345">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-345">Boolean</span></span>|<span data-ttu-id="22896-346">デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="22896-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="22896-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="22896-348">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-348">Boolean</span></span>|<span data-ttu-id="22896-349">デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="22896-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="22896-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="22896-351">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-351">Boolean</span></span>|<span data-ttu-id="22896-352">デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="22896-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="22896-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="22896-354">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-354">Boolean</span></span>|<span data-ttu-id="22896-355">キオスク モード時の補助音声を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="22896-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="22896-357">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-357">Boolean</span></span>|<span data-ttu-id="22896-358">キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="22896-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="22896-360">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-360">Boolean</span></span>|<span data-ttu-id="22896-361">キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="22896-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="22896-363">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-363">Boolean</span></span>|<span data-ttu-id="22896-364">キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="22896-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="22896-366">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-366">Boolean</span></span>|<span data-ttu-id="22896-367">キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="22896-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="22896-369">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-369">Boolean</span></span>|<span data-ttu-id="22896-370">キオスク モード時の画面の回転を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="22896-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="22896-372">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-372">Boolean</span></span>|<span data-ttu-id="22896-373">キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="22896-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="22896-375">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-375">Boolean</span></span>|<span data-ttu-id="22896-376">キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="22896-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="22896-378">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-378">Boolean</span></span>|<span data-ttu-id="22896-379">キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="22896-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="22896-381">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-381">Boolean</span></span>|<span data-ttu-id="22896-382">キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="22896-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="22896-384">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-384">Boolean</span></span>|<span data-ttu-id="22896-385">キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="22896-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="22896-387">文字列</span><span class="sxs-lookup"><span data-stu-id="22896-387">String</span></span>|<span data-ttu-id="22896-388">キオスク モード用に使用するアプリへの、App Store 内の URL。</span><span class="sxs-lookup"><span data-stu-id="22896-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="22896-389">KioskModeManagedAppId が不明な場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="22896-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="22896-390">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="22896-390">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="22896-391">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-391">Boolean</span></span>|<span data-ttu-id="22896-392">キオスク モード時に Assistive Touch が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-392">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-393">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="22896-393">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="22896-394">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-394">Boolean</span></span>|<span data-ttu-id="22896-395">キオスク モード時に色反転が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-395">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-396">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="22896-396">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="22896-397">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-397">Boolean</span></span>|<span data-ttu-id="22896-398">キオスク モード時にモノラル オーディオが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-398">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-399">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="22896-399">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="22896-400">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-400">Boolean</span></span>|<span data-ttu-id="22896-401">キオスク モード時にボイス オーバーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-401">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-402">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="22896-402">kioskModeRequireZoom</span></span>|<span data-ttu-id="22896-403">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-403">Boolean</span></span>|<span data-ttu-id="22896-404">キオスク モード時にズームが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-404">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="22896-405">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="22896-405">kioskModeManagedAppId</span></span>|<span data-ttu-id="22896-406">文字列</span><span class="sxs-lookup"><span data-stu-id="22896-406">String</span></span>|<span data-ttu-id="22896-407">キオスク モード用に使用するアプリの管理対象アプリ ID。</span><span class="sxs-lookup"><span data-stu-id="22896-407">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="22896-408">KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。</span><span class="sxs-lookup"><span data-stu-id="22896-408">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="22896-409">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="22896-409">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="22896-410">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-410">Boolean</span></span>|<span data-ttu-id="22896-411">ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-411">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="22896-412">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="22896-412">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="22896-413">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-413">Boolean</span></span>|<span data-ttu-id="22896-414">ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-414">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="22896-415">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="22896-415">lockScreenBlockPassbook</span></span>|<span data-ttu-id="22896-416">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-416">Boolean</span></span>|<span data-ttu-id="22896-417">デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-417">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="22896-418">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="22896-418">lockScreenBlockTodayView</span></span>|<span data-ttu-id="22896-419">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-419">Boolean</span></span>|<span data-ttu-id="22896-420">ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-420">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="22896-421">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="22896-421">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="22896-422">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="22896-422">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="22896-423">メディア コンテンツの評価の設定 (オーストラリア向け)</span><span class="sxs-lookup"><span data-stu-id="22896-423">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="22896-424">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="22896-424">mediaContentRatingCanada</span></span>|[<span data-ttu-id="22896-425">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="22896-425">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="22896-426">メディア コンテンツの評価の設定 (カナダ向け)</span><span class="sxs-lookup"><span data-stu-id="22896-426">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="22896-427">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="22896-427">mediaContentRatingFrance</span></span>|[<span data-ttu-id="22896-428">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="22896-428">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="22896-429">メディア コンテンツの評価の設定 (フランス向け)</span><span class="sxs-lookup"><span data-stu-id="22896-429">Media content rating settings for France</span></span>|
|<span data-ttu-id="22896-430">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="22896-430">mediaContentRatingGermany</span></span>|[<span data-ttu-id="22896-431">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="22896-431">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="22896-432">メディア コンテンツの評価の設定 (ドイツ向け)</span><span class="sxs-lookup"><span data-stu-id="22896-432">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="22896-433">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="22896-433">mediaContentRatingIreland</span></span>|[<span data-ttu-id="22896-434">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="22896-434">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="22896-435">メディア コンテンツの評価の設定 (アイルランド向け)</span><span class="sxs-lookup"><span data-stu-id="22896-435">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="22896-436">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="22896-436">mediaContentRatingJapan</span></span>|[<span data-ttu-id="22896-437">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="22896-437">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="22896-438">メディア コンテンツの評価の設定 (日本向け)</span><span class="sxs-lookup"><span data-stu-id="22896-438">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="22896-439">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="22896-439">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="22896-440">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="22896-440">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="22896-441">メディア コンテンツの評価の設定 (ニュージーランド向け)</span><span class="sxs-lookup"><span data-stu-id="22896-441">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="22896-442">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="22896-442">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="22896-443">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="22896-443">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="22896-444">メディア コンテンツの評価の設定 (英国向け)</span><span class="sxs-lookup"><span data-stu-id="22896-444">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="22896-445">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="22896-445">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="22896-446">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="22896-446">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="22896-447">メディア コンテンツの評価の設定 (米国向け)</span><span class="sxs-lookup"><span data-stu-id="22896-447">Media content rating settings for United States</span></span>|
|<span data-ttu-id="22896-448">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="22896-448">networkUsageRules</span></span>|<span data-ttu-id="22896-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22896-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="22896-450">管理対象アプリと、それらに適用されるネットワーク ルールのリストです。</span><span class="sxs-lookup"><span data-stu-id="22896-450">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="22896-451">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="22896-451">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="22896-452">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="22896-452">mediaContentRatingApps</span></span>|[<span data-ttu-id="22896-453">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="22896-453">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="22896-454">メディア コンテンツのアプリケーションの設定を評価します。</span><span class="sxs-lookup"><span data-stu-id="22896-454">Media content rating settings for Germany</span></span> <span data-ttu-id="22896-455">指定できる値は、`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17` です。</span><span class="sxs-lookup"><span data-stu-id="22896-455">The possible values are `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`, , , , , , or .</span></span>|
|<span data-ttu-id="22896-456">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-456">messagesBlocked</span></span>|<span data-ttu-id="22896-457">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-457">Boolean</span></span>|<span data-ttu-id="22896-458">ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-458">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="22896-459">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="22896-459">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="22896-460">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-460">Boolean</span></span>|<span data-ttu-id="22896-461">通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-461">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="22896-462">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="22896-462">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="22896-463">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-463">Boolean</span></span>|<span data-ttu-id="22896-464">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-464">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="22896-465">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="22896-465">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="22896-466">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-466">Boolean</span></span>|<span data-ttu-id="22896-467">監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。</span><span class="sxs-lookup"><span data-stu-id="22896-467">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="22896-468">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="22896-468">passcodeBlockModification</span></span>|<span data-ttu-id="22896-469">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-469">Boolean</span></span>|<span data-ttu-id="22896-470">監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-470">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="22896-471">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="22896-471">passcodeBlockSimple</span></span>|<span data-ttu-id="22896-472">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-472">Boolean</span></span>|<span data-ttu-id="22896-473">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-473">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="22896-474">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="22896-474">passcodeExpirationDays</span></span>|<span data-ttu-id="22896-475">Int32</span><span class="sxs-lookup"><span data-stu-id="22896-475">Int32</span></span>|<span data-ttu-id="22896-476">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="22896-476">Number of days before the passcode expires.</span></span> <span data-ttu-id="22896-477">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="22896-477">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="22896-478">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="22896-478">passcodeMinimumLength</span></span>|<span data-ttu-id="22896-479">Int32</span><span class="sxs-lookup"><span data-stu-id="22896-479">Int32</span></span>|<span data-ttu-id="22896-480">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="22896-480">Minimum length of passcode.</span></span> <span data-ttu-id="22896-481">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="22896-481">Valid values 4 to 14</span></span>|
|<span data-ttu-id="22896-482">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="22896-482">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="22896-483">Int32</span><span class="sxs-lookup"><span data-stu-id="22896-483">Int32</span></span>|<span data-ttu-id="22896-484">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="22896-484">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="22896-485">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="22896-485">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="22896-486">Int32</span><span class="sxs-lookup"><span data-stu-id="22896-486">Int32</span></span>|<span data-ttu-id="22896-487">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="22896-487">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="22896-488">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="22896-488">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="22896-489">Int32</span><span class="sxs-lookup"><span data-stu-id="22896-489">Int32</span></span>|<span data-ttu-id="22896-490">パスコードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="22896-490">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="22896-491">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="22896-491">Valid values 0 to 4</span></span>|
|<span data-ttu-id="22896-492">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="22896-492">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="22896-493">Int32</span><span class="sxs-lookup"><span data-stu-id="22896-493">Int32</span></span>|<span data-ttu-id="22896-494">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="22896-494">Number of previous passcodes to block.</span></span> <span data-ttu-id="22896-495">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="22896-495">Valid values 1 to 24</span></span>|
|<span data-ttu-id="22896-496">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="22896-496">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="22896-497">Int32</span><span class="sxs-lookup"><span data-stu-id="22896-497">Int32</span></span>|<span data-ttu-id="22896-498">デバイスをワイプするまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="22896-498">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="22896-499">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="22896-499">Valid values 4 to 11</span></span>|
|<span data-ttu-id="22896-500">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="22896-500">passcodeRequiredType</span></span>|[<span data-ttu-id="22896-501">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="22896-501">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="22896-502">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="22896-502">Type of passcode that is required.</span></span> <span data-ttu-id="22896-503">指定できる値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="22896-503">The possible values are `deviceDefault`, `alphanumeric`, or `numeric`.</span></span>|
|<span data-ttu-id="22896-504">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="22896-504">passcodeRequired</span></span>|<span data-ttu-id="22896-505">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-505">Boolean</span></span>|<span data-ttu-id="22896-506">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="22896-506">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="22896-507">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-507">podcastsBlocked</span></span>|<span data-ttu-id="22896-508">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-508">Boolean</span></span>|<span data-ttu-id="22896-509">ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-509">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="22896-510">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="22896-510">safariBlockAutofill</span></span>|<span data-ttu-id="22896-511">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-511">Boolean</span></span>|<span data-ttu-id="22896-512">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-512">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="22896-513">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="22896-513">safariBlockJavaScript</span></span>|<span data-ttu-id="22896-514">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-514">Boolean</span></span>|<span data-ttu-id="22896-515">Safari 内で JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-515">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="22896-516">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="22896-516">safariBlockPopups</span></span>|<span data-ttu-id="22896-517">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-517">Boolean</span></span>|<span data-ttu-id="22896-518">Safari 内でポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-518">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="22896-519">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-519">safariBlocked</span></span>|<span data-ttu-id="22896-520">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-520">Boolean</span></span>|<span data-ttu-id="22896-521">ユーザーによる Safari の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-521">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="22896-522">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="22896-522">safariCookieSettings</span></span>|[<span data-ttu-id="22896-523">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="22896-523">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="22896-524">Safari の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="22896-524">Cookie settings for Safari.</span></span> <span data-ttu-id="22896-525">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="22896-525">The possible values are `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`, , , , , , , or .</span></span>|
|<span data-ttu-id="22896-526">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="22896-526">safariManagedDomains</span></span>|<span data-ttu-id="22896-527">String コレクション</span><span class="sxs-lookup"><span data-stu-id="22896-527">String collection</span></span>|<span data-ttu-id="22896-528">ここに記載されているパターンに一致する URL は管理対象と見なされます。</span><span class="sxs-lookup"><span data-stu-id="22896-528">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="22896-529">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="22896-529">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="22896-530">String コレクション</span><span class="sxs-lookup"><span data-stu-id="22896-530">String collection</span></span>|<span data-ttu-id="22896-531">ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。</span><span class="sxs-lookup"><span data-stu-id="22896-531">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="22896-532">監視モードのデバイスに適用されます (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-532">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="22896-533">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="22896-533">safariRequireFraudWarning</span></span>|<span data-ttu-id="22896-534">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-534">Boolean</span></span>|<span data-ttu-id="22896-535">Safari での不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-535">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="22896-536">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-536">screenCaptureBlocked</span></span>|<span data-ttu-id="22896-537">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-537">Boolean</span></span>|<span data-ttu-id="22896-538">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-538">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="22896-539">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-539">siriBlocked</span></span>|<span data-ttu-id="22896-540">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-540">Boolean</span></span>|<span data-ttu-id="22896-541">ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-541">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="22896-542">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="22896-542">siriBlockedWhenLocked</span></span>|<span data-ttu-id="22896-543">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-543">Boolean</span></span>|<span data-ttu-id="22896-544">ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-544">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="22896-545">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="22896-545">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="22896-546">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-546">Boolean</span></span>|<span data-ttu-id="22896-547">監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-547">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="22896-548">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="22896-548">siriRequireProfanityFilter</span></span>|<span data-ttu-id="22896-549">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-549">Boolean</span></span>|<span data-ttu-id="22896-550">Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-550">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="22896-551">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="22896-551">spotlightBlockInternetResults</span></span>|<span data-ttu-id="22896-552">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-552">Boolean</span></span>|<span data-ttu-id="22896-553">監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-553">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="22896-554">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="22896-554">voiceDialingBlocked</span></span>|<span data-ttu-id="22896-555">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-555">Boolean</span></span>|<span data-ttu-id="22896-556">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-556">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="22896-557">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="22896-557">wallpaperBlockModification</span></span>|<span data-ttu-id="22896-558">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-558">Boolean</span></span>|<span data-ttu-id="22896-559">監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="22896-559">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="22896-560">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="22896-560">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="22896-561">ブール値</span><span class="sxs-lookup"><span data-stu-id="22896-561">Boolean</span></span>|<span data-ttu-id="22896-562">デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22896-562">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="22896-563">応答</span><span class="sxs-lookup"><span data-stu-id="22896-563">Response</span></span>
<span data-ttu-id="22896-564">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="22896-564">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22896-565">例</span><span class="sxs-lookup"><span data-stu-id="22896-565">Example</span></span>
### <a name="request"></a><span data-ttu-id="22896-566">要求</span><span class="sxs-lookup"><span data-stu-id="22896-566">Request</span></span>
<span data-ttu-id="22896-567">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22896-567">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22896-568">応答</span><span class="sxs-lookup"><span data-stu-id="22896-568">Response</span></span>
<span data-ttu-id="22896-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22896-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



