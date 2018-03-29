# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="af8d6-101">Create windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="af8d6-101">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="af8d6-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="af8d6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af8d6-103">新しい [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af8d6-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="af8d6-104">Prerequisites</span></span>
<span data-ttu-id="af8d6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af8d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af8d6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af8d6-107">Permission type</span></span>|<span data-ttu-id="af8d6-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="af8d6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af8d6-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="af8d6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="af8d6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af8d6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af8d6-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af8d6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af8d6-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af8d6-112">Not supported.</span></span>|
|<span data-ttu-id="af8d6-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af8d6-113">Application</span></span>|<span data-ttu-id="af8d6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af8d6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af8d6-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af8d6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="af8d6-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af8d6-116">Request headers</span></span>
|<span data-ttu-id="af8d6-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af8d6-117">Header</span></span>|<span data-ttu-id="af8d6-118">値</span><span class="sxs-lookup"><span data-stu-id="af8d6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af8d6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="af8d6-119">Authorization</span></span>|<span data-ttu-id="af8d6-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="af8d6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="af8d6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="af8d6-121">Accept</span></span>|<span data-ttu-id="af8d6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="af8d6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af8d6-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="af8d6-123">Request body</span></span>
<span data-ttu-id="af8d6-124">要求本文で、windowsPhone81GeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="af8d6-125">次の表に、windowsPhone81GeneralConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="af8d6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af8d6-126">Property</span></span>|<span data-ttu-id="af8d6-127">型</span><span class="sxs-lookup"><span data-stu-id="af8d6-127">Type</span></span>|<span data-ttu-id="af8d6-128">説明</span><span class="sxs-lookup"><span data-stu-id="af8d6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af8d6-129">id</span><span class="sxs-lookup"><span data-stu-id="af8d6-129">id</span></span>|<span data-ttu-id="af8d6-130">String</span><span class="sxs-lookup"><span data-stu-id="af8d6-130">String</span></span>|<span data-ttu-id="af8d6-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="af8d6-131">Name of the entity.</span></span> <span data-ttu-id="af8d6-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="af8d6-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af8d6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af8d6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="af8d6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8d6-134">DateTimeOffset</span></span>|<span data-ttu-id="af8d6-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="af8d6-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="af8d6-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="af8d6-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af8d6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af8d6-137">createdDateTime</span></span>|<span data-ttu-id="af8d6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8d6-138">DateTimeOffset</span></span>|<span data-ttu-id="af8d6-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="af8d6-139">DateTime the object was created.</span></span> <span data-ttu-id="af8d6-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="af8d6-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af8d6-141">description</span><span class="sxs-lookup"><span data-stu-id="af8d6-141">description</span></span>|<span data-ttu-id="af8d6-142">String</span><span class="sxs-lookup"><span data-stu-id="af8d6-142">String</span></span>|<span data-ttu-id="af8d6-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="af8d6-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="af8d6-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="af8d6-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af8d6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="af8d6-145">displayName</span></span>|<span data-ttu-id="af8d6-146">String</span><span class="sxs-lookup"><span data-stu-id="af8d6-146">String</span></span>|<span data-ttu-id="af8d6-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="af8d6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="af8d6-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="af8d6-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af8d6-149">version</span><span class="sxs-lookup"><span data-stu-id="af8d6-149">version</span></span>|<span data-ttu-id="af8d6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="af8d6-150">Int32</span></span>|<span data-ttu-id="af8d6-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="af8d6-151">Version of the device configuration.</span></span> <span data-ttu-id="af8d6-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="af8d6-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af8d6-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="af8d6-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="af8d6-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-154">Boolean</span></span>|<span data-ttu-id="af8d6-155">このポリシーを Windows Phone 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="af8d6-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="af8d6-156">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="af8d6-156">This property is read-only.</span></span>|
|<span data-ttu-id="af8d6-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="af8d6-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="af8d6-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-158">Boolean</span></span>|<span data-ttu-id="af8d6-159">コピー/貼り付けを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="af8d6-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-160">bluetoothBlocked</span></span>|<span data-ttu-id="af8d6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-161">Boolean</span></span>|<span data-ttu-id="af8d6-162">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="af8d6-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-163">cameraBlocked</span></span>|<span data-ttu-id="af8d6-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-164">Boolean</span></span>|<span data-ttu-id="af8d6-165">カメラをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="af8d6-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="af8d6-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="af8d6-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-167">Boolean</span></span>|<span data-ttu-id="af8d6-168">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="af8d6-169">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="af8d6-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="af8d6-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="af8d6-170">compliantAppsList</span></span>|<span data-ttu-id="af8d6-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="af8d6-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="af8d6-172">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="af8d6-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="af8d6-173">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="af8d6-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="af8d6-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="af8d6-174">compliantAppListType</span></span>|<span data-ttu-id="af8d6-175">String</span><span class="sxs-lookup"><span data-stu-id="af8d6-175">String</span></span>|<span data-ttu-id="af8d6-176">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="af8d6-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="af8d6-177">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="af8d6-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="af8d6-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="af8d6-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="af8d6-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-179">Boolean</span></span>|<span data-ttu-id="af8d6-180">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="af8d6-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="af8d6-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="af8d6-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-182">Boolean</span></span>|<span data-ttu-id="af8d6-183">カスタム電子メール アカウントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="af8d6-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-184">locationServicesBlocked</span></span>|<span data-ttu-id="af8d6-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-185">Boolean</span></span>|<span data-ttu-id="af8d6-186">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="af8d6-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="af8d6-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-188">Boolean</span></span>|<span data-ttu-id="af8d6-189">Microsoft アカウントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="af8d6-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-190">nfcBlocked</span></span>|<span data-ttu-id="af8d6-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-191">Boolean</span></span>|<span data-ttu-id="af8d6-192">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="af8d6-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="af8d6-193">passwordBlockSimple</span></span>|<span data-ttu-id="af8d6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-194">Boolean</span></span>|<span data-ttu-id="af8d6-195">カレンダーの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="af8d6-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="af8d6-196">passwordExpirationDays</span></span>|<span data-ttu-id="af8d6-197">Int32</span><span class="sxs-lookup"><span data-stu-id="af8d6-197">Int32</span></span>|<span data-ttu-id="af8d6-198">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="af8d6-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="af8d6-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="af8d6-199">passwordMinimumLength</span></span>|<span data-ttu-id="af8d6-200">Int32</span><span class="sxs-lookup"><span data-stu-id="af8d6-200">Int32</span></span>|<span data-ttu-id="af8d6-201">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="af8d6-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="af8d6-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="af8d6-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="af8d6-203">Int32</span><span class="sxs-lookup"><span data-stu-id="af8d6-203">Int32</span></span>|<span data-ttu-id="af8d6-204">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="af8d6-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="af8d6-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="af8d6-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="af8d6-206">Int32</span><span class="sxs-lookup"><span data-stu-id="af8d6-206">Int32</span></span>|<span data-ttu-id="af8d6-207">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="af8d6-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="af8d6-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="af8d6-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="af8d6-209">Int32</span><span class="sxs-lookup"><span data-stu-id="af8d6-209">Int32</span></span>|<span data-ttu-id="af8d6-210">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="af8d6-210">Number of previous passwords to block.</span></span> <span data-ttu-id="af8d6-211">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="af8d6-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="af8d6-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="af8d6-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="af8d6-213">Int32</span><span class="sxs-lookup"><span data-stu-id="af8d6-213">Int32</span></span>|<span data-ttu-id="af8d6-214">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="af8d6-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="af8d6-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="af8d6-215">passwordRequiredType</span></span>|<span data-ttu-id="af8d6-216">String</span><span class="sxs-lookup"><span data-stu-id="af8d6-216">String</span></span>|<span data-ttu-id="af8d6-217">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="af8d6-217">Password type that is required.</span></span> <span data-ttu-id="af8d6-218">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="af8d6-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="af8d6-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="af8d6-219">passwordRequired</span></span>|<span data-ttu-id="af8d6-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-220">Boolean</span></span>|<span data-ttu-id="af8d6-221">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="af8d6-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-222">screenCaptureBlocked</span></span>|<span data-ttu-id="af8d6-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-223">Boolean</span></span>|<span data-ttu-id="af8d6-224">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="af8d6-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="af8d6-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="af8d6-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-226">Boolean</span></span>|<span data-ttu-id="af8d6-227">リムーバブル記憶域をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="af8d6-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="af8d6-228">storageRequireEncryption</span></span>|<span data-ttu-id="af8d6-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-229">Boolean</span></span>|<span data-ttu-id="af8d6-230">暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="af8d6-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-231">webBrowserBlocked</span></span>|<span data-ttu-id="af8d6-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-232">Boolean</span></span>|<span data-ttu-id="af8d6-233">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="af8d6-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-234">wifiBlocked</span></span>|<span data-ttu-id="af8d6-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-235">Boolean</span></span>|<span data-ttu-id="af8d6-236">Wi-Fi をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="af8d6-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="af8d6-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="af8d6-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-238">Boolean</span></span>|<span data-ttu-id="af8d6-239">Wi-Fi ホットスポットへの自動接続をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="af8d6-240">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="af8d6-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="af8d6-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="af8d6-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="af8d6-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-242">Boolean</span></span>|<span data-ttu-id="af8d6-243">Wi-Fi ホットスポット レポートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="af8d6-244">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="af8d6-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="af8d6-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="af8d6-245">windowsStoreBlocked</span></span>|<span data-ttu-id="af8d6-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="af8d6-246">Boolean</span></span>|<span data-ttu-id="af8d6-247">Windows ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="af8d6-248">応答</span><span class="sxs-lookup"><span data-stu-id="af8d6-248">Response</span></span>
<span data-ttu-id="af8d6-249">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="af8d6-249">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af8d6-250">例</span><span class="sxs-lookup"><span data-stu-id="af8d6-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="af8d6-251">要求</span><span class="sxs-lookup"><span data-stu-id="af8d6-251">Request</span></span>
<span data-ttu-id="af8d6-252">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af8d6-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1525

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="af8d6-253">応答</span><span class="sxs-lookup"><span data-stu-id="af8d6-253">Response</span></span>
<span data-ttu-id="af8d6-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af8d6-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



