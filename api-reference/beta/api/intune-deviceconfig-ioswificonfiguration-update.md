---
title: iosWiFiConfiguration の更新
description: iosWiFiConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f13f24fcc58e43020e0d1272b6b5cb54d46cc8e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519018"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="23ca4-103">iosWiFiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="23ca4-103">Update iosWiFiConfiguration</span></span>

> <span data-ttu-id="23ca4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23ca4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23ca4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23ca4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23ca4-106">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-106">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23ca4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="23ca4-107">Prerequisites</span></span>
<span data-ttu-id="23ca4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23ca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23ca4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23ca4-110">Permission type</span></span>|<span data-ttu-id="23ca4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="23ca4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23ca4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23ca4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23ca4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23ca4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23ca4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23ca4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23ca4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23ca4-115">Not supported.</span></span>|
|<span data-ttu-id="23ca4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23ca4-116">Application</span></span>|<span data-ttu-id="23ca4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23ca4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23ca4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23ca4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="23ca4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23ca4-119">Request headers</span></span>
|<span data-ttu-id="23ca4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23ca4-120">Header</span></span>|<span data-ttu-id="23ca4-121">値</span><span class="sxs-lookup"><span data-stu-id="23ca4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23ca4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="23ca4-122">Authorization</span></span>|<span data-ttu-id="23ca4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="23ca4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23ca4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="23ca4-124">Accept</span></span>|<span data-ttu-id="23ca4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23ca4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23ca4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="23ca4-126">Request body</span></span>
<span data-ttu-id="23ca4-127">要求本文で、 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-127">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="23ca4-128">次の表に、 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-128">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="23ca4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23ca4-129">Property</span></span>|<span data-ttu-id="23ca4-130">型</span><span class="sxs-lookup"><span data-stu-id="23ca4-130">Type</span></span>|<span data-ttu-id="23ca4-131">説明</span><span class="sxs-lookup"><span data-stu-id="23ca4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23ca4-132">id</span><span class="sxs-lookup"><span data-stu-id="23ca4-132">id</span></span>|<span data-ttu-id="23ca4-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="23ca4-133">String</span></span>|<span data-ttu-id="23ca4-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="23ca4-134">Key of the entity.</span></span> <span data-ttu-id="23ca4-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23ca4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ca4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23ca4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="23ca4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ca4-137">DateTimeOffset</span></span>|<span data-ttu-id="23ca4-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="23ca4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="23ca4-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23ca4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ca4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23ca4-140">roleScopeTagIds</span></span>|<span data-ttu-id="23ca4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="23ca4-141">String collection</span></span>|<span data-ttu-id="23ca4-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="23ca4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="23ca4-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23ca4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ca4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="23ca4-144">supportsScopeTags</span></span>|<span data-ttu-id="23ca4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="23ca4-145">Boolean</span></span>|<span data-ttu-id="23ca4-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="23ca4-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="23ca4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="23ca4-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="23ca4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="23ca4-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-149">This property is read-only.</span></span> <span data-ttu-id="23ca4-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23ca4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ca4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23ca4-151">createdDateTime</span></span>|<span data-ttu-id="23ca4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ca4-152">DateTimeOffset</span></span>|<span data-ttu-id="23ca4-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="23ca4-153">DateTime the object was created.</span></span> <span data-ttu-id="23ca4-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23ca4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ca4-155">説明</span><span class="sxs-lookup"><span data-stu-id="23ca4-155">description</span></span>|<span data-ttu-id="23ca4-156">String</span><span class="sxs-lookup"><span data-stu-id="23ca4-156">String</span></span>|<span data-ttu-id="23ca4-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="23ca4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23ca4-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23ca4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ca4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="23ca4-159">displayName</span></span>|<span data-ttu-id="23ca4-160">String</span><span class="sxs-lookup"><span data-stu-id="23ca4-160">String</span></span>|<span data-ttu-id="23ca4-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="23ca4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23ca4-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23ca4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ca4-163">version</span><span class="sxs-lookup"><span data-stu-id="23ca4-163">version</span></span>|<span data-ttu-id="23ca4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="23ca4-164">Int32</span></span>|<span data-ttu-id="23ca4-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="23ca4-165">Version of the device configuration.</span></span> <span data-ttu-id="23ca4-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23ca4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ca4-167">networkname</span><span class="sxs-lookup"><span data-stu-id="23ca4-167">networkName</span></span>|<span data-ttu-id="23ca4-168">String</span><span class="sxs-lookup"><span data-stu-id="23ca4-168">String</span></span>|<span data-ttu-id="23ca4-169">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="23ca4-169">Network Name</span></span>|
|<span data-ttu-id="23ca4-170">ssid</span><span class="sxs-lookup"><span data-stu-id="23ca4-170">ssid</span></span>|<span data-ttu-id="23ca4-171">String</span><span class="sxs-lookup"><span data-stu-id="23ca4-171">String</span></span>|<span data-ttu-id="23ca4-172">これは、すべてのデバイスにブロードキャストされている wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="23ca4-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="23ca4-173">connectautomatically に</span><span class="sxs-lookup"><span data-stu-id="23ca4-173">connectAutomatically</span></span>|<span data-ttu-id="23ca4-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="23ca4-174">Boolean</span></span>|<span data-ttu-id="23ca4-175">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="23ca4-176">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="23ca4-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="23ca4-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="23ca4-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="23ca4-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="23ca4-178">Boolean</span></span>|<span data-ttu-id="23ca4-179">ネットワークが名前 (SSID) をブロードキャストしていない場合に接続します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="23ca4-180">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="23ca4-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="23ca4-181">wiFiSecurityType</span></span>|[<span data-ttu-id="23ca4-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="23ca4-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="23ca4-183">wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="23ca4-184">可能な値は `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="23ca4-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="23ca4-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="23ca4-185">proxySettings</span></span>|[<span data-ttu-id="23ca4-186">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="23ca4-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="23ca4-187">この wi-fi 接続のプロキシの種類。</span><span class="sxs-lookup"><span data-stu-id="23ca4-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="23ca4-188">使用可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="23ca4-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="23ca4-189">proxymanualaddress</span><span class="sxs-lookup"><span data-stu-id="23ca4-189">proxyManualAddress</span></span>|<span data-ttu-id="23ca4-190">String</span><span class="sxs-lookup"><span data-stu-id="23ca4-190">String</span></span>|<span data-ttu-id="23ca4-191">手動構成が選択されている場合のプロキシサーバーの IP アドレスまたは DNS ホスト名。</span><span class="sxs-lookup"><span data-stu-id="23ca4-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="23ca4-192">proxymanualport</span><span class="sxs-lookup"><span data-stu-id="23ca4-192">proxyManualPort</span></span>|<span data-ttu-id="23ca4-193">Int32</span><span class="sxs-lookup"><span data-stu-id="23ca4-193">Int32</span></span>|<span data-ttu-id="23ca4-194">手動構成が選択されている場合のプロキシサーバーのポート。</span><span class="sxs-lookup"><span data-stu-id="23ca4-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="23ca4-195">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="23ca4-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="23ca4-196">String</span><span class="sxs-lookup"><span data-stu-id="23ca4-196">String</span></span>|<span data-ttu-id="23ca4-197">自動構成が選択されている場合のプロキシサーバーの自動構成スクリプトの URL。</span><span class="sxs-lookup"><span data-stu-id="23ca4-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="23ca4-198">この URL は、通常、PAC (プロキシ自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="23ca4-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="23ca4-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="23ca4-199">preSharedKey</span></span>|<span data-ttu-id="23ca4-200">String</span><span class="sxs-lookup"><span data-stu-id="23ca4-200">String</span></span>|<span data-ttu-id="23ca4-201">これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="23ca4-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="23ca4-202">応答</span><span class="sxs-lookup"><span data-stu-id="23ca4-202">Response</span></span>
<span data-ttu-id="23ca4-203">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="23ca4-203">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23ca4-204">例</span><span class="sxs-lookup"><span data-stu-id="23ca4-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="23ca4-205">要求</span><span class="sxs-lookup"><span data-stu-id="23ca4-205">Request</span></span>
<span data-ttu-id="23ca4-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23ca4-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 675

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="23ca4-207">応答</span><span class="sxs-lookup"><span data-stu-id="23ca4-207">Response</span></span>
<span data-ttu-id="23ca4-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="23ca4-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





