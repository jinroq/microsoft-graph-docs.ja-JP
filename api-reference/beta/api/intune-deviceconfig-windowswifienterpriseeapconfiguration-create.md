---
title: windowsWifiEnterpriseEAPConfiguration を作成する
description: 新しい windowsWifiEnterpriseEAPConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64b79f93cfd9cd23617c99529331c6063efe6716
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32510823"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="de485-103">windowsWifiEnterpriseEAPConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="de485-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="de485-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de485-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de485-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="de485-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de485-106">新しい[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="de485-106">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de485-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="de485-107">Prerequisites</span></span>
<span data-ttu-id="de485-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de485-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de485-110">Permission type</span></span>|<span data-ttu-id="de485-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="de485-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de485-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de485-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de485-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de485-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de485-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de485-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de485-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de485-115">Not supported.</span></span>|
|<span data-ttu-id="de485-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de485-116">Application</span></span>|<span data-ttu-id="de485-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de485-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de485-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de485-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="de485-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de485-119">Request headers</span></span>
|<span data-ttu-id="de485-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de485-120">Header</span></span>|<span data-ttu-id="de485-121">値</span><span class="sxs-lookup"><span data-stu-id="de485-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de485-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de485-122">Authorization</span></span>|<span data-ttu-id="de485-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="de485-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de485-124">承諾</span><span class="sxs-lookup"><span data-stu-id="de485-124">Accept</span></span>|<span data-ttu-id="de485-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de485-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de485-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="de485-126">Request body</span></span>
<span data-ttu-id="de485-127">要求本文で、windowsWifiEnterpriseEAPConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-127">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="de485-128">次の表に、windowsWifiEnterpriseEAPConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="de485-128">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="de485-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de485-129">Property</span></span>|<span data-ttu-id="de485-130">型</span><span class="sxs-lookup"><span data-stu-id="de485-130">Type</span></span>|<span data-ttu-id="de485-131">説明</span><span class="sxs-lookup"><span data-stu-id="de485-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de485-132">id</span><span class="sxs-lookup"><span data-stu-id="de485-132">id</span></span>|<span data-ttu-id="de485-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="de485-133">String</span></span>|<span data-ttu-id="de485-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="de485-134">Key of the entity.</span></span> <span data-ttu-id="de485-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de485-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de485-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de485-136">lastModifiedDateTime</span></span>|<span data-ttu-id="de485-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de485-137">DateTimeOffset</span></span>|<span data-ttu-id="de485-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="de485-138">DateTime the object was last modified.</span></span> <span data-ttu-id="de485-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de485-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de485-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de485-140">roleScopeTagIds</span></span>|<span data-ttu-id="de485-141">String collection</span><span class="sxs-lookup"><span data-stu-id="de485-141">String collection</span></span>|<span data-ttu-id="de485-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="de485-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="de485-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de485-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de485-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="de485-144">supportsScopeTags</span></span>|<span data-ttu-id="de485-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="de485-145">Boolean</span></span>|<span data-ttu-id="de485-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de485-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="de485-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="de485-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="de485-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="de485-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="de485-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="de485-149">This property is read-only.</span></span> <span data-ttu-id="de485-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de485-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de485-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de485-151">createdDateTime</span></span>|<span data-ttu-id="de485-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de485-152">DateTimeOffset</span></span>|<span data-ttu-id="de485-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="de485-153">DateTime the object was created.</span></span> <span data-ttu-id="de485-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de485-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de485-155">説明</span><span class="sxs-lookup"><span data-stu-id="de485-155">description</span></span>|<span data-ttu-id="de485-156">String</span><span class="sxs-lookup"><span data-stu-id="de485-156">String</span></span>|<span data-ttu-id="de485-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="de485-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de485-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de485-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de485-159">displayName</span><span class="sxs-lookup"><span data-stu-id="de485-159">displayName</span></span>|<span data-ttu-id="de485-160">String</span><span class="sxs-lookup"><span data-stu-id="de485-160">String</span></span>|<span data-ttu-id="de485-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="de485-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de485-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de485-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de485-163">version</span><span class="sxs-lookup"><span data-stu-id="de485-163">version</span></span>|<span data-ttu-id="de485-164">Int32</span><span class="sxs-lookup"><span data-stu-id="de485-164">Int32</span></span>|<span data-ttu-id="de485-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="de485-165">Version of the device configuration.</span></span> <span data-ttu-id="de485-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de485-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de485-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="de485-167">preSharedKey</span></span>|<span data-ttu-id="de485-168">String</span><span class="sxs-lookup"><span data-stu-id="de485-168">String</span></span>|<span data-ttu-id="de485-169">これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="de485-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="de485-170">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-170">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="de485-171">wifiSecurityType</span></span>|[<span data-ttu-id="de485-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="de485-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="de485-173">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="de485-174">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="de485-174">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="de485-175">可能な値は `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="de485-175">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="de485-176">meteredconnectionlimit</span><span class="sxs-lookup"><span data-stu-id="de485-176">meteredConnectionLimit</span></span>|[<span data-ttu-id="de485-177">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="de485-177">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="de485-178">wifi 接続の従量制課金接続制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-178">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="de485-179">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="de485-179">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="de485-180">使用可能な値は、`unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="de485-180">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="de485-181">ssid</span><span class="sxs-lookup"><span data-stu-id="de485-181">ssid</span></span>|<span data-ttu-id="de485-182">String</span><span class="sxs-lookup"><span data-stu-id="de485-182">String</span></span>|<span data-ttu-id="de485-183">wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-183">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="de485-184">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-184">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-185">networkname</span><span class="sxs-lookup"><span data-stu-id="de485-185">networkName</span></span>|<span data-ttu-id="de485-186">String</span><span class="sxs-lookup"><span data-stu-id="de485-186">String</span></span>|<span data-ttu-id="de485-187">ネットワーク構成名を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-187">Specify the network configuration name.</span></span> <span data-ttu-id="de485-188">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-188">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-189">connectautomatically に</span><span class="sxs-lookup"><span data-stu-id="de485-189">connectAutomatically</span></span>|<span data-ttu-id="de485-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="de485-190">Boolean</span></span>|<span data-ttu-id="de485-191">範囲内で wifi 接続を自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-191">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="de485-192">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-193">connecttopreferrednetwork</span><span class="sxs-lookup"><span data-stu-id="de485-193">connectToPreferredNetwork</span></span>|<span data-ttu-id="de485-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="de485-194">Boolean</span></span>|<span data-ttu-id="de485-195">この接続に既に接続されている場合に、wifi 接続がより優先度の高いネットワークに接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-195">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="de485-196">connectautomatically 自動的に true になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="de485-196">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="de485-197">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-198">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="de485-198">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="de485-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="de485-199">Boolean</span></span>|<span data-ttu-id="de485-200">SSID がブロードキャストされていない場合でも、wifi 接続が自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-200">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="de485-201">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-202">proxysetting</span><span class="sxs-lookup"><span data-stu-id="de485-202">proxySetting</span></span>|[<span data-ttu-id="de485-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="de485-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="de485-204">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承した wi-fi 構成のプロキシ設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-204">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="de485-205">使用可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="de485-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="de485-206">proxymanualaddress</span><span class="sxs-lookup"><span data-stu-id="de485-206">proxyManualAddress</span></span>|<span data-ttu-id="de485-207">String</span><span class="sxs-lookup"><span data-stu-id="de485-207">String</span></span>|<span data-ttu-id="de485-208">プロキシサーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-208">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="de485-209">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-210">proxymanualport</span><span class="sxs-lookup"><span data-stu-id="de485-210">proxyManualPort</span></span>|<span data-ttu-id="de485-211">Int32</span><span class="sxs-lookup"><span data-stu-id="de485-211">Int32</span></span>|<span data-ttu-id="de485-212">プロキシサーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-212">Specify the port for the proxy server.</span></span> <span data-ttu-id="de485-213">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="de485-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="de485-215">String</span><span class="sxs-lookup"><span data-stu-id="de485-215">String</span></span>|<span data-ttu-id="de485-216">プロキシサーバー構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-216">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="de485-217">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-217">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-218">forcefipscompliance</span><span class="sxs-lookup"><span data-stu-id="de485-218">forceFIPSCompliance</span></span>|<span data-ttu-id="de485-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="de485-219">Boolean</span></span>|<span data-ttu-id="de485-220">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-220">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="de485-221">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="de485-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="de485-222">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="de485-222">networkSingleSignOn</span></span>|[<span data-ttu-id="de485-223">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="de485-223">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="de485-224">ネットワークのシングルサインオンの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-224">Specify the network single sign on type.</span></span> <span data-ttu-id="de485-225">使用可能な値は、`disabled`、`prelogon`、`postlogon` です。</span><span class="sxs-lookup"><span data-stu-id="de485-225">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="de485-226">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="de485-226">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="de485-227">Int32</span><span class="sxs-lookup"><span data-stu-id="de485-227">Int32</span></span>|<span data-ttu-id="de485-228">[最大認証タイムアウト (秒)] を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-228">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="de485-229">有効な範囲: 1-120</span><span class="sxs-lookup"><span data-stu-id="de485-229">Valid range: 1-120</span></span>|
|<span data-ttu-id="de485-230">promptforadditionalauthenticationcredentials</span><span class="sxs-lookup"><span data-stu-id="de485-230">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="de485-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="de485-231">Boolean</span></span>|<span data-ttu-id="de485-232">wifi 接続で追加の認証資格情報を求めるメッセージを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-232">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="de485-233">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="de485-233">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="de485-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="de485-234">Boolean</span></span>|<span data-ttu-id="de485-235">wifi 接続で、ペアワイズマスターキーのキャッシュを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-235">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="de485-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="de485-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="de485-237">Int32</span><span class="sxs-lookup"><span data-stu-id="de485-237">Int32</span></span>|<span data-ttu-id="de485-238">最大ペアワイズマスターキーキャッシュ時間を指定します (分単位)。</span><span class="sxs-lookup"><span data-stu-id="de485-238">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="de485-239">有効な範囲: 5-1440</span><span class="sxs-lookup"><span data-stu-id="de485-239">Valid range: 5-1440</span></span>|
|<span data-ttu-id="de485-240">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="de485-240">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="de485-241">Int32</span><span class="sxs-lookup"><span data-stu-id="de485-241">Int32</span></span>|<span data-ttu-id="de485-242">キャッシュ内のペアワイズマスターキーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-242">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="de485-243">有効な範囲: 1-255</span><span class="sxs-lookup"><span data-stu-id="de485-243">Valid range: 1-255</span></span>|
|<span data-ttu-id="de485-244">enablepreauthentication 認証</span><span class="sxs-lookup"><span data-stu-id="de485-244">enablePreAuthentication</span></span>|<span data-ttu-id="de485-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="de485-245">Boolean</span></span>|<span data-ttu-id="de485-246">事前認証を有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-246">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="de485-247">maximumpreauthenticationattempts</span><span class="sxs-lookup"><span data-stu-id="de485-247">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="de485-248">Int32</span><span class="sxs-lookup"><span data-stu-id="de485-248">Int32</span></span>|<span data-ttu-id="de485-249">事前認証の最大試行回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-249">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="de485-250">有効な範囲: 1-16</span><span class="sxs-lookup"><span data-stu-id="de485-250">Valid range: 1-16</span></span>|
|<span data-ttu-id="de485-251">eaptype</span><span class="sxs-lookup"><span data-stu-id="de485-251">eapType</span></span>|[<span data-ttu-id="de485-252">eaptype</span><span class="sxs-lookup"><span data-stu-id="de485-252">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="de485-253">拡張認証プロトコル (EAP)。</span><span class="sxs-lookup"><span data-stu-id="de485-253">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="de485-254">wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="de485-254">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="de485-255">可能な値は `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` です。</span><span class="sxs-lookup"><span data-stu-id="de485-255">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="de485-256">trustedserverの形式</span><span class="sxs-lookup"><span data-stu-id="de485-256">trustedServerCertificateNames</span></span>|<span data-ttu-id="de485-257">String collection</span><span class="sxs-lookup"><span data-stu-id="de485-257">String collection</span></span>|<span data-ttu-id="de485-258">信頼されたサーバー証明書の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-258">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="de485-259">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="de485-259">authenticationMethod</span></span>|[<span data-ttu-id="de485-260">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="de485-260">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="de485-261">認証方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-261">Specify the authentication method.</span></span> <span data-ttu-id="de485-262">可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="de485-262">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="de485-263">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="de485-263">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="de485-264">none apauthenticationmethod_ apttlstype</span><span class="sxs-lookup"><span data-stu-id="de485-264">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="de485-265">EAP TTLS の内部認証プロトコルを指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-265">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="de485-266">可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="de485-266">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="de485-267">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="de485-267">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="de485-268">String</span><span class="sxs-lookup"><span data-stu-id="de485-268">String</span></span>|<span data-ttu-id="de485-269">EAP TTLS または PEAP を使用している場合は、プライバシー保護のために、ユーザー名を置換する文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="de485-269">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="de485-270">応答</span><span class="sxs-lookup"><span data-stu-id="de485-270">Response</span></span>
<span data-ttu-id="de485-271">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="de485-271">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de485-272">例</span><span class="sxs-lookup"><span data-stu-id="de485-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="de485-273">要求</span><span class="sxs-lookup"><span data-stu-id="de485-273">Request</span></span>
<span data-ttu-id="de485-274">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de485-274">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="de485-275">応答</span><span class="sxs-lookup"><span data-stu-id="de485-275">Response</span></span>
<span data-ttu-id="de485-p131">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de485-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1676

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
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
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





