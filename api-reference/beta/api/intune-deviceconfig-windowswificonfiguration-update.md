---
title: windowsWifiConfiguration の更新
description: windowsWifiConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07573055554ac68aea1caa14a774c92bb2ef713f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781569"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="aec36-103">windowsWifiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="aec36-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="aec36-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aec36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aec36-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aec36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aec36-106">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aec36-106">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aec36-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="aec36-107">Prerequisites</span></span>
<span data-ttu-id="aec36-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aec36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec36-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aec36-110">Permission type</span></span>|<span data-ttu-id="aec36-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aec36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aec36-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aec36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aec36-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec36-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aec36-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aec36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aec36-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aec36-115">Not supported.</span></span>|
|<span data-ttu-id="aec36-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aec36-116">Application</span></span>|<span data-ttu-id="aec36-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aec36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aec36-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aec36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aec36-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aec36-119">Request headers</span></span>
|<span data-ttu-id="aec36-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aec36-120">Header</span></span>|<span data-ttu-id="aec36-121">値</span><span class="sxs-lookup"><span data-stu-id="aec36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aec36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aec36-122">Authorization</span></span>|<span data-ttu-id="aec36-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="aec36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aec36-124">承諾</span><span class="sxs-lookup"><span data-stu-id="aec36-124">Accept</span></span>|<span data-ttu-id="aec36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aec36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aec36-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="aec36-126">Request body</span></span>
<span data-ttu-id="aec36-127">要求本文で、 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-127">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="aec36-128">次の表に、 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="aec36-128">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="aec36-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aec36-129">Property</span></span>|<span data-ttu-id="aec36-130">型</span><span class="sxs-lookup"><span data-stu-id="aec36-130">Type</span></span>|<span data-ttu-id="aec36-131">説明</span><span class="sxs-lookup"><span data-stu-id="aec36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aec36-132">id</span><span class="sxs-lookup"><span data-stu-id="aec36-132">id</span></span>|<span data-ttu-id="aec36-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="aec36-133">String</span></span>|<span data-ttu-id="aec36-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aec36-134">Key of the entity.</span></span> <span data-ttu-id="aec36-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aec36-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aec36-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aec36-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aec36-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec36-137">DateTimeOffset</span></span>|<span data-ttu-id="aec36-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="aec36-138">DateTime the object was last modified.</span></span> <span data-ttu-id="aec36-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aec36-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aec36-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aec36-140">roleScopeTagIds</span></span>|<span data-ttu-id="aec36-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aec36-141">String collection</span></span>|<span data-ttu-id="aec36-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="aec36-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aec36-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aec36-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aec36-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aec36-144">supportsScopeTags</span></span>|<span data-ttu-id="aec36-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec36-145">Boolean</span></span>|<span data-ttu-id="aec36-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aec36-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aec36-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="aec36-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aec36-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="aec36-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aec36-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="aec36-149">This property is read-only.</span></span> <span data-ttu-id="aec36-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aec36-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aec36-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aec36-151">createdDateTime</span></span>|<span data-ttu-id="aec36-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec36-152">DateTimeOffset</span></span>|<span data-ttu-id="aec36-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="aec36-153">DateTime the object was created.</span></span> <span data-ttu-id="aec36-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aec36-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aec36-155">説明</span><span class="sxs-lookup"><span data-stu-id="aec36-155">description</span></span>|<span data-ttu-id="aec36-156">String</span><span class="sxs-lookup"><span data-stu-id="aec36-156">String</span></span>|<span data-ttu-id="aec36-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="aec36-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aec36-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aec36-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aec36-159">displayName</span><span class="sxs-lookup"><span data-stu-id="aec36-159">displayName</span></span>|<span data-ttu-id="aec36-160">String</span><span class="sxs-lookup"><span data-stu-id="aec36-160">String</span></span>|<span data-ttu-id="aec36-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="aec36-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aec36-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aec36-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aec36-163">version</span><span class="sxs-lookup"><span data-stu-id="aec36-163">version</span></span>|<span data-ttu-id="aec36-164">Int32</span><span class="sxs-lookup"><span data-stu-id="aec36-164">Int32</span></span>|<span data-ttu-id="aec36-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="aec36-165">Version of the device configuration.</span></span> <span data-ttu-id="aec36-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aec36-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aec36-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="aec36-167">preSharedKey</span></span>|<span data-ttu-id="aec36-168">文字列</span><span class="sxs-lookup"><span data-stu-id="aec36-168">String</span></span>|<span data-ttu-id="aec36-169">これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="aec36-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="aec36-170">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="aec36-170">wifiSecurityType</span></span>|[<span data-ttu-id="aec36-171">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="aec36-171">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="aec36-172">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-172">Specify the Wifi Security Type.</span></span> <span data-ttu-id="aec36-173">可能な値は `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="aec36-173">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="aec36-174">meteredconnectionlimit</span><span class="sxs-lookup"><span data-stu-id="aec36-174">meteredConnectionLimit</span></span>|[<span data-ttu-id="aec36-175">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="aec36-175">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="aec36-176">wifi 接続の従量制課金接続制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-176">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="aec36-177">使用可能な値は、`unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="aec36-177">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="aec36-178">ssid</span><span class="sxs-lookup"><span data-stu-id="aec36-178">ssid</span></span>|<span data-ttu-id="aec36-179">文字列</span><span class="sxs-lookup"><span data-stu-id="aec36-179">String</span></span>|<span data-ttu-id="aec36-180">wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-180">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="aec36-181">networkname</span><span class="sxs-lookup"><span data-stu-id="aec36-181">networkName</span></span>|<span data-ttu-id="aec36-182">文字列</span><span class="sxs-lookup"><span data-stu-id="aec36-182">String</span></span>|<span data-ttu-id="aec36-183">ネットワーク構成名を指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-183">Specify the network configuration name.</span></span>|
|<span data-ttu-id="aec36-184">connectautomatically に</span><span class="sxs-lookup"><span data-stu-id="aec36-184">connectAutomatically</span></span>|<span data-ttu-id="aec36-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec36-185">Boolean</span></span>|<span data-ttu-id="aec36-186">範囲内で wifi 接続を自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-186">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="aec36-187">connecttopreferrednetwork</span><span class="sxs-lookup"><span data-stu-id="aec36-187">connectToPreferredNetwork</span></span>|<span data-ttu-id="aec36-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec36-188">Boolean</span></span>|<span data-ttu-id="aec36-189">この接続に既に接続されている場合に、wifi 接続がより優先度の高いネットワークに接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-189">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="aec36-190">connectautomatically 自動的に true になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="aec36-190">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="aec36-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="aec36-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="aec36-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec36-192">Boolean</span></span>|<span data-ttu-id="aec36-193">SSID がブロードキャストされていない場合でも、wifi 接続が自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-193">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="aec36-194">proxysetting</span><span class="sxs-lookup"><span data-stu-id="aec36-194">proxySetting</span></span>|[<span data-ttu-id="aec36-195">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="aec36-195">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="aec36-196">wi-fi 構成のプロキシ設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-196">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="aec36-197">使用可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="aec36-197">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="aec36-198">proxymanualaddress</span><span class="sxs-lookup"><span data-stu-id="aec36-198">proxyManualAddress</span></span>|<span data-ttu-id="aec36-199">文字列</span><span class="sxs-lookup"><span data-stu-id="aec36-199">String</span></span>|<span data-ttu-id="aec36-200">プロキシサーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-200">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="aec36-201">proxymanualport</span><span class="sxs-lookup"><span data-stu-id="aec36-201">proxyManualPort</span></span>|<span data-ttu-id="aec36-202">Int32</span><span class="sxs-lookup"><span data-stu-id="aec36-202">Int32</span></span>|<span data-ttu-id="aec36-203">プロキシサーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-203">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="aec36-204">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="aec36-204">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="aec36-205">文字列</span><span class="sxs-lookup"><span data-stu-id="aec36-205">String</span></span>|<span data-ttu-id="aec36-206">プロキシサーバー構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-206">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="aec36-207">forcefipscompliance</span><span class="sxs-lookup"><span data-stu-id="aec36-207">forceFIPSCompliance</span></span>|<span data-ttu-id="aec36-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec36-208">Boolean</span></span>|<span data-ttu-id="aec36-209">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="aec36-209">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="aec36-210">応答</span><span class="sxs-lookup"><span data-stu-id="aec36-210">Response</span></span>
<span data-ttu-id="aec36-211">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aec36-211">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aec36-212">例</span><span class="sxs-lookup"><span data-stu-id="aec36-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="aec36-213">要求</span><span class="sxs-lookup"><span data-stu-id="aec36-213">Request</span></span>
<span data-ttu-id="aec36-214">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aec36-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 786

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="aec36-215">応答</span><span class="sxs-lookup"><span data-stu-id="aec36-215">Response</span></span>
<span data-ttu-id="aec36-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aec36-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```





