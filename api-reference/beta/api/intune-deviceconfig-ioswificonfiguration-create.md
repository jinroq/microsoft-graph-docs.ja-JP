---
title: IosWiFiConfiguration を作成します。
description: 新しい iosWiFiConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 0e16c9ed6877977ff0e0b6c3c5c4e21597934130
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362252"
---
# <a name="create-ioswificonfiguration"></a><span data-ttu-id="9dcdf-103">IosWiFiConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-103">Create iosWiFiConfiguration</span></span>

> <span data-ttu-id="9dcdf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dcdf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9dcdf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9dcdf-107">新しい[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-107">Create a new [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9dcdf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9dcdf-108">Prerequisites</span></span>
<span data-ttu-id="9dcdf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dcdf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9dcdf-111">Permission type</span></span>|<span data-ttu-id="9dcdf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9dcdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dcdf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9dcdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9dcdf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dcdf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9dcdf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9dcdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dcdf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-116">Not supported.</span></span>|
|<span data-ttu-id="9dcdf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9dcdf-117">Application</span></span>|<span data-ttu-id="9dcdf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dcdf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9dcdf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9dcdf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9dcdf-120">Request headers</span></span>
|<span data-ttu-id="9dcdf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9dcdf-121">Header</span></span>|<span data-ttu-id="9dcdf-122">値</span><span class="sxs-lookup"><span data-stu-id="9dcdf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dcdf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dcdf-123">Authorization</span></span>|<span data-ttu-id="9dcdf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dcdf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9dcdf-125">Accept</span></span>|<span data-ttu-id="9dcdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9dcdf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dcdf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9dcdf-127">Request body</span></span>
<span data-ttu-id="9dcdf-128">要求の本文に iosWiFiConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-128">In the request body, supply a JSON representation for the iosWiFiConfiguration object.</span></span>

<span data-ttu-id="9dcdf-129">次の表は、iosWiFiConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-129">The following table shows the properties that are required when you create the iosWiFiConfiguration.</span></span>

|<span data-ttu-id="9dcdf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dcdf-130">Property</span></span>|<span data-ttu-id="9dcdf-131">種類</span><span class="sxs-lookup"><span data-stu-id="9dcdf-131">Type</span></span>|<span data-ttu-id="9dcdf-132">説明</span><span class="sxs-lookup"><span data-stu-id="9dcdf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dcdf-133">ID</span><span class="sxs-lookup"><span data-stu-id="9dcdf-133">id</span></span>|<span data-ttu-id="9dcdf-134">String</span><span class="sxs-lookup"><span data-stu-id="9dcdf-134">String</span></span>|<span data-ttu-id="9dcdf-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-135">Key of the entity.</span></span> <span data-ttu-id="9dcdf-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9dcdf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dcdf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9dcdf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9dcdf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dcdf-138">DateTimeOffset</span></span>|<span data-ttu-id="9dcdf-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9dcdf-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9dcdf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dcdf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9dcdf-141">roleScopeTagIds</span></span>|<span data-ttu-id="9dcdf-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9dcdf-142">String collection</span></span>|<span data-ttu-id="9dcdf-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9dcdf-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9dcdf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dcdf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9dcdf-145">supportsScopeTags</span></span>|<span data-ttu-id="9dcdf-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="9dcdf-146">Boolean</span></span>|<span data-ttu-id="9dcdf-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9dcdf-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9dcdf-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9dcdf-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-150">This property is read-only.</span></span> <span data-ttu-id="9dcdf-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9dcdf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dcdf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9dcdf-152">createdDateTime</span></span>|<span data-ttu-id="9dcdf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dcdf-153">DateTimeOffset</span></span>|<span data-ttu-id="9dcdf-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-154">DateTime the object was created.</span></span> <span data-ttu-id="9dcdf-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9dcdf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dcdf-156">説明</span><span class="sxs-lookup"><span data-stu-id="9dcdf-156">description</span></span>|<span data-ttu-id="9dcdf-157">String</span><span class="sxs-lookup"><span data-stu-id="9dcdf-157">String</span></span>|<span data-ttu-id="9dcdf-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9dcdf-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9dcdf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dcdf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9dcdf-160">displayName</span></span>|<span data-ttu-id="9dcdf-161">String</span><span class="sxs-lookup"><span data-stu-id="9dcdf-161">String</span></span>|<span data-ttu-id="9dcdf-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9dcdf-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9dcdf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dcdf-164">version</span><span class="sxs-lookup"><span data-stu-id="9dcdf-164">version</span></span>|<span data-ttu-id="9dcdf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9dcdf-165">Int32</span></span>|<span data-ttu-id="9dcdf-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-166">Version of the device configuration.</span></span> <span data-ttu-id="9dcdf-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9dcdf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dcdf-168">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="9dcdf-168">networkName</span></span>|<span data-ttu-id="9dcdf-169">String</span><span class="sxs-lookup"><span data-stu-id="9dcdf-169">String</span></span>|<span data-ttu-id="9dcdf-170">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="9dcdf-170">Network Name</span></span>|
|<span data-ttu-id="9dcdf-171">ssid</span><span class="sxs-lookup"><span data-stu-id="9dcdf-171">ssid</span></span>|<span data-ttu-id="9dcdf-172">String</span><span class="sxs-lookup"><span data-stu-id="9dcdf-172">String</span></span>|<span data-ttu-id="9dcdf-173">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="9dcdf-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="9dcdf-174">connectAutomatically</span></span>|<span data-ttu-id="9dcdf-175">ブール型</span><span class="sxs-lookup"><span data-stu-id="9dcdf-175">Boolean</span></span>|<span data-ttu-id="9dcdf-176">このネットワークが範囲内にすると自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="9dcdf-177">これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="9dcdf-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9dcdf-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9dcdf-179">ブール型</span><span class="sxs-lookup"><span data-stu-id="9dcdf-179">Boolean</span></span>|<span data-ttu-id="9dcdf-180">ネットワーク名 (SSID) をブロードキャストしていないときに接続します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-180">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="9dcdf-181">True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="9dcdf-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9dcdf-182">wiFiSecurityType</span></span>|[<span data-ttu-id="9dcdf-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9dcdf-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="9dcdf-184">Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-184">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="9dcdf-185">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="9dcdf-186">型のオブジェクトで</span><span class="sxs-lookup"><span data-stu-id="9dcdf-186">proxySettings</span></span>|[<span data-ttu-id="9dcdf-187">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="9dcdf-187">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="9dcdf-188">この Wi-fi 接続のプロキシの種類です。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-188">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="9dcdf-189">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-189">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="9dcdf-190">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="9dcdf-190">proxyManualAddress</span></span>|<span data-ttu-id="9dcdf-191">String</span><span class="sxs-lookup"><span data-stu-id="9dcdf-191">String</span></span>|<span data-ttu-id="9dcdf-192">手動の構成が選択されている時にプロキシ サーバーの IP アドレスまたは DNS ホスト名</span><span class="sxs-lookup"><span data-stu-id="9dcdf-192">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="9dcdf-193">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="9dcdf-193">proxyManualPort</span></span>|<span data-ttu-id="9dcdf-194">Int32</span><span class="sxs-lookup"><span data-stu-id="9dcdf-194">Int32</span></span>|<span data-ttu-id="9dcdf-195">手動の構成が選択されている時にプロキシ サーバーのポートです。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-195">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="9dcdf-196">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="9dcdf-196">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="9dcdf-197">String</span><span class="sxs-lookup"><span data-stu-id="9dcdf-197">String</span></span>|<span data-ttu-id="9dcdf-198">自動構成を選択すると、プロキシ サーバーの自動構成スクリプトの URL です。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-198">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="9dcdf-199">この URL は、通常、PAC (プロキシの自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-199">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="9dcdf-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="9dcdf-200">preSharedKey</span></span>|<span data-ttu-id="9dcdf-201">String</span><span class="sxs-lookup"><span data-stu-id="9dcdf-201">String</span></span>|<span data-ttu-id="9dcdf-202">これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="9dcdf-203">応答</span><span class="sxs-lookup"><span data-stu-id="9dcdf-203">Response</span></span>
<span data-ttu-id="9dcdf-204">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-204">If successful, this method returns a `201 Created` response code and a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dcdf-205">例</span><span class="sxs-lookup"><span data-stu-id="9dcdf-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="9dcdf-206">要求</span><span class="sxs-lookup"><span data-stu-id="9dcdf-206">Request</span></span>
<span data-ttu-id="9dcdf-207">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-207">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 739

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="9dcdf-208">応答</span><span class="sxs-lookup"><span data-stu-id="9dcdf-208">Response</span></span>
<span data-ttu-id="9dcdf-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9dcdf-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 847

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```




