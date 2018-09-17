# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="546ef-101">windows10GeneralConfigurationを更新する</span><span class="sxs-lookup"><span data-stu-id="546ef-101">Update windows10GeneralConfiguration</span></span>

> <span data-ttu-id="546ef-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="546ef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="546ef-103">[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="546ef-103">Update the properties of a [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="546ef-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="546ef-104">Prerequisites</span></span>
<span data-ttu-id="546ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="546ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="546ef-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="546ef-107">Permission type</span></span>|<span data-ttu-id="546ef-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="546ef-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="546ef-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="546ef-109">Delegated (work or school account)</span></span>|<span data-ttu-id="546ef-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546ef-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="546ef-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="546ef-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="546ef-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="546ef-112">Not supported.</span></span>|
|<span data-ttu-id="546ef-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="546ef-113">Application</span></span>|<span data-ttu-id="546ef-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="546ef-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="546ef-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="546ef-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="546ef-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="546ef-116">Request headers</span></span>
|<span data-ttu-id="546ef-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="546ef-117">Header</span></span>|<span data-ttu-id="546ef-118">値</span><span class="sxs-lookup"><span data-stu-id="546ef-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="546ef-119">承認</span><span class="sxs-lookup"><span data-stu-id="546ef-119">Authorization</span></span>|<span data-ttu-id="546ef-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="546ef-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="546ef-121">承諾</span><span class="sxs-lookup"><span data-stu-id="546ef-121">Accept</span></span>|<span data-ttu-id="546ef-122">アプリケーションまたは JSON</span><span class="sxs-lookup"><span data-stu-id="546ef-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="546ef-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="546ef-123">Request body</span></span>
<span data-ttu-id="546ef-124">要求本文で、[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-124">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="546ef-125">次の表に、[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-125">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="546ef-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="546ef-126">Property</span></span>|<span data-ttu-id="546ef-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="546ef-127">Type</span></span>|<span data-ttu-id="546ef-128">説明</span><span class="sxs-lookup"><span data-stu-id="546ef-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="546ef-129">ID</span><span class="sxs-lookup"><span data-stu-id="546ef-129">id</span></span>|<span data-ttu-id="546ef-130">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-130">String</span></span>|<span data-ttu-id="546ef-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="546ef-131">Key of the entity.</span></span> <span data-ttu-id="546ef-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="546ef-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="546ef-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="546ef-133">lastModifiedDateTime</span></span>|<span data-ttu-id="546ef-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="546ef-134">DateTimeOffset</span></span>|<span data-ttu-id="546ef-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="546ef-135">DateTime the object was last modified.</span></span> <span data-ttu-id="546ef-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="546ef-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="546ef-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="546ef-137">createdDateTime</span></span>|<span data-ttu-id="546ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="546ef-138">DateTimeOffset</span></span>|<span data-ttu-id="546ef-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="546ef-139">DateTime the object was created.</span></span> <span data-ttu-id="546ef-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="546ef-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="546ef-141">説明</span><span class="sxs-lookup"><span data-stu-id="546ef-141">description</span></span>|<span data-ttu-id="546ef-142">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-142">String</span></span>|<span data-ttu-id="546ef-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="546ef-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="546ef-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="546ef-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="546ef-145">displayName</span><span class="sxs-lookup"><span data-stu-id="546ef-145">displayName</span></span>|<span data-ttu-id="546ef-146">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-146">String</span></span>|<span data-ttu-id="546ef-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="546ef-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="546ef-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="546ef-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="546ef-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="546ef-149">version</span></span>|<span data-ttu-id="546ef-150">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-150">Int32</span></span>|<span data-ttu-id="546ef-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="546ef-151">Version of the device configuration.</span></span> <span data-ttu-id="546ef-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="546ef-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="546ef-153">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="546ef-153">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="546ef-154">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-154">String</span></span>|<span data-ttu-id="546ef-155">クラウド プリンターを検出するエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="546ef-155">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="546ef-156">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="546ef-156">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="546ef-157">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-157">String</span></span>|<span data-ttu-id="546ef-158">OAuth トークンを取得するための認証エンドポイント。</span><span class="sxs-lookup"><span data-stu-id="546ef-158">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="546ef-159">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="546ef-159">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="546ef-160">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-160">String</span></span>|<span data-ttu-id="546ef-161">OAuth 認証機関から OAuth トークンを取得することを承認されているクライアント アプリケーションの GUID。</span><span class="sxs-lookup"><span data-stu-id="546ef-161">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="546ef-162">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="546ef-162">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="546ef-163">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-163">String</span></span>|<span data-ttu-id="546ef-164">Azure Portal で構成されている印刷サービスの OAuth リソース URI。</span><span class="sxs-lookup"><span data-stu-id="546ef-164">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="546ef-165">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="546ef-165">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="546ef-166">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-166">Int32</span></span>|<span data-ttu-id="546ef-167">検出エンドポイントからクエリを実行する必要があるプリンターの最大数。</span><span class="sxs-lookup"><span data-stu-id="546ef-167">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="546ef-168">これはモバイルのみでの設定です。</span><span class="sxs-lookup"><span data-stu-id="546ef-168">This is a mobile only setting.</span></span> <span data-ttu-id="546ef-169">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="546ef-170">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="546ef-170">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="546ef-171">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-171">String</span></span>|<span data-ttu-id="546ef-172">Azure Portal で構成されているプリンター検出サービスの OAuth リソース URI。</span><span class="sxs-lookup"><span data-stu-id="546ef-172">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="546ef-173">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="546ef-173">searchBlockDiacritics</span></span>|<span data-ttu-id="546ef-174">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-174">Boolean</span></span>|<span data-ttu-id="546ef-175">検索で分音記号を使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-175">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="546ef-176">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="546ef-176">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="546ef-177">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-177">Boolean</span></span>|<span data-ttu-id="546ef-178">コンテンツとプロパティのインデックスを作成するときに、自動言語検出を使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-178">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="546ef-179">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="546ef-179">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="546ef-180">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-180">Boolean</span></span>|<span data-ttu-id="546ef-181">Cortana またはエクスプローラーの検索結果に表示されないようにするため、WIP で保護されているアイテムのインデックス作成を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-181">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="546ef-182">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="546ef-182">searchEnableRemoteQueries</span></span>|<span data-ttu-id="546ef-183">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-183">Boolean</span></span>|<span data-ttu-id="546ef-184">このコンピューターのインデックスに対するリモート クエリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-184">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="546ef-185">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="546ef-185">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="546ef-186">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-186">Boolean</span></span>|<span data-ttu-id="546ef-187">インデクサー バックオフの検索機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-187">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="546ef-188">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="546ef-188">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="546ef-189">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-189">Boolean</span></span>|<span data-ttu-id="546ef-190">リムーバブル ドライブ上の場所をライブラリに追加してインデックスを作成することをユーザーに許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-190">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="546ef-191">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="546ef-191">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="546ef-192">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-192">Boolean</span></span>|<span data-ttu-id="546ef-193">インデックスの場所と同じドライブ上のハード ドライブ領域の最小値を指定して、その最小値を下回ったらインデックス作成を停止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-193">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="546ef-194">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="546ef-194">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="546ef-195">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="546ef-195">diagnosticDataSubmissionMode</span></span>](../resources/intune_deviceconfig_diagnosticdatasubmissionmode.md)|<span data-ttu-id="546ef-p109">Watsonのような診断および使用遠隔測定法データを送信するためのデバイス用の値を取得または設定します。可能な値は、 `userDefined`, `none`, `basic`, `enhanced`, `full`です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p109">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson. The possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="546ef-198">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="546ef-198">oneDriveDisableFileSync</span></span>|<span data-ttu-id="546ef-199">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-199">Boolean</span></span>|<span data-ttu-id="546ef-200">アプリや機能から OneDrive 上のファイルを操作することを IT 管理者が禁止できるかどうかを示す値を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-200">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="546ef-201">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="546ef-201">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="546ef-202">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-202">Boolean</span></span>|<span data-ttu-id="546ef-203">ユーザーがストア以外の場所からアプリをインストールできるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="546ef-203">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="546ef-204">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="546ef-204">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="546ef-205">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-205">String</span></span>|<span data-ttu-id="546ef-206">ダウンロードしてデスクトップ画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはデスクトップ画像として使用する必要があるファイル システム上のローカル画像のファイル URL。</span><span class="sxs-lookup"><span data-stu-id="546ef-206">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="546ef-207">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="546ef-207">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="546ef-208">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-208">String</span></span>|<span data-ttu-id="546ef-209">ダウンロードしてロック画面画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはロック画面画像として使用する必要があるファイル システム上のローカル画像のファイル URL。</span><span class="sxs-lookup"><span data-stu-id="546ef-209">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="546ef-210">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="546ef-210">bluetoothAllowedServices</span></span>|<span data-ttu-id="546ef-211">String コレクション</span><span class="sxs-lookup"><span data-stu-id="546ef-211">String collection</span></span>|<span data-ttu-id="546ef-212">許可されている Bluetooth サービスおよびプロファイルの一覧を 16 進形式の文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-212">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="546ef-213">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="546ef-213">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="546ef-214">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-214">Boolean</span></span>|<span data-ttu-id="546ef-215">ユーザーが Bluetooth 広告を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-215">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="546ef-216">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="546ef-216">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="546ef-217">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-217">Boolean</span></span>|<span data-ttu-id="546ef-218">ユーザーが Bluetooth の発見可能モードを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-218">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="546ef-219">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="546ef-219">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="546ef-220">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-220">Boolean</span></span>|<span data-ttu-id="546ef-221">バンドルされた特定のいくつかの Bluetooth 周辺機器を自動的にホスト デバイスとペアにすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-221">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="546ef-222">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="546ef-222">edgeBlockAutofill</span></span>|<span data-ttu-id="546ef-223">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-223">Boolean</span></span>|<span data-ttu-id="546ef-224">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-224">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="546ef-225">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-225">edgeBlocked</span></span>|<span data-ttu-id="546ef-226">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-226">Boolean</span></span>|<span data-ttu-id="546ef-227">ユーザーが Edge ブラウザーを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-227">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="546ef-228">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="546ef-228">edgeCookiePolicy</span></span>|[<span data-ttu-id="546ef-229">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="546ef-229">edgeCookiePolicy</span></span>](../resources/intune_deviceconfig_edgecookiepolicy.md)|<span data-ttu-id="546ef-p110">エッジのブラウザーでブロックしている cookie を指定します。可能な値は、 `userDefined`, `allow`, `blockThirdParty`, `blockAll`です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p110">Indicates which cookies to block in the Edge browser. The possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="546ef-232">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="546ef-232">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="546ef-233">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-233">Boolean</span></span>|<span data-ttu-id="546ef-234">Edge ブラウザー内の開発者ツールを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-234">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="546ef-235">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="546ef-235">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="546ef-236">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-236">Boolean</span></span>|<span data-ttu-id="546ef-237">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-237">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="546ef-238">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="546ef-238">edgeBlockExtensions</span></span>|<span data-ttu-id="546ef-239">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-239">Boolean</span></span>|<span data-ttu-id="546ef-240">Edge ブラウザーの拡張機能を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-240">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="546ef-241">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="546ef-241">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="546ef-242">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-242">Boolean</span></span>|<span data-ttu-id="546ef-243">Edge ブラウザーで会社のネットワークの InPrivate ブラウズを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-243">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="546ef-244">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="546ef-244">edgeBlockJavaScript</span></span>|<span data-ttu-id="546ef-245">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-245">Boolean</span></span>|<span data-ttu-id="546ef-246">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-246">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="546ef-247">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="546ef-247">edgeBlockPasswordManager</span></span>|<span data-ttu-id="546ef-248">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-248">Boolean</span></span>|<span data-ttu-id="546ef-249">パスワード マネージャーを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-249">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="546ef-250">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="546ef-250">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="546ef-251">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-251">Boolean</span></span>|<span data-ttu-id="546ef-252">Microsoft Edge のアドレス バー ドロップダウン機能を禁止します。</span><span class="sxs-lookup"><span data-stu-id="546ef-252">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="546ef-253">Microsoft Edge から Microsoft サービスへのネットワーク接続を最小限に抑えるには、この設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="546ef-253">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="546ef-254">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="546ef-254">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="546ef-255">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-255">Boolean</span></span>|<span data-ttu-id="546ef-256">Microsoft Edge での Microsoft 互換性リストを禁止します。</span><span class="sxs-lookup"><span data-stu-id="546ef-256">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="546ef-257">Microsoft ではこのリストを利用して、既知の互換性の問題があるサイトを Edge で正しく表示できるようにします。</span><span class="sxs-lookup"><span data-stu-id="546ef-257">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="546ef-258">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="546ef-258">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="546ef-259">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-259">Boolean</span></span>|<span data-ttu-id="546ef-260">Microsoft Edge の終了時にブラウズ データを消去します。</span><span class="sxs-lookup"><span data-stu-id="546ef-260">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="546ef-261">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="546ef-261">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="546ef-262">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-262">Boolean</span></span>|<span data-ttu-id="546ef-263">Edge のスタート ページをユーザーが変更することを許可します。</span><span class="sxs-lookup"><span data-stu-id="546ef-263">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="546ef-264">ユーザーが Edge を開いたときに既定で表示されるスタート ページを指定するには、EdgeHomepageUrls を使用します。</span><span class="sxs-lookup"><span data-stu-id="546ef-264">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="546ef-265">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="546ef-265">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="546ef-266">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-266">Boolean</span></span>|<span data-ttu-id="546ef-267">Microsoft Edge の初回使用時に表示される Microsoft の Web ページを禁止します。</span><span class="sxs-lookup"><span data-stu-id="546ef-267">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="546ef-268">このポリシーでは、ゼロ エミッション構成に登録している企業などが、このページの表示を禁止できます。</span><span class="sxs-lookup"><span data-stu-id="546ef-268">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="546ef-269">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="546ef-269">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="546ef-270">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-270">Boolean</span></span>|<span data-ttu-id="546ef-271">ユーザーが Microsoft Edge からスタートにサイトをピン留めしたときに、ライブ タイルを作成するために Microsoft が情報を収集することを禁止します。</span><span class="sxs-lookup"><span data-stu-id="546ef-271">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="546ef-272">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="546ef-272">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="546ef-273">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-273">Boolean</span></span>|<span data-ttu-id="546ef-274">Internet Explorer と Microsoft Edge の間でお気に入りの同期を有効にします。</span><span class="sxs-lookup"><span data-stu-id="546ef-274">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="546ef-275">お気に入りの追加、削除、変更、順序変更が、ブラウザー間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="546ef-275">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="546ef-276">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="546ef-276">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="546ef-277">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-277">Boolean</span></span>|<span data-ttu-id="546ef-278">ローミング中に携帯電話上でユーザーがデータを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-278">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="546ef-279">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="546ef-279">cellularBlockVpn</span></span>|<span data-ttu-id="546ef-280">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-280">Boolean</span></span>|<span data-ttu-id="546ef-281">携帯電話上でユーザーが VPN を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-281">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="546ef-282">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="546ef-282">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="546ef-283">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-283">Boolean</span></span>|<span data-ttu-id="546ef-284">ローミング時に携帯電話上でユーザーが VPN を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-284">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="546ef-285">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="546ef-285">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="546ef-286">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-286">Boolean</span></span>|<span data-ttu-id="546ef-287">エンド ユーザーが Defender にアクセスすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-287">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="546ef-288">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="546ef-288">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="546ef-289">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-289">Int32</span></span>|<span data-ttu-id="546ef-290">検疫済みのマルウェアを削除するまでの日数。</span><span class="sxs-lookup"><span data-stu-id="546ef-290">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="546ef-291">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-291">Valid values 0 to 90</span></span>|
|<span data-ttu-id="546ef-292">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="546ef-292">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="546ef-293">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="546ef-293">defenderDetectedMalwareActions</span></span>](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|<span data-ttu-id="546ef-294">検出されたマルウェアに対する Defender のアクションを脅威レベルごとに取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-294">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="546ef-295">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="546ef-295">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="546ef-296">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="546ef-296">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="546ef-p117">Defender がシステムをスキャンする曜日。可能な値は、 `userDefined`、 `everyday`、 `sunday`、 `monday`、 `tuesday`、 `wednesday`、 `thursday`、 `friday`、 `saturday`です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p117">Defender day of the week for the system scan. The possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="546ef-299">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="546ef-299">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="546ef-300">String コレクション</span><span class="sxs-lookup"><span data-stu-id="546ef-300">String collection</span></span>|<span data-ttu-id="546ef-301">スキャンとリアルタイム保護から除外するファイルとフォルダー。</span><span class="sxs-lookup"><span data-stu-id="546ef-301">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="546ef-302">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="546ef-302">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="546ef-303">String コレクション</span><span class="sxs-lookup"><span data-stu-id="546ef-303">String collection</span></span>|<span data-ttu-id="546ef-304">スキャンとリアルタイム保護から除外するファイル拡張子。</span><span class="sxs-lookup"><span data-stu-id="546ef-304">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="546ef-305">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="546ef-305">defenderScanMaxCpu</span></span>|<span data-ttu-id="546ef-306">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-306">Int32</span></span>|<span data-ttu-id="546ef-307">スキャン中の最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="546ef-307">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="546ef-308">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-308">Valid values 0 to 100</span></span>|
|<span data-ttu-id="546ef-309">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="546ef-309">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="546ef-310">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="546ef-310">defenderMonitorFileActivity</span></span>](../resources/intune_deviceconfig_defendermonitorfileactivity.md)|<span data-ttu-id="546ef-p119">ファイル アクティビティを監視する値。可能な値: `userDefined`、 `disable`、 `monitorAllFiles`、 `monitorIncomingFilesOnly`、 `monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="546ef-p119">Value for monitoring file activity. The possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="546ef-313">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="546ef-313">defenderProcessesToExclude</span></span>|<span data-ttu-id="546ef-314">String コレクション</span><span class="sxs-lookup"><span data-stu-id="546ef-314">String collection</span></span>|<span data-ttu-id="546ef-315">スキャンとリアルタイム保護から除外するプロセス。</span><span class="sxs-lookup"><span data-stu-id="546ef-315">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="546ef-316">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="546ef-316">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="546ef-317">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="546ef-317">defenderPromptForSampleSubmission</span></span>](../resources/intune_deviceconfig_defenderpromptforsamplesubmission.md)|<span data-ttu-id="546ef-p120">ユーザーにサンプルの送信を要求する方法の設定。可能な値は、 `userDefined`、 `alwaysPrompt`、 `promptBeforeSendingPersonalData`、 `neverSendData`、 `sendAllDataWithoutPrompting` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p120">The configuration for how to prompt user for sample submission. The possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="546ef-320">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="546ef-320">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="546ef-321">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-321">Boolean</span></span>|<span data-ttu-id="546ef-322">動作の監視が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-322">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="546ef-323">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="546ef-323">defenderRequireCloudProtection</span></span>|<span data-ttu-id="546ef-324">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-324">Boolean</span></span>|<span data-ttu-id="546ef-325">クラウドの保護が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-325">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="546ef-326">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="546ef-326">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="546ef-327">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-327">Boolean</span></span>|<span data-ttu-id="546ef-328">ネットワーク検査システムが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-328">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="546ef-329">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="546ef-329">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="546ef-330">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-330">Boolean</span></span>|<span data-ttu-id="546ef-331">リアルタイムの監視が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-331">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="546ef-332">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="546ef-332">defenderScanArchiveFiles</span></span>|<span data-ttu-id="546ef-333">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-333">Boolean</span></span>|<span data-ttu-id="546ef-334">アーカイブ ファイルをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-334">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="546ef-335">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="546ef-335">defenderScanDownloads</span></span>|<span data-ttu-id="546ef-336">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-336">Boolean</span></span>|<span data-ttu-id="546ef-337">ダウンロードをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-337">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="546ef-338">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="546ef-338">defenderScanNetworkFiles</span></span>|<span data-ttu-id="546ef-339">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-339">Boolean</span></span>|<span data-ttu-id="546ef-340">ネットワーク フォルダーから開かれたファイルをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-340">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="546ef-341">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="546ef-341">defenderScanIncomingMail</span></span>|<span data-ttu-id="546ef-342">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-342">Boolean</span></span>|<span data-ttu-id="546ef-343">受信メール メッセージをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-343">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="546ef-344">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="546ef-344">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="546ef-345">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-345">Boolean</span></span>|<span data-ttu-id="546ef-346">フル スキャン時に、マップされたネットワーク ドライブをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-346">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="546ef-347">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="546ef-347">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="546ef-348">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-348">Boolean</span></span>|<span data-ttu-id="546ef-349">フル スキャン時に、リムーバブル ドライブをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-349">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="546ef-350">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="546ef-350">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="546ef-351">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-351">Boolean</span></span>|<span data-ttu-id="546ef-352">Internet Explorer ブラウザーに読み込まれるスクリプトをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-352">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="546ef-353">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="546ef-353">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="546ef-354">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-354">Int32</span></span>|<span data-ttu-id="546ef-355">署名を更新する間隔 (時間)。</span><span class="sxs-lookup"><span data-stu-id="546ef-355">The signature update interval in hours.</span></span> <span data-ttu-id="546ef-356">確認しない場合は 0 を指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-356">Specify 0 not to check.</span></span> <span data-ttu-id="546ef-357">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-357">Valid values 0 to 24</span></span>|
|<span data-ttu-id="546ef-358">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="546ef-358">defenderScanType</span></span>|[<span data-ttu-id="546ef-359">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="546ef-359">defenderScanType</span></span>](../resources/intune_deviceconfig_defenderscantype.md)|<span data-ttu-id="546ef-p122">Defender のシステム スキャンの種類。可能な値は、 `userDefined`、 `disabled`、 `quick`、 `full`です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p122">The defender system scan type. The possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="546ef-362">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="546ef-362">defenderScheduledScanTime</span></span>|<span data-ttu-id="546ef-363">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="546ef-363">TimeOfDay</span></span>|<span data-ttu-id="546ef-364">システムのスキャンの Defender 時刻。</span><span class="sxs-lookup"><span data-stu-id="546ef-364">The defender time for the system scan.</span></span>|
|<span data-ttu-id="546ef-365">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="546ef-365">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="546ef-366">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="546ef-366">TimeOfDay</span></span>|<span data-ttu-id="546ef-367">毎日のクイック スキャンを実行する時刻。</span><span class="sxs-lookup"><span data-stu-id="546ef-367">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="546ef-368">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="546ef-368">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="546ef-369">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="546ef-369">defenderCloudBlockLevelType</span></span>](../resources/intune_deviceconfig_defendercloudblockleveltype.md)|<span data-ttu-id="546ef-p123">クラウドが提供する保護のレベルを指定します。可能な値は、`notConfigured`、 `high`、 `highPlus`、 `zeroTolerance`です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p123">Specifies the level of cloud-delivered protection. The possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="546ef-372">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="546ef-372">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="546ef-373">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-373">Boolean</span></span>|<span data-ttu-id="546ef-374">Windows 10 Mobile デバイスのロック画面で、画面のタイムアウトを制御するユーザー構成可能な設定を表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-374">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="546ef-375">このポリシーが [許可] に設定されている場合は、lockScreenTimeoutInSeconds によって設定された値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="546ef-375">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="546ef-376">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="546ef-376">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="546ef-377">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-377">Boolean</span></span>|<span data-ttu-id="546ef-378">ロック画面上のアクション センター通知を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-378">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="546ef-379">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="546ef-379">lockScreenBlockCortana</span></span>|<span data-ttu-id="546ef-380">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-380">Boolean</span></span>|<span data-ttu-id="546ef-381">システムのロック中にユーザーが音声認識を使用して Cortana と対話できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-381">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="546ef-382">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="546ef-382">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="546ef-383">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-383">Boolean</span></span>|<span data-ttu-id="546ef-384">デバイスのロック画面へのトースト通知を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-384">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="546ef-385">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="546ef-385">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="546ef-386">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-386">Int32</span></span>|<span data-ttu-id="546ef-387">Windows 10 Mobile デバイスで画面をロックしてから画面をオフにするまでの時間 (秒) を設定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-387">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="546ef-388">サポートされている値は 11 から 1800 までです。</span><span class="sxs-lookup"><span data-stu-id="546ef-388">Supported values are 11-1800.</span></span> <span data-ttu-id="546ef-389">有効な値は 11 から 1800 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-389">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="546ef-390">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="546ef-390">passwordBlockSimple</span></span>|<span data-ttu-id="546ef-391">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-391">Boolean</span></span>|<span data-ttu-id="546ef-392">"1111" や "1234" などの PIN またはパスワードを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-392">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="546ef-393">Windows 10 デスクトップでは、ピクチャ パスワードの使用も制御します。</span><span class="sxs-lookup"><span data-stu-id="546ef-393">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="546ef-394">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="546ef-394">passwordExpirationDays</span></span>|<span data-ttu-id="546ef-395">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-395">Int32</span></span>|<span data-ttu-id="546ef-396">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="546ef-396">The password expiration in days.</span></span> <span data-ttu-id="546ef-397">有効な値は 0 から 730 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-397">Valid values 0 to 730</span></span>|
|<span data-ttu-id="546ef-398">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="546ef-398">passwordMinimumLength</span></span>|<span data-ttu-id="546ef-399">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-399">Int32</span></span>|<span data-ttu-id="546ef-400">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="546ef-400">The minimum password length.</span></span> <span data-ttu-id="546ef-401">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-401">Valid values 4 to 16</span></span>|
|<span data-ttu-id="546ef-402">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="546ef-402">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="546ef-403">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-403">Int32</span></span>|<span data-ttu-id="546ef-404">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="546ef-404">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="546ef-405">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="546ef-405">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="546ef-406">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-406">Int32</span></span>|<span data-ttu-id="546ef-407">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="546ef-407">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="546ef-408">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="546ef-408">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="546ef-409">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-409">Int32</span></span>|<span data-ttu-id="546ef-410">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="546ef-410">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="546ef-411">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-411">Valid values 0 to 50</span></span>|
|<span data-ttu-id="546ef-412">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="546ef-412">passwordRequired</span></span>|<span data-ttu-id="546ef-413">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-413">Boolean</span></span>|<span data-ttu-id="546ef-414">ユーザーにパスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-414">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="546ef-415">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="546ef-415">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="546ef-416">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-416">Boolean</span></span>|<span data-ttu-id="546ef-417">アイドル状態からの再開時にパスワードを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-417">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="546ef-418">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="546ef-418">passwordRequiredType</span></span>|[<span data-ttu-id="546ef-419">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="546ef-419">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="546ef-p130">必要なパスワードの種類です。使用可能な値は`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p130">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="546ef-422">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="546ef-422">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="546ef-423">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-423">Int32</span></span>|<span data-ttu-id="546ef-424">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="546ef-424">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="546ef-425">有効な値は 0 から 999 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-425">Valid values 0 to 999</span></span>|
|<span data-ttu-id="546ef-426">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="546ef-426">privacyAdvertisingId</span></span>|[<span data-ttu-id="546ef-427">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="546ef-427">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="546ef-p132">広告IDの使用を有効化または非有効化します。バージョン1607のWindows 10 に追加されています。可能な値は、`notConfigured`, `blocked`, `allowed`です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p132">Enables or disables the use of advertising ID. Added in Windows 10, version 1607. The possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="546ef-431">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="546ef-431">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="546ef-432">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-432">Boolean</span></span>|<span data-ttu-id="546ef-433">アプリの起動時に、ペアリングとプライバシーに関するユーザーの同意ダイアログの自動受け入れを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-433">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="546ef-434">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="546ef-434">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="546ef-435">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-435">Boolean</span></span>|<span data-ttu-id="546ef-436">Cortana、音声入力、ストア アプリケーションに対するクラウド ベースの音声サービスの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-436">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="546ef-437">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="546ef-437">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="546ef-438">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-438">Boolean</span></span>|<span data-ttu-id="546ef-439">ユーザーがタスク バーからアプリのピン留めを外すことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-439">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="546ef-440">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="546ef-440">startMenuAppListVisibility</span></span>|[<span data-ttu-id="546ef-441">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="546ef-441">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune_deviceconfig_windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="546ef-p133">この値を設定すると、アプリ リストを折りたたんだり、アプリ リスト全体を削除したり、設定アプリで対応する切り替えが無効になります。可能な値は、 `userDefined`, `collapse`, `remove`, `disableSettingsApp` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p133">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app. The possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="546ef-444">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="546ef-444">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="546ef-445">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-445">Boolean</span></span>|<span data-ttu-id="546ef-446">このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウント設定の変更] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-446">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="546ef-447">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="546ef-447">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="546ef-448">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-448">Boolean</span></span>|<span data-ttu-id="546ef-449">このポリシーを有効にすると、よく使われるアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="546ef-449">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="546ef-450">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="546ef-450">startMenuHideHibernate</span></span>|<span data-ttu-id="546ef-451">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-451">Boolean</span></span>|<span data-ttu-id="546ef-452">このポリシーを有効にすると、スタート メニューの電源ボタンに [休止状態] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-452">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="546ef-453">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="546ef-453">startMenuHideLock</span></span>|<span data-ttu-id="546ef-454">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-454">Boolean</span></span>|<span data-ttu-id="546ef-455">このポリシーを有効にすると、スタート メニューのユーザー タイルに [ロック] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-455">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="546ef-456">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="546ef-456">startMenuHidePowerButton</span></span>|<span data-ttu-id="546ef-457">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-457">Boolean</span></span>|<span data-ttu-id="546ef-458">このポリシーを有効にすると、スタート メニューに電源ボタンが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-458">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="546ef-459">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="546ef-459">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="546ef-460">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-460">Boolean</span></span>|<span data-ttu-id="546ef-461">このポリシーを有効にすると、最近開いた項目のジャンプ リストがスタート メニュー/タスクバーに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="546ef-461">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="546ef-462">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="546ef-462">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="546ef-463">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-463">Boolean</span></span>|<span data-ttu-id="546ef-464">このポリシーを有効にすると、最近追加したアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="546ef-464">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="546ef-465">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="546ef-465">startMenuHideRestartOptions</span></span>|<span data-ttu-id="546ef-466">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-466">Boolean</span></span>|<span data-ttu-id="546ef-467">このポリシーを有効にすると、スタート メニューの電源ボタンに [再起動]/[更新して再起動] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-467">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="546ef-468">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="546ef-468">startMenuHideShutDown</span></span>|<span data-ttu-id="546ef-469">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-469">Boolean</span></span>|<span data-ttu-id="546ef-470">このポリシーを有効にすると、スタート メニューの電源ボタンに [シャットダウン]/[更新してシャットダウン] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-470">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="546ef-471">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="546ef-471">startMenuHideSignOut</span></span>|<span data-ttu-id="546ef-472">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-472">Boolean</span></span>|<span data-ttu-id="546ef-473">このポリシーを有効にすると、スタート メニューのユーザー タイルに [サインアウト] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-473">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="546ef-474">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="546ef-474">startMenuHideSleep</span></span>|<span data-ttu-id="546ef-475">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-475">Boolean</span></span>|<span data-ttu-id="546ef-476">このポリシーを有効にすると、スタート メニューの電源ボタンに [スリープ] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-476">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="546ef-477">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="546ef-477">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="546ef-478">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-478">Boolean</span></span>|<span data-ttu-id="546ef-479">このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウントの切り替え] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-479">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="546ef-480">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="546ef-480">startMenuHideUserTile</span></span>|<span data-ttu-id="546ef-481">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-481">Boolean</span></span>|<span data-ttu-id="546ef-482">このポリシーを有効にすると、スタート メニューにユーザー タイルが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="546ef-482">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="546ef-483">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="546ef-483">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="546ef-484">バイナリ</span><span class="sxs-lookup"><span data-stu-id="546ef-484">Binary</span></span>|<span data-ttu-id="546ef-485">このポリシー設定では、Edge アセットをインポートして startMenuLayoutXml ポリシーで使用することができます。</span><span class="sxs-lookup"><span data-stu-id="546ef-485">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="546ef-486">スタートのレイアウトには、Edge アプリからのセカンダリ タイルを含めることができ、このタイルは Edge のローカル アセット ファイルを検索します。</span><span class="sxs-lookup"><span data-stu-id="546ef-486">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="546ef-487">Edge のローカル アセットは存在しないことがあり、その場合は Edge のセカンダリ タイルが空で表示されます。</span><span class="sxs-lookup"><span data-stu-id="546ef-487">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="546ef-488">このポリシーは、startMenuLayoutXml ポリシーが変更された場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="546ef-488">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="546ef-489">値は、UTF-8 の Base64 でエンコードされたバイト配列にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="546ef-489">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="546ef-490">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="546ef-490">startMenuLayoutXml</span></span>|<span data-ttu-id="546ef-491">バイナリ</span><span class="sxs-lookup"><span data-stu-id="546ef-491">Binary</span></span>|<span data-ttu-id="546ef-492">管理者がスタート メニューの既定のレイアウトを上書きし、ユーザーがこれを変更できないようにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="546ef-492">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="546ef-493">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-493">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="546ef-494">XML は、UTF8 エンコードのバイト配列形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="546ef-494">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="546ef-495">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="546ef-495">startMenuMode</span></span>|[<span data-ttu-id="546ef-496">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="546ef-496">windowsStartMenuModeType</span></span>](../resources/intune_deviceconfig_windowsstartmenumodetype.md)|<span data-ttu-id="546ef-p136">管理者は、[スタート]メニューの表示方法を決定できます。可能な値は、`userDefined`, `fullScreen`, `nonFullScreen` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p136">Allows admins to decide how the Start menu is displayed. The possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="546ef-499">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="546ef-499">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="546ef-500">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-500">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p137">スタート メニューへのドキュメント フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p137">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-503">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="546ef-503">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="546ef-504">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-504">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p138">スタート メニューへのダウンロード フォルダー ショートカットの表示/非表示を強制します。可能な値は、`notConfigured`, `hide`, `show` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p138">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-507">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="546ef-507">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="546ef-508">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-508">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p139">スタート メニューへのファイル エクスプローラー ショートカットの表示/非表示を強制します。可能な値は、  `notConfigured`, `hide`, `show` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p139">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-511">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="546ef-511">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="546ef-512">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-512">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p140">スタート メニューへのホームグループ フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p140">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-515">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="546ef-515">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="546ef-516">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-516">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p141">スタート メニューへのミュージック フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show`  です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p141">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-519">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="546ef-519">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="546ef-520">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-520">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p142">スタート メニューへのネットワーク フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p142">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-523">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="546ef-523">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="546ef-524">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-524">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p143">スタート メニューへの個人用フォルダー ショートカットの表示/非表示を強制します。可能な値は、   `notConfigured`, `hide`, `show`  です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p143">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-527">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="546ef-527">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="546ef-528">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-528">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p144">スタート メニューへのピクチャ フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p144">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-531">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="546ef-531">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="546ef-532">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-532">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p145">スタート メニューへのピクチャ フォルダー ショートカットの表示/非表示を強制します。可能な値は、`notConfigured`, `hide`, `show` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p145">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-535">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="546ef-535">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="546ef-536">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="546ef-536">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="546ef-p146">スタート メニューへのビデオ フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p146">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="546ef-539">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="546ef-539">settingsBlockSettingsApp</span></span>|<span data-ttu-id="546ef-540">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-540">Boolean</span></span>|<span data-ttu-id="546ef-541">設定アプリへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-541">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="546ef-542">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="546ef-542">settingsBlockSystemPage</span></span>|<span data-ttu-id="546ef-543">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-543">Boolean</span></span>|<span data-ttu-id="546ef-544">設定アプリ内の [システム] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-544">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="546ef-545">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="546ef-545">settingsBlockDevicesPage</span></span>|<span data-ttu-id="546ef-546">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-546">Boolean</span></span>|<span data-ttu-id="546ef-547">設定アプリ内の [デバイス] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-547">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="546ef-548">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="546ef-548">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="546ef-549">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-549">Boolean</span></span>|<span data-ttu-id="546ef-550">設定アプリ内の [ネットワークとインターネット] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-550">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="546ef-551">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="546ef-551">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="546ef-552">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-552">Boolean</span></span>|<span data-ttu-id="546ef-553">設定アプリ内の [個人用設定] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-553">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="546ef-554">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="546ef-554">settingsBlockAccountsPage</span></span>|<span data-ttu-id="546ef-555">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-555">Boolean</span></span>|<span data-ttu-id="546ef-556">設定アプリ内の [アカウント] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-556">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="546ef-557">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="546ef-557">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="546ef-558">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-558">Boolean</span></span>|<span data-ttu-id="546ef-559">設定アプリ内の [時刻と言語] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-559">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="546ef-560">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="546ef-560">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="546ef-561">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-561">Boolean</span></span>|<span data-ttu-id="546ef-562">設定アプリ内の [簡単操作] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-562">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="546ef-563">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="546ef-563">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="546ef-564">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-564">Boolean</span></span>|<span data-ttu-id="546ef-565">設定アプリ内の [プライバシー] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-565">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="546ef-566">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="546ef-566">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="546ef-567">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-567">Boolean</span></span>|<span data-ttu-id="546ef-568">設定アプリ内の [更新とセキュリティ] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-568">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="546ef-569">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="546ef-569">settingsBlockAppsPage</span></span>|<span data-ttu-id="546ef-570">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-570">Boolean</span></span>|<span data-ttu-id="546ef-571">設定アプリ内の [アプリ] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-571">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="546ef-572">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="546ef-572">settingsBlockGamingPage</span></span>|<span data-ttu-id="546ef-573">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-573">Boolean</span></span>|<span data-ttu-id="546ef-574">設定アプリ内の [ゲーム] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-574">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="546ef-575">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="546ef-575">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="546ef-576">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-576">Boolean</span></span>|<span data-ttu-id="546ef-577">通常はコンシューマー向けのエクスペリエンスを IT 管理者が禁止できるようにします。たとえば、開始時の提案、メンバーシップ通知、OOBE 後のアプリ インストール、リダイレクト タイルなどです。</span><span class="sxs-lookup"><span data-stu-id="546ef-577">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="546ef-578">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-578">windowsSpotlightBlocked</span></span>|<span data-ttu-id="546ef-579">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-579">Boolean</span></span>|<span data-ttu-id="546ef-580">IT 管理者が Windows スポットライトのすべての機能をオフにできるようにします</span><span class="sxs-lookup"><span data-stu-id="546ef-580">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="546ef-581">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="546ef-581">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="546ef-582">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-582">Boolean</span></span>|<span data-ttu-id="546ef-583">各 OS のクリーン インストールやアップグレードの後、またはその後も継続的に、新しい機能や変更された機能を Microsoft からユーザーに紹介することを禁止します</span><span class="sxs-lookup"><span data-stu-id="546ef-583">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="546ef-584">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="546ef-584">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="546ef-585">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-585">Boolean</span></span>|<span data-ttu-id="546ef-586">ユーザーのデバイスの使用状況に基づいて Windows スポットライトのコンテンツをカスタマイズすることを禁止します。</span><span class="sxs-lookup"><span data-stu-id="546ef-586">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="546ef-587">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="546ef-587">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="546ef-588">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-588">Boolean</span></span>|<span data-ttu-id="546ef-589">Windows スポットライト経由でサード パーティのコンテンツを配信することを禁止します</span><span class="sxs-lookup"><span data-stu-id="546ef-589">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="546ef-590">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="546ef-590">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="546ef-591">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-591">Boolean</span></span>|<span data-ttu-id="546ef-592">Windows スポットライトからの Windows へようこそのエクスペリエンスを禁止します</span><span class="sxs-lookup"><span data-stu-id="546ef-592">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="546ef-593">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="546ef-593">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="546ef-594">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-594">Boolean</span></span>|<span data-ttu-id="546ef-595">Windows のヒントのポップアップを IT 管理者がオフにできるようにします。</span><span class="sxs-lookup"><span data-stu-id="546ef-595">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="546ef-596">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="546ef-596">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="546ef-597">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="546ef-597">windowsSpotlightEnablementSettings</span></span>](../resources/intune_deviceconfig_windowsspotlightenablementsettings.md)|<span data-ttu-id="546ef-p147">スポットライトの種類を指定します。可能な値は、  `notConfigured`、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p147">Specifies the type of Spotlight Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="546ef-600">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="546ef-600">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="546ef-601">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-601">Boolean</span></span>|<span data-ttu-id="546ef-602">オンに設定すると、プロキシの設定がデバイスのすべてのプロセスとアカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="546ef-602">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="546ef-603">それ以外の場合は、MDM に登録されているユーザー アカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="546ef-603">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="546ef-604">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="546ef-604">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="546ef-605">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-605">Boolean</span></span>|<span data-ttu-id="546ef-606">設定の自動検出を無効にします。</span><span class="sxs-lookup"><span data-stu-id="546ef-606">Disable automatic detection of settings.</span></span> <span data-ttu-id="546ef-607">有効にした場合、システムはプロキシ自動構成 (PAC) スクリプトへのパスを検索します。</span><span class="sxs-lookup"><span data-stu-id="546ef-607">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="546ef-608">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="546ef-608">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="546ef-609">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-609">String</span></span>|<span data-ttu-id="546ef-610">使用するプロキシ自動構成 (PAC) スクリプトのアドレス。</span><span class="sxs-lookup"><span data-stu-id="546ef-610">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="546ef-611">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="546ef-611">networkProxyServer</span></span>|[<span data-ttu-id="546ef-612">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="546ef-612">windows10NetworkProxyServer</span></span>](../resources/intune_deviceconfig_windows10networkproxyserver.md)|<span data-ttu-id="546ef-613">プロキシ サーバーの設定を手動で指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-613">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="546ef-614">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="546ef-614">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="546ef-615">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-615">Boolean</span></span>|<span data-ttu-id="546ef-616">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-616">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="546ef-617">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-617">antiTheftModeBlocked</span></span>|<span data-ttu-id="546ef-618">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-618">Boolean</span></span>|<span data-ttu-id="546ef-619">ユーザーが盗難防止モードの設定を選択することを禁止するかどうかを示します (Windows 10 Mobile のみ)。</span><span class="sxs-lookup"><span data-stu-id="546ef-619">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="546ef-620">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-620">bluetoothBlocked</span></span>|<span data-ttu-id="546ef-621">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-621">Boolean</span></span>|<span data-ttu-id="546ef-622">ユーザーが Bluetooth を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-622">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="546ef-623">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-623">cameraBlocked</span></span>|<span data-ttu-id="546ef-624">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-624">Boolean</span></span>|<span data-ttu-id="546ef-625">ユーザーがデバイスのカメラにアクセスすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-625">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="546ef-626">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-626">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="546ef-627">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-627">Boolean</span></span>|<span data-ttu-id="546ef-628">他のデバイスの検出と接続、リモート メッセージング、リモート アプリ セッション、その他のデバイス間エクスペリエンスを可能にする、接続されているデバイスのサービスを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-628">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="546ef-629">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="546ef-629">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="546ef-630">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-630">Boolean</span></span>|<span data-ttu-id="546ef-631">ユーザーが手動でルート証明書をインストールすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-631">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="546ef-632">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-632">copyPasteBlocked</span></span>|<span data-ttu-id="546ef-633">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-633">Boolean</span></span>|<span data-ttu-id="546ef-634">ユーザーがコピーと貼り付けを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-634">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="546ef-635">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-635">cortanaBlocked</span></span>|<span data-ttu-id="546ef-636">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-636">Boolean</span></span>|<span data-ttu-id="546ef-637">ユーザーが Cortana を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="546ef-637">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="546ef-638">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="546ef-638">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="546ef-639">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-639">Boolean</span></span>|<span data-ttu-id="546ef-640">ユーザーが携帯電話をリセットすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-640">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="546ef-641">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="546ef-641">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="546ef-642">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-642">Boolean</span></span>|<span data-ttu-id="546ef-643">ユーザーがデバイス管理から手動で登録解除を行うことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-643">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="546ef-644">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="546ef-644">safeSearchFilter</span></span>|[<span data-ttu-id="546ef-645">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="546ef-645">safeSearchFilterType</span></span>](../resources/intune_deviceconfig_safesearchfiltertype.md)|<span data-ttu-id="546ef-p150">安全な検索が必要なフィルター レベルを指定します。可能な値は、  `userDefined`、 `strict`、 `moderate` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p150">Specifies what filter level of safe search is required. The possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="546ef-648">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="546ef-648">edgeBlockPopups</span></span>|<span data-ttu-id="546ef-649">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-649">Boolean</span></span>|<span data-ttu-id="546ef-650">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-650">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="546ef-651">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="546ef-651">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="546ef-652">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-652">Boolean</span></span>|<span data-ttu-id="546ef-653">ユーザーがアドレス バーで検索候補を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-653">Indicates whether or not to Block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="546ef-654">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="546ef-654">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="546ef-655">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-655">Boolean</span></span>|<span data-ttu-id="546ef-656">ユーザーが Edge から Internet Explorer にイントラネット トラフィックを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-656">Indicates whether or not to Block the user from sending Intranet traffic to Internet Explorer from Edge.</span></span>|
|<span data-ttu-id="546ef-657">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="546ef-657">edgeRequireSmartScreen</span></span>|<span data-ttu-id="546ef-658">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-658">Boolean</span></span>|<span data-ttu-id="546ef-659">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-659">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="546ef-660">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="546ef-660">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="546ef-661">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-661">String</span></span>|<span data-ttu-id="546ef-662">エンタープライズ モードのサイト リストの場所を示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-662">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="546ef-663">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="546ef-663">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="546ef-664">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="546ef-664">edgeFirstRunUrl</span></span>|<span data-ttu-id="546ef-665">文字列</span><span class="sxs-lookup"><span data-stu-id="546ef-665">String</span></span>|<span data-ttu-id="546ef-666">Edge ブラウザーを初めて開いたときに最初に実行される URL です。</span><span class="sxs-lookup"><span data-stu-id="546ef-666">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="546ef-667">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="546ef-667">edgeSearchEngine</span></span>|[<span data-ttu-id="546ef-668">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="546ef-668">edgeSearchEngineBase</span></span>](../resources/intune_deviceconfig_edgesearchenginebase.md)|<span data-ttu-id="546ef-669">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="546ef-669">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="546ef-670">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="546ef-670">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="546ef-671">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="546ef-671">edgeHomepageUrls</span></span>|<span data-ttu-id="546ef-672">String コレクション</span><span class="sxs-lookup"><span data-stu-id="546ef-672">String collection</span></span>|<span data-ttu-id="546ef-673">MDM に登録されているデバイスの Edge ブラウザーに表示されるホームページの URL の一覧です。</span><span class="sxs-lookup"><span data-stu-id="546ef-673">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="546ef-674">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="546ef-674">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="546ef-675">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-675">Boolean</span></span>|<span data-ttu-id="546ef-676">Edge ブラウザーの about:flags へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-676">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="546ef-677">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="546ef-677">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="546ef-678">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-678">Boolean</span></span>|<span data-ttu-id="546ef-679">悪意のある Web サイトの可能性があるサイトに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-679">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="546ef-680">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="546ef-680">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="546ef-681">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-681">Boolean</span></span>|<span data-ttu-id="546ef-682">未検証のファイルのダウンロードに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="546ef-682">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="546ef-683">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="546ef-683">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="546ef-684">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-684">Boolean</span></span>|<span data-ttu-id="546ef-685">WebRTC を使用して通話を発信しているときにユーザーのローカル ホストの IP アドレスが表示されるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="546ef-685">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="546ef-686">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-686">internetSharingBlocked</span></span>|<span data-ttu-id="546ef-687">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-687">Boolean</span></span>|<span data-ttu-id="546ef-688">ユーザーがインターネット共有を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-688">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="546ef-689">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="546ef-689">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="546ef-690">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-690">Boolean</span></span>|<span data-ttu-id="546ef-691">ユーザーがプロビジョニング パッケージをインストールすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-691">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="546ef-692">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="546ef-692">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="546ef-693">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-693">Boolean</span></span>|<span data-ttu-id="546ef-694">ランタイム構成エージェントがプロビジョニング パッケージを削除することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-694">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="546ef-695">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="546ef-695">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="546ef-696">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-696">Boolean</span></span>|<span data-ttu-id="546ef-697">ユーザーが日付と時刻の設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-697">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="546ef-698">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="546ef-698">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="546ef-699">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-699">Boolean</span></span>|<span data-ttu-id="546ef-700">ユーザーがデバイス名を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-700">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="546ef-701">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="546ef-701">settingsBlockChangeRegion</span></span>|<span data-ttu-id="546ef-702">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-702">Boolean</span></span>|<span data-ttu-id="546ef-703">ユーザーがリージョン設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-703">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="546ef-704">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="546ef-704">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="546ef-705">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-705">Boolean</span></span>|<span data-ttu-id="546ef-706">ユーザーが言語の設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-706">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="546ef-707">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="546ef-707">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="546ef-708">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-708">Boolean</span></span>|<span data-ttu-id="546ef-709">ユーザーが電源とスリープの設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-709">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="546ef-710">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-710">locationServicesBlocked</span></span>|<span data-ttu-id="546ef-711">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-711">Boolean</span></span>|<span data-ttu-id="546ef-712">ユーザーが位置情報サービスを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-712">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="546ef-713">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-713">microsoftAccountBlocked</span></span>|<span data-ttu-id="546ef-714">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-714">Boolean</span></span>|<span data-ttu-id="546ef-715">Microsoft アカウントを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-715">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="546ef-716">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="546ef-716">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="546ef-717">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-717">Boolean</span></span>|<span data-ttu-id="546ef-718">Microsoft アカウントの設定の同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-718">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="546ef-719">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-719">nfcBlocked</span></span>|<span data-ttu-id="546ef-720">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-720">Boolean</span></span>|<span data-ttu-id="546ef-721">ユーザーが近距離無線通信を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-721">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="546ef-722">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-722">resetProtectionModeBlocked</span></span>|<span data-ttu-id="546ef-723">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-723">Boolean</span></span>|<span data-ttu-id="546ef-724">ユーザーが保護モードをリセットすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-724">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="546ef-725">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-725">screenCaptureBlocked</span></span>|<span data-ttu-id="546ef-726">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-726">Boolean</span></span>|<span data-ttu-id="546ef-727">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-727">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="546ef-728">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="546ef-728">storageBlockRemovableStorage</span></span>|<span data-ttu-id="546ef-729">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-729">Boolean</span></span>|<span data-ttu-id="546ef-730">ユーザーがリムーバブル記憶域を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-730">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="546ef-731">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="546ef-731">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="546ef-732">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-732">Boolean</span></span>|<span data-ttu-id="546ef-733">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-733">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="546ef-734">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-734">usbBlocked</span></span>|<span data-ttu-id="546ef-735">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-735">Boolean</span></span>|<span data-ttu-id="546ef-736">ユーザーが USB 接続を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-736">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="546ef-737">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-737">voiceRecordingBlocked</span></span>|<span data-ttu-id="546ef-738">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-738">Boolean</span></span>|<span data-ttu-id="546ef-739">ユーザーが音声録音を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-739">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="546ef-740">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="546ef-740">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="546ef-741">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-741">Boolean</span></span>|<span data-ttu-id="546ef-742">Wi-Fi ホットスポットへの自動接続を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-742">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="546ef-743">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="546ef-743">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="546ef-744">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-744">wiFiBlocked</span></span>|<span data-ttu-id="546ef-745">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-745">Boolean</span></span>|<span data-ttu-id="546ef-746">ユーザーが Wi-Fi を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-746">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="546ef-747">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="546ef-747">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="546ef-748">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-748">Boolean</span></span>|<span data-ttu-id="546ef-749">ユーザーが Wi-Fi の手動構成を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-749">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="546ef-750">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="546ef-750">wiFiScanInterval</span></span>|<span data-ttu-id="546ef-751">Int32</span><span class="sxs-lookup"><span data-stu-id="546ef-751">Int32</span></span>|<span data-ttu-id="546ef-752">Wi-Fi ネットワークに対するデバイス スキャンの頻度を指定します。</span><span class="sxs-lookup"><span data-stu-id="546ef-752">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="546ef-753">サポートされている値は 1 から 500 まで、既定値は 100、500 は最低頻度です。</span><span class="sxs-lookup"><span data-stu-id="546ef-753">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="546ef-754">有効な値は 1 から 500 までです</span><span class="sxs-lookup"><span data-stu-id="546ef-754">Valid values 1 to 500</span></span>|
|<span data-ttu-id="546ef-755">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="546ef-755">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="546ef-756">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-756">Boolean</span></span>|<span data-ttu-id="546ef-757">他のデバイスがこの PC をプロジェクター用に検出することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-757">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="546ef-758">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="546ef-758">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="546ef-759">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-759">Boolean</span></span>|<span data-ttu-id="546ef-760">ワイヤレス ディスプレイ レシーバーからのユーザー入力を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-760">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="546ef-761">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="546ef-761">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="546ef-762">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-762">Boolean</span></span>|<span data-ttu-id="546ef-763">新しいデバイスがペアリングを開始するときに PIN が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-763">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="546ef-764">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-764">windowsStoreBlocked</span></span>|<span data-ttu-id="546ef-765">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-765">Boolean</span></span>|<span data-ttu-id="546ef-766">ユーザーが Windows ストアを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-766">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="546ef-767">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="546ef-767">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="546ef-768">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="546ef-768">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="546ef-p155">AppX パッケージが信頼できる証明書で署名されてからアプリケーションが読み込まれる側にできるかどうかを示します。可能な値は、 `notConfigured`、 `blocked`、 `allowed` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p155">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded. The possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="546ef-771">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="546ef-771">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="546ef-772">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-772">Boolean</span></span>|<span data-ttu-id="546ef-773">Windows ストアからのアプリの自動更新を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-773">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="546ef-774">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="546ef-774">developerUnlockSetting</span></span>|[<span data-ttu-id="546ef-775">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="546ef-775">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="546ef-p156">開発者によるロック解除を許可するかどうかを示します。可能な値は、 `notConfigured`, `blocked`, `allowed` です。</span><span class="sxs-lookup"><span data-stu-id="546ef-p156">Indicates whether or not to allow developer unlock. The possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="546ef-778">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="546ef-778">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="546ef-779">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-779">Boolean</span></span>|<span data-ttu-id="546ef-780">同じアプリの複数のユーザーによるデータ共有を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-780">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="546ef-781">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="546ef-781">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="546ef-782">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-782">Boolean</span></span>|<span data-ttu-id="546ef-783">プレインストールまたはダウンロードによって取得したすべての Windows ストア アプリの起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-783">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="546ef-784">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="546ef-784">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="546ef-785">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-785">Boolean</span></span>|<span data-ttu-id="546ef-786">プライベート ストアのみを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-786">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="546ef-787">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="546ef-787">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="546ef-788">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-788">Boolean</span></span>|<span data-ttu-id="546ef-789">アプリケーションのデータがシステム ドライブに制限されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-789">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="546ef-790">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="546ef-790">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="546ef-791">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-791">Boolean</span></span>|<span data-ttu-id="546ef-792">アプリケーションのインストールがシステム ドライブに制限されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-792">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="546ef-793">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="546ef-793">gameDvrBlocked</span></span>|<span data-ttu-id="546ef-794">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-794">Boolean</span></span>|<span data-ttu-id="546ef-795">DVR とブロードキャストを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-795">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="546ef-796">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="546ef-796">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="546ef-797">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-797">Boolean</span></span>|<span data-ttu-id="546ef-798">デバイス検出 UX を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-798">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="546ef-799">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="546ef-799">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="546ef-800">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-800">Boolean</span></span>|<span data-ttu-id="546ef-801">SIM カードが検出されない場合にエラー ダイアログを表示することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-801">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="546ef-802">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="546ef-802">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="546ef-803">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-803">Boolean</span></span>|<span data-ttu-id="546ef-804">デバイスでのタスクの切り替えを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546ef-804">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="546ef-805">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="546ef-805">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="546ef-806">ブール値</span><span class="sxs-lookup"><span data-stu-id="546ef-806">Boolean</span></span>|<span data-ttu-id="546ef-807">同時にログオンしているユーザー間での切り替えをログオフなしで迅速に行う機能を無効にします。</span><span class="sxs-lookup"><span data-stu-id="546ef-807">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|



## <a name="response"></a><span data-ttu-id="546ef-808">応答</span><span class="sxs-lookup"><span data-stu-id="546ef-808">Response</span></span>
<span data-ttu-id="546ef-809">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="546ef-809">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="546ef-810">例</span><span class="sxs-lookup"><span data-stu-id="546ef-810">Example</span></span>
### <a name="request"></a><span data-ttu-id="546ef-811">要求</span><span class="sxs-lookup"><span data-stu-id="546ef-811">Request</span></span>
<span data-ttu-id="546ef-812">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="546ef-812">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9699

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```

### <a name="response"></a><span data-ttu-id="546ef-813">応答</span><span class="sxs-lookup"><span data-stu-id="546ef-813">Response</span></span>
<span data-ttu-id="546ef-p157">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="546ef-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9875

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```








