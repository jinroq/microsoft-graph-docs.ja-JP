# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="a2ecc-101">windows10TeamGeneralConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="a2ecc-101">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="a2ecc-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2ecc-103">新しい [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-103">Create a new [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2ecc-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2ecc-104">Prerequisites</span></span>
<span data-ttu-id="a2ecc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2ecc-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2ecc-107">Permission type</span></span>|<span data-ttu-id="a2ecc-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2ecc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2ecc-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2ecc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a2ecc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ecc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2ecc-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2ecc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2ecc-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-112">Not supported.</span></span>|
|<span data-ttu-id="a2ecc-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2ecc-113">Application</span></span>|<span data-ttu-id="a2ecc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2ecc-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2ecc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a2ecc-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2ecc-116">Request headers</span></span>
|<span data-ttu-id="a2ecc-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2ecc-117">Header</span></span>|<span data-ttu-id="a2ecc-118">値</span><span class="sxs-lookup"><span data-stu-id="a2ecc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2ecc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2ecc-119">Authorization</span></span>|<span data-ttu-id="a2ecc-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2ecc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a2ecc-121">Accept</span></span>|<span data-ttu-id="a2ecc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a2ecc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2ecc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2ecc-123">Request body</span></span>
<span data-ttu-id="a2ecc-124">要求本文で、windows10TeamGeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-124">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="a2ecc-125">次の表に、windows10TeamGeneralConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-125">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="a2ecc-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2ecc-126">Property</span></span>|<span data-ttu-id="a2ecc-127">型</span><span class="sxs-lookup"><span data-stu-id="a2ecc-127">Type</span></span>|<span data-ttu-id="a2ecc-128">説明</span><span class="sxs-lookup"><span data-stu-id="a2ecc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ecc-129">id</span><span class="sxs-lookup"><span data-stu-id="a2ecc-129">id</span></span>|<span data-ttu-id="a2ecc-130">String</span><span class="sxs-lookup"><span data-stu-id="a2ecc-130">String</span></span>|<span data-ttu-id="a2ecc-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-131">Key of the entity.</span></span> <span data-ttu-id="a2ecc-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2ecc-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2ecc-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ecc-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a2ecc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ecc-134">DateTimeOffset</span></span>|<span data-ttu-id="a2ecc-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a2ecc-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2ecc-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2ecc-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ecc-137">createdDateTime</span></span>|<span data-ttu-id="a2ecc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ecc-138">DateTimeOffset</span></span>|<span data-ttu-id="a2ecc-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-139">DateTime the object was created.</span></span> <span data-ttu-id="a2ecc-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2ecc-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2ecc-141">description</span><span class="sxs-lookup"><span data-stu-id="a2ecc-141">description</span></span>|<span data-ttu-id="a2ecc-142">String</span><span class="sxs-lookup"><span data-stu-id="a2ecc-142">String</span></span>|<span data-ttu-id="a2ecc-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2ecc-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2ecc-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2ecc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a2ecc-145">displayName</span></span>|<span data-ttu-id="a2ecc-146">String</span><span class="sxs-lookup"><span data-stu-id="a2ecc-146">String</span></span>|<span data-ttu-id="a2ecc-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2ecc-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2ecc-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2ecc-149">version</span><span class="sxs-lookup"><span data-stu-id="a2ecc-149">version</span></span>|<span data-ttu-id="a2ecc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ecc-150">Int32</span></span>|<span data-ttu-id="a2ecc-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-151">Version of the device configuration.</span></span> <span data-ttu-id="a2ecc-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2ecc-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2ecc-153">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="a2ecc-153">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="a2ecc-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-154">Boolean</span></span>|<span data-ttu-id="a2ecc-155">Azure Operational Insights をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-155">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="a2ecc-156">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="a2ecc-156">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="a2ecc-157">String</span><span class="sxs-lookup"><span data-stu-id="a2ecc-157">String</span></span>|<span data-ttu-id="a2ecc-158">Azure Operational Insights のワークスペース ID。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-158">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="a2ecc-159">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="a2ecc-159">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="a2ecc-160">String</span><span class="sxs-lookup"><span data-stu-id="a2ecc-160">String</span></span>|<span data-ttu-id="a2ecc-161">Azure Operational Insights のワークスペース キー。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-161">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="a2ecc-162">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="a2ecc-162">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="a2ecc-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-163">Boolean</span></span>|<span data-ttu-id="a2ecc-164">投影を開始するたびに、接続アプリを自動的に起動するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-164">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="a2ecc-165">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="a2ecc-165">maintenanceWindowBlocked</span></span>|<span data-ttu-id="a2ecc-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-166">Boolean</span></span>|<span data-ttu-id="a2ecc-167">デバイス更新のメンテナンス ウィンドウの設定をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-167">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="a2ecc-168">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="a2ecc-168">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="a2ecc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ecc-169">Int32</span></span>|<span data-ttu-id="a2ecc-170">デバイス更新のためのメンテナンス期間の長さ (時間)。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-170">Maintenance window duration for device updates.</span></span> <span data-ttu-id="a2ecc-171">有効な値は 0 から 5 までです</span><span class="sxs-lookup"><span data-stu-id="a2ecc-171">Valid values 0 to 5</span></span>|
|<span data-ttu-id="a2ecc-172">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="a2ecc-172">maintenanceWindowStartTime</span></span>|<span data-ttu-id="a2ecc-173">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a2ecc-173">TimeOfDay</span></span>|<span data-ttu-id="a2ecc-174">デバイス更新のためのメンテナンス期間の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-174">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="a2ecc-175">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="a2ecc-175">miracastChannel</span></span>|[<span data-ttu-id="a2ecc-176">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="a2ecc-176">miracastChannel</span></span>](../resources/intune_deviceconfig_miracastchannel.md)|<span data-ttu-id="a2ecc-177">チャネル。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-177">The channel.</span></span> <span data-ttu-id="a2ecc-178">可能な値は、`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive` です。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-178">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="a2ecc-179">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="a2ecc-179">miracastBlocked</span></span>|<span data-ttu-id="a2ecc-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-180">Boolean</span></span>|<span data-ttu-id="a2ecc-181">ワイヤレス投影をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-181">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="a2ecc-182">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="a2ecc-182">miracastRequirePin</span></span>|<span data-ttu-id="a2ecc-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-183">Boolean</span></span>|<span data-ttu-id="a2ecc-184">ワイヤレス投影の pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-184">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="a2ecc-185">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="a2ecc-185">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="a2ecc-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-186">Boolean</span></span>|<span data-ttu-id="a2ecc-187">スタート メニューで [会議とファイル] 機能を無効にするかどうかを指定します。この機能は、サインイン ユーザーの会議とファイルを Office 365 から表示します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-187">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="a2ecc-188">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="a2ecc-188">settingsBlockSessionResume</span></span>|<span data-ttu-id="a2ecc-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-189">Boolean</span></span>|<span data-ttu-id="a2ecc-190">セッションがタイムアウトになった際にセッションを再開する機能を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-190">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="a2ecc-191">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="a2ecc-191">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="a2ecc-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-192">Boolean</span></span>|<span data-ttu-id="a2ecc-193">スケジュールされている会議の招待者をサインイン ダイアログに自動入力する機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-193">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="a2ecc-194">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="a2ecc-194">settingsDefaultVolume</span></span>|<span data-ttu-id="a2ecc-195">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ecc-195">Int32</span></span>|<span data-ttu-id="a2ecc-196">新しいセッションの既定のボリューム値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-196">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="a2ecc-197">許可される値は、0 から 100 までです。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-197">Permitted values are 0-100.</span></span> <span data-ttu-id="a2ecc-198">既定値は 45 です。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-198">The default is 45.</span></span> <span data-ttu-id="a2ecc-199">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="a2ecc-199">Valid values 0 to 100</span></span>|
|<span data-ttu-id="a2ecc-200">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a2ecc-200">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="a2ecc-201">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ecc-201">Int32</span></span>|<span data-ttu-id="a2ecc-202">ハブ スクリーンがオフになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-202">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="a2ecc-203">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a2ecc-203">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="a2ecc-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ecc-204">Int32</span></span>|<span data-ttu-id="a2ecc-205">セッションがタイムアウトになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-205">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="a2ecc-206">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a2ecc-206">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="a2ecc-207">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ecc-207">Int32</span></span>|<span data-ttu-id="a2ecc-208">ハブがスリープ モードになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-208">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="a2ecc-209">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="a2ecc-209">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="a2ecc-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2ecc-210">Boolean</span></span>|<span data-ttu-id="a2ecc-211">ユーザーが入室した際に、ようこそ画面が自動的に起動するのをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-211">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="a2ecc-212">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="a2ecc-212">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="a2ecc-213">String</span><span class="sxs-lookup"><span data-stu-id="a2ecc-213">String</span></span>|<span data-ttu-id="a2ecc-214">ようこそ画面の背景画像の URL。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-214">The welcome screen background image URL.</span></span> <span data-ttu-id="a2ecc-215">URL は HTTPS プロトコルを使用し、PNG 画像を返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-215">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="a2ecc-216">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="a2ecc-216">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="a2ecc-217">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="a2ecc-217">welcomeScreenMeetingInformation</span></span>](../resources/intune_deviceconfig_welcomescreenmeetinginformation.md)|<span data-ttu-id="a2ecc-218">表示される、ようこそ画面の会議情報。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-218">The welcome screen meeting information shown.</span></span> <span data-ttu-id="a2ecc-219">可能な値は、`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject` です。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-219">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="a2ecc-220">応答</span><span class="sxs-lookup"><span data-stu-id="a2ecc-220">Response</span></span>
<span data-ttu-id="a2ecc-221">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-221">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ecc-222">例</span><span class="sxs-lookup"><span data-stu-id="a2ecc-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2ecc-223">要求</span><span class="sxs-lookup"><span data-stu-id="a2ecc-223">Request</span></span>
<span data-ttu-id="a2ecc-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1150

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="a2ecc-225">応答</span><span class="sxs-lookup"><span data-stu-id="a2ecc-225">Response</span></span>
<span data-ttu-id="a2ecc-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2ecc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1322

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```



