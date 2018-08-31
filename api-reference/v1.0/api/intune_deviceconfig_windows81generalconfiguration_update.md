# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="60f26-101">windows81GeneralConfiguration を更新</span><span class="sxs-lookup"><span data-stu-id="60f26-101">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="60f26-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="60f26-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60f26-103">[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="60f26-103">Update the properties of a [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60f26-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="60f26-104">Prerequisites</span></span>
<span data-ttu-id="60f26-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="60f26-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60f26-107">Permission type</span></span>|<span data-ttu-id="60f26-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="60f26-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60f26-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60f26-109">Delegated (work or school account)</span></span>|<span data-ttu-id="60f26-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60f26-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60f26-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60f26-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60f26-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60f26-112">Not supported.</span></span>|
|<span data-ttu-id="60f26-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60f26-113">Application</span></span>|<span data-ttu-id="60f26-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60f26-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60f26-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60f26-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="60f26-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60f26-116">Request headers</span></span>
|<span data-ttu-id="60f26-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60f26-117">Header</span></span>|<span data-ttu-id="60f26-118">値</span><span class="sxs-lookup"><span data-stu-id="60f26-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60f26-119">承認</span><span class="sxs-lookup"><span data-stu-id="60f26-119">Authorization</span></span>|<span data-ttu-id="60f26-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="60f26-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60f26-121">承諾</span><span class="sxs-lookup"><span data-stu-id="60f26-121">Accept</span></span>|<span data-ttu-id="60f26-122">application/json</span><span class="sxs-lookup"><span data-stu-id="60f26-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60f26-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="60f26-123">Request body</span></span>
<span data-ttu-id="60f26-124">要求本文で、[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="60f26-124">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="60f26-125">次の表に、[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-125">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="60f26-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60f26-126">Property</span></span>|<span data-ttu-id="60f26-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="60f26-127">Type</span></span>|<span data-ttu-id="60f26-128">説明</span><span class="sxs-lookup"><span data-stu-id="60f26-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60f26-129">id</span><span class="sxs-lookup"><span data-stu-id="60f26-129">id</span></span>|<span data-ttu-id="60f26-130">文字列</span><span class="sxs-lookup"><span data-stu-id="60f26-130">String</span></span>|<span data-ttu-id="60f26-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="60f26-131">Key of the entity.</span></span> <span data-ttu-id="60f26-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="60f26-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60f26-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60f26-133">lastModifiedDateTime</span></span>|<span data-ttu-id="60f26-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60f26-134">DateTimeOffset</span></span>|<span data-ttu-id="60f26-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="60f26-135">DateTime the object was last modified.</span></span> <span data-ttu-id="60f26-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="60f26-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60f26-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60f26-137">createdDateTime</span></span>|<span data-ttu-id="60f26-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60f26-138">DateTimeOffset</span></span>|<span data-ttu-id="60f26-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="60f26-139">DateTime the object was created.</span></span> <span data-ttu-id="60f26-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="60f26-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60f26-141">description</span><span class="sxs-lookup"><span data-stu-id="60f26-141">description</span></span>|<span data-ttu-id="60f26-142">String</span><span class="sxs-lookup"><span data-stu-id="60f26-142">String</span></span>|<span data-ttu-id="60f26-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="60f26-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="60f26-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="60f26-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60f26-145">displayName</span><span class="sxs-lookup"><span data-stu-id="60f26-145">displayName</span></span>|<span data-ttu-id="60f26-146">String</span><span class="sxs-lookup"><span data-stu-id="60f26-146">String</span></span>|<span data-ttu-id="60f26-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="60f26-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="60f26-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="60f26-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60f26-149">version</span><span class="sxs-lookup"><span data-stu-id="60f26-149">version</span></span>|<span data-ttu-id="60f26-150">Int32</span><span class="sxs-lookup"><span data-stu-id="60f26-150">Int32</span></span>|<span data-ttu-id="60f26-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="60f26-151">Version of the device configuration.</span></span> <span data-ttu-id="60f26-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="60f26-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60f26-153">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="60f26-153">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="60f26-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-154">Boolean</span></span>|<span data-ttu-id="60f26-155">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-155">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="60f26-156">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="60f26-156">applyOnlyToWindows81</span></span>|<span data-ttu-id="60f26-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-157">Boolean</span></span>|<span data-ttu-id="60f26-158">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="60f26-158">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="60f26-159">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="60f26-159">This property is read-only.</span></span>|
|<span data-ttu-id="60f26-160">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="60f26-160">browserBlockAutofill</span></span>|<span data-ttu-id="60f26-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-161">Boolean</span></span>|<span data-ttu-id="60f26-162">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-162">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="60f26-163">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="60f26-163">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="60f26-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-164">Boolean</span></span>|<span data-ttu-id="60f26-165">イントラネット サイトの自動検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-165">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="60f26-166">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="60f26-166">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="60f26-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-167">Boolean</span></span>|<span data-ttu-id="60f26-168">エンタープライズ モードのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-168">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="60f26-169">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="60f26-169">browserBlockJavaScript</span></span>|<span data-ttu-id="60f26-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-170">Boolean</span></span>|<span data-ttu-id="60f26-171">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-171">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="60f26-172">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="60f26-172">browserBlockPlugins</span></span>|<span data-ttu-id="60f26-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-173">Boolean</span></span>|<span data-ttu-id="60f26-174">プラグインを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-174">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="60f26-175">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="60f26-175">browserBlockPopups</span></span>|<span data-ttu-id="60f26-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-176">Boolean</span></span>|<span data-ttu-id="60f26-177">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-177">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="60f26-178">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="60f26-178">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="60f26-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-179">Boolean</span></span>|<span data-ttu-id="60f26-180">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-180">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="60f26-181">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="60f26-181">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="60f26-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-182">Boolean</span></span>|<span data-ttu-id="60f26-183">イントラネット サイトでの 1 単語のエントリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-183">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="60f26-184">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="60f26-184">browserRequireSmartScreen</span></span>|<span data-ttu-id="60f26-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-185">Boolean</span></span>|<span data-ttu-id="60f26-186">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-186">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="60f26-187">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="60f26-187">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="60f26-188">String</span><span class="sxs-lookup"><span data-stu-id="60f26-188">String</span></span>|<span data-ttu-id="60f26-189">エンタープライズ モードのサイト リストの場所。</span><span class="sxs-lookup"><span data-stu-id="60f26-189">The enterprise mode site list location.</span></span> <span data-ttu-id="60f26-190">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="60f26-190">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="60f26-191">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="60f26-191">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="60f26-192">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="60f26-192">internetSiteSecurityLevel</span></span>](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|<span data-ttu-id="60f26-193">インターネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="60f26-193">The internet security level.</span></span> <span data-ttu-id="60f26-194">可能な値は、`userDefined`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="60f26-194">The possible values are `userDefined`, `medium`, `mediumHigh`, `high`, , , , , , , , or .</span></span>|
|<span data-ttu-id="60f26-195">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="60f26-195">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="60f26-196">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="60f26-196">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="60f26-197">イントラネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="60f26-197">The Intranet security level.</span></span> <span data-ttu-id="60f26-198">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="60f26-198">The possible values are `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`, , , , , , or .</span></span>|
|<span data-ttu-id="60f26-199">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="60f26-199">browserLoggingReportLocation</span></span>|<span data-ttu-id="60f26-200">String</span><span class="sxs-lookup"><span data-stu-id="60f26-200">String</span></span>|<span data-ttu-id="60f26-201">ログ レポートの場所。</span><span class="sxs-lookup"><span data-stu-id="60f26-201">The logging report location.</span></span>|
|<span data-ttu-id="60f26-202">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="60f26-202">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="60f26-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-203">Boolean</span></span>|<span data-ttu-id="60f26-204">制限付きサイトに対する高度なセキュリティを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-204">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="60f26-205">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="60f26-205">browserRequireFirewall</span></span>|<span data-ttu-id="60f26-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-206">Boolean</span></span>|<span data-ttu-id="60f26-207">ファイアウォールが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-207">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="60f26-208">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="60f26-208">browserRequireFraudWarning</span></span>|<span data-ttu-id="60f26-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-209">Boolean</span></span>|<span data-ttu-id="60f26-210">不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-210">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="60f26-211">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="60f26-211">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="60f26-212">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="60f26-212">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="60f26-213">信頼済みサイトのセキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="60f26-213">The trusted sites security level.</span></span> <span data-ttu-id="60f26-214">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="60f26-214">The possible values are `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`, , , , , , or .</span></span>|
|<span data-ttu-id="60f26-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="60f26-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="60f26-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-216">Boolean</span></span>|<span data-ttu-id="60f26-217">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="60f26-218">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="60f26-218">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="60f26-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-219">Boolean</span></span>|<span data-ttu-id="60f26-220">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-220">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="60f26-221">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="60f26-221">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="60f26-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-222">Boolean</span></span>|<span data-ttu-id="60f26-223">ユーザーがピクチャ パスワードおよび暗証番号 (PIN) を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-223">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="60f26-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="60f26-224">passwordExpirationDays</span></span>|<span data-ttu-id="60f26-225">Int32</span><span class="sxs-lookup"><span data-stu-id="60f26-225">Int32</span></span>|<span data-ttu-id="60f26-226">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="60f26-226">Password expiration in days.</span></span>|
|<span data-ttu-id="60f26-227">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="60f26-227">passwordMinimumLength</span></span>|<span data-ttu-id="60f26-228">Int32</span><span class="sxs-lookup"><span data-stu-id="60f26-228">Int32</span></span>|<span data-ttu-id="60f26-229">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="60f26-229">The minimum password length.</span></span>|
|<span data-ttu-id="60f26-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="60f26-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="60f26-231">Int32</span><span class="sxs-lookup"><span data-stu-id="60f26-231">Int32</span></span>|<span data-ttu-id="60f26-232">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="60f26-232">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="60f26-233">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="60f26-233">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="60f26-234">Int32</span><span class="sxs-lookup"><span data-stu-id="60f26-234">Int32</span></span>|<span data-ttu-id="60f26-235">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="60f26-235">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="60f26-236">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="60f26-236">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="60f26-237">Int32</span><span class="sxs-lookup"><span data-stu-id="60f26-237">Int32</span></span>|<span data-ttu-id="60f26-238">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="60f26-238">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="60f26-239">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="60f26-239">Valid values 0 to 24</span></span>|
|<span data-ttu-id="60f26-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="60f26-240">passwordRequiredType</span></span>|[<span data-ttu-id="60f26-241">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="60f26-241">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="60f26-242">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="60f26-242">The required password type.</span></span> <span data-ttu-id="60f26-243">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="60f26-243">The possible values are `deviceDefault`, `alphanumeric`, or `numeric`.</span></span>|
|<span data-ttu-id="60f26-244">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="60f26-244">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="60f26-245">Int32</span><span class="sxs-lookup"><span data-stu-id="60f26-245">Int32</span></span>|<span data-ttu-id="60f26-246">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="60f26-246">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="60f26-247">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="60f26-247">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="60f26-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-248">Boolean</span></span>|<span data-ttu-id="60f26-249">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-249">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="60f26-250">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="60f26-250">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="60f26-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="60f26-251">Boolean</span></span>|<span data-ttu-id="60f26-252">自動更新が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60f26-252">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="60f26-253">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="60f26-253">userAccountControlSettings</span></span>|[<span data-ttu-id="60f26-254">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="60f26-254">windowsUserAccountControlSettings</span></span>](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|<span data-ttu-id="60f26-255">ユーザー アカウント制御の設定。</span><span class="sxs-lookup"><span data-stu-id="60f26-255">The user account control settings.</span></span> <span data-ttu-id="60f26-256">可能な値は、`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify` です。</span><span class="sxs-lookup"><span data-stu-id="60f26-256">The possible values are `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`, , , , , , , or .</span></span>|
|<span data-ttu-id="60f26-257">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="60f26-257">workFoldersUrl</span></span>|<span data-ttu-id="60f26-258">String</span><span class="sxs-lookup"><span data-stu-id="60f26-258">String</span></span>|<span data-ttu-id="60f26-259">作業フォルダーの URL。</span><span class="sxs-lookup"><span data-stu-id="60f26-259">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="60f26-260">応答</span><span class="sxs-lookup"><span data-stu-id="60f26-260">Response</span></span>
<span data-ttu-id="60f26-261">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="60f26-261">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60f26-262">例</span><span class="sxs-lookup"><span data-stu-id="60f26-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="60f26-263">要求</span><span class="sxs-lookup"><span data-stu-id="60f26-263">Request</span></span>
<span data-ttu-id="60f26-264">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60f26-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1689

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="60f26-265">応答</span><span class="sxs-lookup"><span data-stu-id="60f26-265">Response</span></span>
<span data-ttu-id="60f26-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60f26-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```



