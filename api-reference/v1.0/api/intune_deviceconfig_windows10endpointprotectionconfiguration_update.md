# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="d2aa5-101">windows10EndpointProtectionConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d2aa5-101">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="d2aa5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2aa5-103">[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-103">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2aa5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2aa5-104">Prerequisites</span></span>
<span data-ttu-id="d2aa5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2aa5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2aa5-107">Permission type</span></span>|<span data-ttu-id="d2aa5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2aa5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2aa5-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2aa5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d2aa5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2aa5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2aa5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2aa5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2aa5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-112">Not supported.</span></span>|
|<span data-ttu-id="d2aa5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2aa5-113">Application</span></span>|<span data-ttu-id="d2aa5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2aa5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2aa5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d2aa5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2aa5-116">Request headers</span></span>
|<span data-ttu-id="d2aa5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2aa5-117">Header</span></span>|<span data-ttu-id="d2aa5-118">値</span><span class="sxs-lookup"><span data-stu-id="d2aa5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2aa5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2aa5-119">Authorization</span></span>|<span data-ttu-id="d2aa5-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2aa5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d2aa5-121">Accept</span></span>|<span data-ttu-id="d2aa5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d2aa5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2aa5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2aa5-123">Request body</span></span>
<span data-ttu-id="d2aa5-124">要求本文で、[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-124">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="d2aa5-125">次の表に、[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-125">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="d2aa5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2aa5-126">Property</span></span>|<span data-ttu-id="d2aa5-127">型</span><span class="sxs-lookup"><span data-stu-id="d2aa5-127">Type</span></span>|<span data-ttu-id="d2aa5-128">説明</span><span class="sxs-lookup"><span data-stu-id="d2aa5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2aa5-129">id</span><span class="sxs-lookup"><span data-stu-id="d2aa5-129">id</span></span>|<span data-ttu-id="d2aa5-130">String</span><span class="sxs-lookup"><span data-stu-id="d2aa5-130">String</span></span>|<span data-ttu-id="d2aa5-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-131">Key of the entity.</span></span> <span data-ttu-id="d2aa5-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2aa5-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2aa5-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d2aa5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2aa5-134">DateTimeOffset</span></span>|<span data-ttu-id="d2aa5-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-135">DateTime the object was last modified.</span></span> <span data-ttu-id="d2aa5-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2aa5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2aa5-137">createdDateTime</span></span>|<span data-ttu-id="d2aa5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2aa5-138">DateTimeOffset</span></span>|<span data-ttu-id="d2aa5-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-139">DateTime the object was created.</span></span> <span data-ttu-id="d2aa5-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2aa5-141">description</span><span class="sxs-lookup"><span data-stu-id="d2aa5-141">description</span></span>|<span data-ttu-id="d2aa5-142">String</span><span class="sxs-lookup"><span data-stu-id="d2aa5-142">String</span></span>|<span data-ttu-id="d2aa5-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d2aa5-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2aa5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d2aa5-145">displayName</span></span>|<span data-ttu-id="d2aa5-146">String</span><span class="sxs-lookup"><span data-stu-id="d2aa5-146">String</span></span>|<span data-ttu-id="d2aa5-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d2aa5-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2aa5-149">version</span><span class="sxs-lookup"><span data-stu-id="d2aa5-149">version</span></span>|<span data-ttu-id="d2aa5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d2aa5-150">Int32</span></span>|<span data-ttu-id="d2aa5-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-151">Version of the device configuration.</span></span> <span data-ttu-id="d2aa5-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2aa5-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="d2aa5-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="d2aa5-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-154">Boolean</span></span>|<span data-ttu-id="d2aa5-155">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="d2aa5-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="d2aa5-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="d2aa5-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="d2aa5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d2aa5-157">Int32</span></span>|<span data-ttu-id="d2aa5-158">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="d2aa5-159">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="d2aa5-160">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="d2aa5-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="d2aa5-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="d2aa5-161">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="d2aa5-162">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="d2aa5-162">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune_deviceconfig_firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="d2aa5-163">事前共有キーを使用するエンコーディングを選択します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-163">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="d2aa5-164">可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-164">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="d2aa5-165">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="d2aa5-165">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="d2aa5-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-166">Boolean</span></span>|<span data-ttu-id="d2aa5-167">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-167">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d2aa5-168">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="d2aa5-168">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="d2aa5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-169">Boolean</span></span>|<span data-ttu-id="d2aa5-170">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-170">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="d2aa5-171">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="d2aa5-171">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="d2aa5-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-172">Boolean</span></span>|<span data-ttu-id="d2aa5-173">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-173">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d2aa5-174">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="d2aa5-174">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="d2aa5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-175">Boolean</span></span>|<span data-ttu-id="d2aa5-176">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-176">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="d2aa5-177">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="d2aa5-177">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="d2aa5-178">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="d2aa5-178">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune_deviceconfig_firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="d2aa5-179">証明書失効リストを適用する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-179">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="d2aa5-180">可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-180">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="d2aa5-181">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="d2aa5-181">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="d2aa5-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-182">Boolean</span></span>|<span data-ttu-id="d2aa5-183">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-183">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="d2aa5-184">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="d2aa5-184">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="d2aa5-185">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="d2aa5-185">firewallPacketQueueingMethodType</span></span>](../resources/intune_deviceconfig_firewallpacketqueueingmethodtype.md)|<span data-ttu-id="d2aa5-186">トンネルのゲートウェイでパケットのキューイングを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-186">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="d2aa5-187">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-187">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="d2aa5-188">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="d2aa5-188">firewallProfileDomain</span></span>|[<span data-ttu-id="d2aa5-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d2aa5-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="d2aa5-190">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-190">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="d2aa5-191">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="d2aa5-191">firewallProfilePublic</span></span>|[<span data-ttu-id="d2aa5-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d2aa5-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="d2aa5-193">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-193">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="d2aa5-194">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="d2aa5-194">firewallProfilePrivate</span></span>|[<span data-ttu-id="d2aa5-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d2aa5-195">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="d2aa5-196">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-196">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="d2aa5-197">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="d2aa5-197">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="d2aa5-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d2aa5-198">String collection</span></span>|<span data-ttu-id="d2aa5-199">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="d2aa5-199">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="d2aa5-200">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="d2aa5-200">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="d2aa5-201">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d2aa5-201">String collection</span></span>|<span data-ttu-id="d2aa5-202">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="d2aa5-202">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="d2aa5-203">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="d2aa5-203">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="d2aa5-204">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d2aa5-204">String collection</span></span>|<span data-ttu-id="d2aa5-205">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="d2aa5-205">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="d2aa5-206">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="d2aa5-206">defenderExploitProtectionXml</span></span>|<span data-ttu-id="d2aa5-207">Binary</span><span class="sxs-lookup"><span data-stu-id="d2aa5-207">Binary</span></span>|<span data-ttu-id="d2aa5-208">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-208">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="d2aa5-209">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="d2aa5-209">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="d2aa5-210">String</span><span class="sxs-lookup"><span data-stu-id="d2aa5-210">String</span></span>|<span data-ttu-id="d2aa5-211">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-211">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="d2aa5-212">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="d2aa5-212">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="d2aa5-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-213">Boolean</span></span>|<span data-ttu-id="d2aa5-214">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-214">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="d2aa5-215">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="d2aa5-215">appLockerApplicationControl</span></span>|[<span data-ttu-id="d2aa5-216">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="d2aa5-216">appLockerApplicationControlType</span></span>](../resources/intune_deviceconfig_applockerapplicationcontroltype.md)|<span data-ttu-id="d2aa5-217">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-217">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="d2aa5-218">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-218">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="d2aa5-219">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="d2aa5-219">smartScreenEnableInShell</span></span>|<span data-ttu-id="d2aa5-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-220">Boolean</span></span>|<span data-ttu-id="d2aa5-221">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-221">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="d2aa5-222">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="d2aa5-222">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="d2aa5-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-223">Boolean</span></span>|<span data-ttu-id="d2aa5-224">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-224">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="d2aa5-225">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="d2aa5-225">applicationGuardEnabled</span></span>|<span data-ttu-id="d2aa5-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-226">Boolean</span></span>|<span data-ttu-id="d2aa5-227">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="d2aa5-227">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="d2aa5-228">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="d2aa5-228">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="d2aa5-229">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="d2aa5-229">applicationGuardBlockFileTransferType</span></span>](../resources/intune_deviceconfig_applicationguardblockfiletransfertype.md)|<span data-ttu-id="d2aa5-230">イメージ ファイルの転送、テキスト ファイルのいずれかにクリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-230">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="d2aa5-231">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-231">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="d2aa5-232">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="d2aa5-232">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="d2aa5-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-233">Boolean</span></span>|<span data-ttu-id="d2aa5-234">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="d2aa5-234">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="d2aa5-235">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="d2aa5-235">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="d2aa5-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-236">Boolean</span></span>|<span data-ttu-id="d2aa5-237">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-237">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="d2aa5-238">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="d2aa5-238">applicationGuardForceAuditing</span></span>|<span data-ttu-id="d2aa5-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-239">Boolean</span></span>|<span data-ttu-id="d2aa5-240">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="d2aa5-240">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="d2aa5-241">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="d2aa5-241">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="d2aa5-242">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="d2aa5-242">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune_deviceconfig_applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="d2aa5-243">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-243">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="d2aa5-244">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-244">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="d2aa5-245">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="d2aa5-245">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="d2aa5-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-246">Boolean</span></span>|<span data-ttu-id="d2aa5-247">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-247">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="d2aa5-248">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="d2aa5-248">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="d2aa5-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-249">Boolean</span></span>|<span data-ttu-id="d2aa5-250">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-250">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="d2aa5-251">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="d2aa5-251">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="d2aa5-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-252">Boolean</span></span>|<span data-ttu-id="d2aa5-253">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-253">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="d2aa5-254">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="d2aa5-254">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="d2aa5-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-255">Boolean</span></span>|<span data-ttu-id="d2aa5-256">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="d2aa5-256">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="d2aa5-257">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="d2aa5-257">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="d2aa5-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-258">Boolean</span></span>|<span data-ttu-id="d2aa5-259">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-259">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="d2aa5-260">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="d2aa5-260">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="d2aa5-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-261">Boolean</span></span>|<span data-ttu-id="d2aa5-262">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="d2aa5-263">このポリシーは、モバイルの SKU に対してのみ有効です。
</span><span class="sxs-lookup"><span data-stu-id="d2aa5-263">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="d2aa5-264">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="d2aa5-264">bitLockerEncryptDevice</span></span>|<span data-ttu-id="d2aa5-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2aa5-265">Boolean</span></span>|<span data-ttu-id="d2aa5-266">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-266">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="d2aa5-267">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d2aa5-267">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="d2aa5-268">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d2aa5-268">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="d2aa5-269">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-269">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="d2aa5-270">応答</span><span class="sxs-lookup"><span data-stu-id="d2aa5-270">Response</span></span>
<span data-ttu-id="d2aa5-271">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-271">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2aa5-272">例</span><span class="sxs-lookup"><span data-stu-id="d2aa5-272">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2aa5-273">要求</span><span class="sxs-lookup"><span data-stu-id="d2aa5-273">Request</span></span>
<span data-ttu-id="d2aa5-274">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-274">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4245

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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

### <a name="response"></a><span data-ttu-id="d2aa5-275">応答</span><span class="sxs-lookup"><span data-stu-id="d2aa5-275">Response</span></span>
<span data-ttu-id="d2aa5-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2aa5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



