# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="fe00e-101">windows10EndpointProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="fe00e-101">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="fe00e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe00e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe00e-103">新しい [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe00e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="fe00e-104">Prerequisites</span></span>
<span data-ttu-id="fe00e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe00e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe00e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe00e-107">Permission type</span></span>|<span data-ttu-id="fe00e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe00e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe00e-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe00e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fe00e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe00e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe00e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe00e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe00e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe00e-112">Not supported.</span></span>|
|<span data-ttu-id="fe00e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe00e-113">Application</span></span>|<span data-ttu-id="fe00e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe00e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe00e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe00e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fe00e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe00e-116">Request headers</span></span>
|<span data-ttu-id="fe00e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe00e-117">Header</span></span>|<span data-ttu-id="fe00e-118">値</span><span class="sxs-lookup"><span data-stu-id="fe00e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe00e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe00e-119">Authorization</span></span>|<span data-ttu-id="fe00e-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fe00e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fe00e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fe00e-121">Accept</span></span>|<span data-ttu-id="fe00e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fe00e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe00e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe00e-123">Request body</span></span>
<span data-ttu-id="fe00e-124">要求本文で、windows10EndpointProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="fe00e-125">次の表に、windows10EndpointProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="fe00e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe00e-126">Property</span></span>|<span data-ttu-id="fe00e-127">型</span><span class="sxs-lookup"><span data-stu-id="fe00e-127">Type</span></span>|<span data-ttu-id="fe00e-128">説明</span><span class="sxs-lookup"><span data-stu-id="fe00e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe00e-129">id</span><span class="sxs-lookup"><span data-stu-id="fe00e-129">id</span></span>|<span data-ttu-id="fe00e-130">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-130">String</span></span>|<span data-ttu-id="fe00e-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fe00e-131">Name of the entity.</span></span> <span data-ttu-id="fe00e-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe00e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe00e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe00e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fe00e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe00e-134">DateTimeOffset</span></span>|<span data-ttu-id="fe00e-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fe00e-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="fe00e-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe00e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe00e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe00e-137">createdDateTime</span></span>|<span data-ttu-id="fe00e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe00e-138">DateTimeOffset</span></span>|<span data-ttu-id="fe00e-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fe00e-139">DateTime the object was created.</span></span> <span data-ttu-id="fe00e-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe00e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe00e-141">description</span><span class="sxs-lookup"><span data-stu-id="fe00e-141">description</span></span>|<span data-ttu-id="fe00e-142">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-142">String</span></span>|<span data-ttu-id="fe00e-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="fe00e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe00e-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe00e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe00e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fe00e-145">displayName</span></span>|<span data-ttu-id="fe00e-146">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-146">String</span></span>|<span data-ttu-id="fe00e-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="fe00e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe00e-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe00e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe00e-149">version</span><span class="sxs-lookup"><span data-stu-id="fe00e-149">version</span></span>|<span data-ttu-id="fe00e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fe00e-150">Int32</span></span>|<span data-ttu-id="fe00e-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="fe00e-151">Version of the device configuration.</span></span> <span data-ttu-id="fe00e-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe00e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe00e-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="fe00e-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="fe00e-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-154">Boolean</span></span>|<span data-ttu-id="fe00e-155">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="fe00e-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="fe00e-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="fe00e-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="fe00e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="fe00e-157">Int32</span></span>|<span data-ttu-id="fe00e-158">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="fe00e-159">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="fe00e-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="fe00e-160">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="fe00e-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="fe00e-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="fe00e-161">firewallPreSharedKeyEncodingMethod</span></span>|<span data-ttu-id="fe00e-162">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-162">String</span></span>|<span data-ttu-id="fe00e-163">使用する事前共有キーのエンコードを選択します。可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="fe00e-163">Select the preshared key encoding to be used Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="fe00e-164">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="fe00e-164">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="fe00e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-165">Boolean</span></span>|<span data-ttu-id="fe00e-166">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-166">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="fe00e-167">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="fe00e-167">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="fe00e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-168">Boolean</span></span>|<span data-ttu-id="fe00e-169">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-169">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="fe00e-170">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="fe00e-170">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="fe00e-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-171">Boolean</span></span>|<span data-ttu-id="fe00e-172">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-172">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="fe00e-173">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="fe00e-173">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="fe00e-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-174">Boolean</span></span>|<span data-ttu-id="fe00e-175">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-175">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="fe00e-176">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="fe00e-176">firewallCertificateRevocationListCheckMethod</span></span>|<span data-ttu-id="fe00e-177">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-177">String</span></span>|<span data-ttu-id="fe00e-178">証明書失効リストの実施方法を指定します。可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="fe00e-178">Specify how the certificate revocation list is to be enforced Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="fe00e-179">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="fe00e-179">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="fe00e-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-180">Boolean</span></span>|<span data-ttu-id="fe00e-181">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="fe00e-181">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="fe00e-182">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="fe00e-182">firewallPacketQueueingMethod</span></span>|<span data-ttu-id="fe00e-183">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-183">String</span></span>|<span data-ttu-id="fe00e-184">トンネル ゲートウェイのシナリオでパケットのキューを適用する方法を構成します。可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="fe00e-184">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="fe00e-185">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="fe00e-185">firewallProfileDomain</span></span>|[<span data-ttu-id="fe00e-186">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="fe00e-186">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="fe00e-187">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="fe00e-187">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="fe00e-188">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="fe00e-188">firewallProfilePublic</span></span>|[<span data-ttu-id="fe00e-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="fe00e-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="fe00e-190">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="fe00e-190">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="fe00e-191">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="fe00e-191">firewallProfilePrivate</span></span>|[<span data-ttu-id="fe00e-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="fe00e-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="fe00e-193">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="fe00e-193">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="fe00e-194">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="fe00e-194">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="fe00e-195">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fe00e-195">String collection</span></span>|<span data-ttu-id="fe00e-196">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="fe00e-196">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="fe00e-197">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="fe00e-197">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="fe00e-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fe00e-198">String collection</span></span>|<span data-ttu-id="fe00e-199">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="fe00e-199">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="fe00e-200">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="fe00e-200">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="fe00e-201">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fe00e-201">String collection</span></span>|<span data-ttu-id="fe00e-202">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="fe00e-202">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="fe00e-203">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="fe00e-203">defenderExploitProtectionXml</span></span>|<span data-ttu-id="fe00e-204">Binary</span><span class="sxs-lookup"><span data-stu-id="fe00e-204">Binary</span></span>|<span data-ttu-id="fe00e-205">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="fe00e-205">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="fe00e-206">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="fe00e-206">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="fe00e-207">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-207">String</span></span>|<span data-ttu-id="fe00e-208">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="fe00e-208">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="fe00e-209">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="fe00e-209">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="fe00e-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-210">Boolean</span></span>|<span data-ttu-id="fe00e-211">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-211">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="fe00e-212">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="fe00e-212">appLockerApplicationControl</span></span>|<span data-ttu-id="fe00e-213">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-213">String</span></span>|<span data-ttu-id="fe00e-214">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="fe00e-214">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="fe00e-215">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="fe00e-215">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="fe00e-216">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="fe00e-216">smartScreenEnableInShell</span></span>|<span data-ttu-id="fe00e-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-217">Boolean</span></span>|<span data-ttu-id="fe00e-218">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-218">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="fe00e-219">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="fe00e-219">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="fe00e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-220">Boolean</span></span>|<span data-ttu-id="fe00e-221">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-221">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="fe00e-222">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="fe00e-222">applicationGuardEnabled</span></span>|<span data-ttu-id="fe00e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-223">Boolean</span></span>|<span data-ttu-id="fe00e-224">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="fe00e-224">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="fe00e-225">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="fe00e-225">applicationGuardBlockFileTransfer</span></span>|<span data-ttu-id="fe00e-226">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-226">String</span></span>|<span data-ttu-id="fe00e-227">クリップボードへの画像ファイルまたはテキスト ファイルの転送をブロックします。あるいは、どちらもブロックしません。可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="fe00e-227">Block clipboard to transfer image file, text file or neither of them Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="fe00e-228">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="fe00e-228">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="fe00e-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-229">Boolean</span></span>|<span data-ttu-id="fe00e-230">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="fe00e-230">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="fe00e-231">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="fe00e-231">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="fe00e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-232">Boolean</span></span>|<span data-ttu-id="fe00e-233">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-233">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="fe00e-234">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="fe00e-234">applicationGuardForceAuditing</span></span>|<span data-ttu-id="fe00e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-235">Boolean</span></span>|<span data-ttu-id="fe00e-236">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="fe00e-236">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="fe00e-237">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="fe00e-237">applicationGuardBlockClipboardSharing</span></span>|<span data-ttu-id="fe00e-238">String</span><span class="sxs-lookup"><span data-stu-id="fe00e-238">String</span></span>|<span data-ttu-id="fe00e-239">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="fe00e-239">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="fe00e-240">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="fe00e-240">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="fe00e-241">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="fe00e-241">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="fe00e-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-242">Boolean</span></span>|<span data-ttu-id="fe00e-243">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-243">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="fe00e-244">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="fe00e-244">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="fe00e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-245">Boolean</span></span>|<span data-ttu-id="fe00e-246">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-246">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="fe00e-247">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="fe00e-247">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="fe00e-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-248">Boolean</span></span>|<span data-ttu-id="fe00e-249">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-249">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="fe00e-250">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="fe00e-250">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="fe00e-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-251">Boolean</span></span>|<span data-ttu-id="fe00e-252">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="fe00e-252">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="fe00e-253">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="fe00e-253">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="fe00e-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-254">Boolean</span></span>|<span data-ttu-id="fe00e-255">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-255">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="fe00e-256">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="fe00e-256">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="fe00e-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-257">Boolean</span></span>|<span data-ttu-id="fe00e-258">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-258">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="fe00e-259">このポリシーは、モバイルの SKU に対してのみ有効です。
</span><span class="sxs-lookup"><span data-stu-id="fe00e-259">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="fe00e-260">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="fe00e-260">bitLockerEncryptDevice</span></span>|<span data-ttu-id="fe00e-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe00e-261">Boolean</span></span>|<span data-ttu-id="fe00e-262">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="fe00e-263">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="fe00e-263">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="fe00e-264">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="fe00e-264">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="fe00e-265">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="fe00e-265">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="fe00e-266">応答</span><span class="sxs-lookup"><span data-stu-id="fe00e-266">Response</span></span>
<span data-ttu-id="fe00e-267">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fe00e-267">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe00e-268">例</span><span class="sxs-lookup"><span data-stu-id="fe00e-268">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe00e-269">要求</span><span class="sxs-lookup"><span data-stu-id="fe00e-269">Request</span></span>
<span data-ttu-id="fe00e-270">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe00e-270">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4309

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="fe00e-271">応答</span><span class="sxs-lookup"><span data-stu-id="fe00e-271">Response</span></span>
<span data-ttu-id="fe00e-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe00e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4417

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```



