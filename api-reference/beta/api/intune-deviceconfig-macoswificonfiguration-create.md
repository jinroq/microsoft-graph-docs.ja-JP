---
title: MacOSWiFiConfiguration を作成する
description: 新しい macOSWiFiConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73e5dc37202efbcd045a60454b3d93bbde561ef1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922144"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="160f6-103">MacOSWiFiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="160f6-103">Create macOSWiFiConfiguration</span></span>

> <span data-ttu-id="160f6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="160f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="160f6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="160f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="160f6-106">新しい[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="160f6-106">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="160f6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="160f6-107">Prerequisites</span></span>
<span data-ttu-id="160f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="160f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="160f6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="160f6-110">Permission type</span></span>|<span data-ttu-id="160f6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="160f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="160f6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="160f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="160f6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="160f6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="160f6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="160f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="160f6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="160f6-115">Not supported.</span></span>|
|<span data-ttu-id="160f6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="160f6-116">Application</span></span>|<span data-ttu-id="160f6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="160f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="160f6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="160f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="160f6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="160f6-119">Request headers</span></span>
|<span data-ttu-id="160f6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="160f6-120">Header</span></span>|<span data-ttu-id="160f6-121">値</span><span class="sxs-lookup"><span data-stu-id="160f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="160f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="160f6-122">Authorization</span></span>|<span data-ttu-id="160f6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="160f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="160f6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="160f6-124">Accept</span></span>|<span data-ttu-id="160f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="160f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="160f6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="160f6-126">Request body</span></span>
<span data-ttu-id="160f6-127">要求本文で、macOSWiFiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="160f6-127">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="160f6-128">次の表に、macOSWiFiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="160f6-128">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="160f6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="160f6-129">Property</span></span>|<span data-ttu-id="160f6-130">型</span><span class="sxs-lookup"><span data-stu-id="160f6-130">Type</span></span>|<span data-ttu-id="160f6-131">説明</span><span class="sxs-lookup"><span data-stu-id="160f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="160f6-132">id</span><span class="sxs-lookup"><span data-stu-id="160f6-132">id</span></span>|<span data-ttu-id="160f6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="160f6-133">String</span></span>|<span data-ttu-id="160f6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="160f6-134">Key of the entity.</span></span> <span data-ttu-id="160f6-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160f6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160f6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="160f6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="160f6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="160f6-137">DateTimeOffset</span></span>|<span data-ttu-id="160f6-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="160f6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="160f6-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160f6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160f6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="160f6-140">roleScopeTagIds</span></span>|<span data-ttu-id="160f6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="160f6-141">String collection</span></span>|<span data-ttu-id="160f6-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="160f6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="160f6-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160f6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160f6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="160f6-144">supportsScopeTags</span></span>|<span data-ttu-id="160f6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="160f6-145">Boolean</span></span>|<span data-ttu-id="160f6-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="160f6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="160f6-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="160f6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="160f6-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="160f6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="160f6-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="160f6-149">This property is read-only.</span></span> <span data-ttu-id="160f6-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160f6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160f6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="160f6-151">createdDateTime</span></span>|<span data-ttu-id="160f6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="160f6-152">DateTimeOffset</span></span>|<span data-ttu-id="160f6-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="160f6-153">DateTime the object was created.</span></span> <span data-ttu-id="160f6-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160f6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160f6-155">description</span><span class="sxs-lookup"><span data-stu-id="160f6-155">description</span></span>|<span data-ttu-id="160f6-156">String</span><span class="sxs-lookup"><span data-stu-id="160f6-156">String</span></span>|<span data-ttu-id="160f6-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="160f6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="160f6-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160f6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160f6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="160f6-159">displayName</span></span>|<span data-ttu-id="160f6-160">String</span><span class="sxs-lookup"><span data-stu-id="160f6-160">String</span></span>|<span data-ttu-id="160f6-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="160f6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="160f6-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160f6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160f6-163">version</span><span class="sxs-lookup"><span data-stu-id="160f6-163">version</span></span>|<span data-ttu-id="160f6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="160f6-164">Int32</span></span>|<span data-ttu-id="160f6-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="160f6-165">Version of the device configuration.</span></span> <span data-ttu-id="160f6-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160f6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160f6-167">networkName</span><span class="sxs-lookup"><span data-stu-id="160f6-167">networkName</span></span>|<span data-ttu-id="160f6-168">String</span><span class="sxs-lookup"><span data-stu-id="160f6-168">String</span></span>|<span data-ttu-id="160f6-169">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="160f6-169">Network Name</span></span>|
|<span data-ttu-id="160f6-170">ssid</span><span class="sxs-lookup"><span data-stu-id="160f6-170">ssid</span></span>|<span data-ttu-id="160f6-171">String</span><span class="sxs-lookup"><span data-stu-id="160f6-171">String</span></span>|<span data-ttu-id="160f6-172">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="160f6-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="160f6-173">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="160f6-173">connectAutomatically</span></span>|<span data-ttu-id="160f6-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="160f6-174">Boolean</span></span>|<span data-ttu-id="160f6-175">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="160f6-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="160f6-176">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="160f6-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="160f6-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="160f6-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="160f6-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="160f6-178">Boolean</span></span>|<span data-ttu-id="160f6-179">ネットワークが名前 (SSID) をブロードキャストしていない場合に接続します。</span><span class="sxs-lookup"><span data-stu-id="160f6-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="160f6-180">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="160f6-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="160f6-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="160f6-181">wiFiSecurityType</span></span>|[<span data-ttu-id="160f6-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="160f6-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="160f6-183">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="160f6-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="160f6-184">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="160f6-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="160f6-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="160f6-185">proxySettings</span></span>|[<span data-ttu-id="160f6-186">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="160f6-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="160f6-187">この Wi-fi 接続のプロキシの種類。</span><span class="sxs-lookup"><span data-stu-id="160f6-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="160f6-188">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="160f6-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="160f6-189">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="160f6-189">proxyManualAddress</span></span>|<span data-ttu-id="160f6-190">String</span><span class="sxs-lookup"><span data-stu-id="160f6-190">String</span></span>|<span data-ttu-id="160f6-191">手動構成が選択されている場合のプロキシサーバーの IP アドレスまたは DNS ホスト名。</span><span class="sxs-lookup"><span data-stu-id="160f6-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="160f6-192">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="160f6-192">proxyManualPort</span></span>|<span data-ttu-id="160f6-193">Int32</span><span class="sxs-lookup"><span data-stu-id="160f6-193">Int32</span></span>|<span data-ttu-id="160f6-194">手動構成が選択されている場合のプロキシサーバーのポート。</span><span class="sxs-lookup"><span data-stu-id="160f6-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="160f6-195">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="160f6-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="160f6-196">String</span><span class="sxs-lookup"><span data-stu-id="160f6-196">String</span></span>|<span data-ttu-id="160f6-197">自動構成が選択されている場合のプロキシサーバーの自動構成スクリプトの URL。</span><span class="sxs-lookup"><span data-stu-id="160f6-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="160f6-198">この URL は、通常、PAC (プロキシ自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="160f6-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="160f6-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="160f6-199">preSharedKey</span></span>|<span data-ttu-id="160f6-200">String</span><span class="sxs-lookup"><span data-stu-id="160f6-200">String</span></span>|<span data-ttu-id="160f6-201">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="160f6-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="160f6-202">応答</span><span class="sxs-lookup"><span data-stu-id="160f6-202">Response</span></span>
<span data-ttu-id="160f6-203">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="160f6-203">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="160f6-204">例</span><span class="sxs-lookup"><span data-stu-id="160f6-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="160f6-205">要求</span><span class="sxs-lookup"><span data-stu-id="160f6-205">Request</span></span>
<span data-ttu-id="160f6-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="160f6-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 677

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="160f6-207">応答</span><span class="sxs-lookup"><span data-stu-id="160f6-207">Response</span></span>
<span data-ttu-id="160f6-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="160f6-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 849

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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




