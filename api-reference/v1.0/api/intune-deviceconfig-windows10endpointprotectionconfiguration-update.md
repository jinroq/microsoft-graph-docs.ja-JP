---
title: windows10EndpointProtectionConfiguration の更新
description: windows10EndpointProtectionConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 544c39eac05023937741bd5301912b4126d9bdde
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987679"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="3cc53-103">windows10EndpointProtectionConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="3cc53-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="3cc53-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cc53-105">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-105">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cc53-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3cc53-106">Prerequisites</span></span>
<span data-ttu-id="3cc53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cc53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cc53-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3cc53-109">Permission type</span></span>|<span data-ttu-id="3cc53-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3cc53-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cc53-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3cc53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3cc53-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cc53-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cc53-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3cc53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cc53-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cc53-114">Not supported.</span></span>|
|<span data-ttu-id="3cc53-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3cc53-115">Application</span></span>|<span data-ttu-id="3cc53-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cc53-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cc53-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3cc53-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3cc53-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cc53-118">Request headers</span></span>
|<span data-ttu-id="3cc53-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cc53-119">Header</span></span>|<span data-ttu-id="3cc53-120">値</span><span class="sxs-lookup"><span data-stu-id="3cc53-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cc53-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cc53-121">Authorization</span></span>|<span data-ttu-id="3cc53-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cc53-123">承諾</span><span class="sxs-lookup"><span data-stu-id="3cc53-123">Accept</span></span>|<span data-ttu-id="3cc53-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3cc53-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cc53-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3cc53-125">Request body</span></span>
<span data-ttu-id="3cc53-126">要求本文で、[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-126">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="3cc53-127">次の表に、[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-127">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="3cc53-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cc53-128">Property</span></span>|<span data-ttu-id="3cc53-129">型</span><span class="sxs-lookup"><span data-stu-id="3cc53-129">Type</span></span>|<span data-ttu-id="3cc53-130">説明</span><span class="sxs-lookup"><span data-stu-id="3cc53-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cc53-131">id</span><span class="sxs-lookup"><span data-stu-id="3cc53-131">id</span></span>|<span data-ttu-id="3cc53-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3cc53-132">String</span></span>|<span data-ttu-id="3cc53-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3cc53-133">Key of the entity.</span></span> <span data-ttu-id="3cc53-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cc53-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cc53-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cc53-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3cc53-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cc53-136">DateTimeOffset</span></span>|<span data-ttu-id="3cc53-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3cc53-137">DateTime the object was last modified.</span></span> <span data-ttu-id="3cc53-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cc53-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cc53-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cc53-139">createdDateTime</span></span>|<span data-ttu-id="3cc53-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cc53-140">DateTimeOffset</span></span>|<span data-ttu-id="3cc53-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3cc53-141">DateTime the object was created.</span></span> <span data-ttu-id="3cc53-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cc53-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cc53-143">description</span><span class="sxs-lookup"><span data-stu-id="3cc53-143">description</span></span>|<span data-ttu-id="3cc53-144">String</span><span class="sxs-lookup"><span data-stu-id="3cc53-144">String</span></span>|<span data-ttu-id="3cc53-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="3cc53-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3cc53-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cc53-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cc53-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3cc53-147">displayName</span></span>|<span data-ttu-id="3cc53-148">String</span><span class="sxs-lookup"><span data-stu-id="3cc53-148">String</span></span>|<span data-ttu-id="3cc53-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="3cc53-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3cc53-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cc53-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cc53-151">version</span><span class="sxs-lookup"><span data-stu-id="3cc53-151">version</span></span>|<span data-ttu-id="3cc53-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3cc53-152">Int32</span></span>|<span data-ttu-id="3cc53-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3cc53-153">Version of the device configuration.</span></span> <span data-ttu-id="3cc53-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cc53-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cc53-155">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="3cc53-155">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="3cc53-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-156">Boolean</span></span>|<span data-ttu-id="3cc53-157">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="3cc53-157">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="3cc53-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="3cc53-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="3cc53-159">Int32</span><span class="sxs-lookup"><span data-stu-id="3cc53-159">Int32</span></span>|<span data-ttu-id="3cc53-160">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-160">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="3cc53-161">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-161">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="3cc53-162">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="3cc53-162">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="3cc53-163">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="3cc53-163">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="3cc53-164">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="3cc53-164">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="3cc53-165">使用する事前共有キーのエンコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-165">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="3cc53-166">使用可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-166">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="3cc53-167">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="3cc53-167">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="3cc53-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-168">Boolean</span></span>|<span data-ttu-id="3cc53-169">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-169">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="3cc53-170">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="3cc53-170">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="3cc53-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-171">Boolean</span></span>|<span data-ttu-id="3cc53-172">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-172">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="3cc53-173">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="3cc53-173">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="3cc53-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-174">Boolean</span></span>|<span data-ttu-id="3cc53-175">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-175">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="3cc53-176">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="3cc53-176">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="3cc53-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-177">Boolean</span></span>|<span data-ttu-id="3cc53-178">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-178">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="3cc53-179">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="3cc53-179">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="3cc53-180">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="3cc53-180">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="3cc53-181">証明書失効リストの適用方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-181">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="3cc53-182">可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-182">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="3cc53-183">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="3cc53-183">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="3cc53-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-184">Boolean</span></span>|<span data-ttu-id="3cc53-185">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="3cc53-185">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="3cc53-186">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="3cc53-186">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="3cc53-187">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="3cc53-187">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="3cc53-188">トンネルゲートウェイのシナリオでパケットキューを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-188">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="3cc53-189">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-189">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="3cc53-190">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="3cc53-190">firewallProfileDomain</span></span>|[<span data-ttu-id="3cc53-191">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3cc53-191">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="3cc53-192">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="3cc53-192">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="3cc53-193">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="3cc53-193">firewallProfilePublic</span></span>|[<span data-ttu-id="3cc53-194">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3cc53-194">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="3cc53-195">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="3cc53-195">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="3cc53-196">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="3cc53-196">firewallProfilePrivate</span></span>|[<span data-ttu-id="3cc53-197">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3cc53-197">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="3cc53-198">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="3cc53-198">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="3cc53-199">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="3cc53-199">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="3cc53-200">String collection</span><span class="sxs-lookup"><span data-stu-id="3cc53-200">String collection</span></span>|<span data-ttu-id="3cc53-201">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="3cc53-201">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="3cc53-202">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="3cc53-202">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="3cc53-203">String collection</span><span class="sxs-lookup"><span data-stu-id="3cc53-203">String collection</span></span>|<span data-ttu-id="3cc53-204">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="3cc53-204">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="3cc53-205">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="3cc53-205">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="3cc53-206">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3cc53-206">String collection</span></span>|<span data-ttu-id="3cc53-207">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="3cc53-207">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="3cc53-208">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="3cc53-208">defenderExploitProtectionXml</span></span>|<span data-ttu-id="3cc53-209">Binary</span><span class="sxs-lookup"><span data-stu-id="3cc53-209">Binary</span></span>|<span data-ttu-id="3cc53-210">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="3cc53-210">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="3cc53-211">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="3cc53-211">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="3cc53-212">String</span><span class="sxs-lookup"><span data-stu-id="3cc53-212">String</span></span>|<span data-ttu-id="3cc53-213">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="3cc53-213">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="3cc53-214">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="3cc53-214">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="3cc53-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-215">Boolean</span></span>|<span data-ttu-id="3cc53-216">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-216">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="3cc53-217">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="3cc53-217">appLockerApplicationControl</span></span>|[<span data-ttu-id="3cc53-218">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="3cc53-218">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="3cc53-219">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="3cc53-219">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="3cc53-220">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-220">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="3cc53-221">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="3cc53-221">smartScreenEnableInShell</span></span>|<span data-ttu-id="3cc53-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-222">Boolean</span></span>|<span data-ttu-id="3cc53-223">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-223">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="3cc53-224">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="3cc53-224">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="3cc53-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-225">Boolean</span></span>|<span data-ttu-id="3cc53-226">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-226">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="3cc53-227">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="3cc53-227">applicationGuardEnabled</span></span>|<span data-ttu-id="3cc53-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-228">Boolean</span></span>|<span data-ttu-id="3cc53-229">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="3cc53-229">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="3cc53-230">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="3cc53-230">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="3cc53-231">applicationgu/blockfiletransfertype</span><span class="sxs-lookup"><span data-stu-id="3cc53-231">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="3cc53-232">画像ファイル、テキストファイル、またはそのどちらも転送しないように、クリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="3cc53-232">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="3cc53-233">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-233">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="3cc53-234">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="3cc53-234">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="3cc53-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-235">Boolean</span></span>|<span data-ttu-id="3cc53-236">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="3cc53-236">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="3cc53-237">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="3cc53-237">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="3cc53-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-238">Boolean</span></span>|<span data-ttu-id="3cc53-239">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-239">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="3cc53-240">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="3cc53-240">applicationGuardForceAuditing</span></span>|<span data-ttu-id="3cc53-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-241">Boolean</span></span>|<span data-ttu-id="3cc53-242">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="3cc53-242">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="3cc53-243">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="3cc53-243">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="3cc53-244">applicationgu/blockクリップボード sharingtype</span><span class="sxs-lookup"><span data-stu-id="3cc53-244">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="3cc53-245">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="3cc53-245">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="3cc53-246">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-246">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="3cc53-247">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="3cc53-247">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="3cc53-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-248">Boolean</span></span>|<span data-ttu-id="3cc53-249">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-249">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="3cc53-250">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="3cc53-250">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="3cc53-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-251">Boolean</span></span>|<span data-ttu-id="3cc53-252">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-252">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="3cc53-253">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="3cc53-253">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="3cc53-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-254">Boolean</span></span>|<span data-ttu-id="3cc53-255">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-255">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="3cc53-256">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="3cc53-256">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="3cc53-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-257">Boolean</span></span>|<span data-ttu-id="3cc53-258">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="3cc53-258">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="3cc53-259">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="3cc53-259">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="3cc53-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-260">Boolean</span></span>|<span data-ttu-id="3cc53-261">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-261">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="3cc53-262">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="3cc53-262">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="3cc53-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-263">Boolean</span></span>|<span data-ttu-id="3cc53-264">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-264">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="3cc53-265">このポリシーは、携帯電話の SKU に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-265">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="3cc53-266">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="3cc53-266">bitLockerEncryptDevice</span></span>|<span data-ttu-id="3cc53-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc53-267">Boolean</span></span>|<span data-ttu-id="3cc53-268">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-268">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="3cc53-269">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3cc53-269">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="3cc53-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3cc53-270">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="3cc53-271">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="3cc53-271">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="3cc53-272">応答</span><span class="sxs-lookup"><span data-stu-id="3cc53-272">Response</span></span>
<span data-ttu-id="3cc53-273">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3cc53-273">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cc53-274">例</span><span class="sxs-lookup"><span data-stu-id="3cc53-274">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cc53-275">要求</span><span class="sxs-lookup"><span data-stu-id="3cc53-275">Request</span></span>
<span data-ttu-id="3cc53-276">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3cc53-276">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3cc53-277">応答</span><span class="sxs-lookup"><span data-stu-id="3cc53-277">Response</span></span>
<span data-ttu-id="3cc53-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3cc53-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



