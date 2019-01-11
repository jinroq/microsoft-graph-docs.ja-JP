---
title: WindowsWifiConfiguration を更新します。
description: WindowsWifiConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c58ede51940c1d913632668919532ba6d61ad201
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847111"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="29d31-103">WindowsWifiConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="29d31-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="29d31-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29d31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29d31-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29d31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29d31-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29d31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29d31-107">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="29d31-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29d31-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="29d31-108">Prerequisites</span></span>
<span data-ttu-id="29d31-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29d31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d31-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29d31-111">Permission type</span></span>|<span data-ttu-id="29d31-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="29d31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29d31-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29d31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29d31-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29d31-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29d31-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29d31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29d31-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29d31-116">Not supported.</span></span>|
|<span data-ttu-id="29d31-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29d31-117">Application</span></span>|<span data-ttu-id="29d31-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29d31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29d31-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29d31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29d31-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29d31-120">Request headers</span></span>
|<span data-ttu-id="29d31-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29d31-121">Header</span></span>|<span data-ttu-id="29d31-122">値</span><span class="sxs-lookup"><span data-stu-id="29d31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29d31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29d31-123">Authorization</span></span>|<span data-ttu-id="29d31-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="29d31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29d31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="29d31-125">Accept</span></span>|<span data-ttu-id="29d31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29d31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29d31-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="29d31-127">Request body</span></span>
<span data-ttu-id="29d31-128">要求の本文に[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="29d31-129">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="29d31-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="29d31-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29d31-130">Property</span></span>|<span data-ttu-id="29d31-131">種類</span><span class="sxs-lookup"><span data-stu-id="29d31-131">Type</span></span>|<span data-ttu-id="29d31-132">説明</span><span class="sxs-lookup"><span data-stu-id="29d31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29d31-133">ID</span><span class="sxs-lookup"><span data-stu-id="29d31-133">id</span></span>|<span data-ttu-id="29d31-134">String</span><span class="sxs-lookup"><span data-stu-id="29d31-134">String</span></span>|<span data-ttu-id="29d31-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="29d31-135">Key of the entity.</span></span> <span data-ttu-id="29d31-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29d31-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29d31-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29d31-137">lastModifiedDateTime</span></span>|<span data-ttu-id="29d31-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29d31-138">DateTimeOffset</span></span>|<span data-ttu-id="29d31-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="29d31-139">DateTime the object was last modified.</span></span> <span data-ttu-id="29d31-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29d31-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29d31-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="29d31-141">roleScopeTagIds</span></span>|<span data-ttu-id="29d31-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="29d31-142">String collection</span></span>|<span data-ttu-id="29d31-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="29d31-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="29d31-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29d31-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29d31-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="29d31-145">supportsScopeTags</span></span>|<span data-ttu-id="29d31-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="29d31-146">Boolean</span></span>|<span data-ttu-id="29d31-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29d31-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="29d31-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="29d31-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="29d31-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="29d31-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="29d31-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="29d31-150">This property is read-only.</span></span> <span data-ttu-id="29d31-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29d31-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29d31-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29d31-152">createdDateTime</span></span>|<span data-ttu-id="29d31-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29d31-153">DateTimeOffset</span></span>|<span data-ttu-id="29d31-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="29d31-154">DateTime the object was created.</span></span> <span data-ttu-id="29d31-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29d31-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29d31-156">説明</span><span class="sxs-lookup"><span data-stu-id="29d31-156">description</span></span>|<span data-ttu-id="29d31-157">String</span><span class="sxs-lookup"><span data-stu-id="29d31-157">String</span></span>|<span data-ttu-id="29d31-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="29d31-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="29d31-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29d31-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29d31-160">displayName</span><span class="sxs-lookup"><span data-stu-id="29d31-160">displayName</span></span>|<span data-ttu-id="29d31-161">String</span><span class="sxs-lookup"><span data-stu-id="29d31-161">String</span></span>|<span data-ttu-id="29d31-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="29d31-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="29d31-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29d31-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29d31-164">version</span><span class="sxs-lookup"><span data-stu-id="29d31-164">version</span></span>|<span data-ttu-id="29d31-165">Int32</span><span class="sxs-lookup"><span data-stu-id="29d31-165">Int32</span></span>|<span data-ttu-id="29d31-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="29d31-166">Version of the device configuration.</span></span> <span data-ttu-id="29d31-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29d31-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29d31-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="29d31-168">preSharedKey</span></span>|<span data-ttu-id="29d31-169">String</span><span class="sxs-lookup"><span data-stu-id="29d31-169">String</span></span>|<span data-ttu-id="29d31-170">これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="29d31-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="29d31-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="29d31-171">wifiSecurityType</span></span>|[<span data-ttu-id="29d31-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="29d31-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="29d31-173">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="29d31-174">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="29d31-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="29d31-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="29d31-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="29d31-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="29d31-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="29d31-177">Wifi 接続のメータリングされた接続の制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="29d31-178">可能な値は、`unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="29d31-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="29d31-179">ssid</span><span class="sxs-lookup"><span data-stu-id="29d31-179">ssid</span></span>|<span data-ttu-id="29d31-180">String</span><span class="sxs-lookup"><span data-stu-id="29d31-180">String</span></span>|<span data-ttu-id="29d31-181">Wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="29d31-182">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="29d31-182">networkName</span></span>|<span data-ttu-id="29d31-183">String</span><span class="sxs-lookup"><span data-stu-id="29d31-183">String</span></span>|<span data-ttu-id="29d31-184">ネットワーク構成の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="29d31-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="29d31-185">connectAutomatically</span></span>|<span data-ttu-id="29d31-186">ブール型</span><span class="sxs-lookup"><span data-stu-id="29d31-186">Boolean</span></span>|<span data-ttu-id="29d31-187">範囲で wifi 接続が自動的に接続する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="29d31-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="29d31-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="29d31-189">ブール型</span><span class="sxs-lookup"><span data-stu-id="29d31-189">Boolean</span></span>|<span data-ttu-id="29d31-190">Wifi 接続は、この 1 つに既に接続されている場合より優先するネットワークに接続する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="29d31-191">True を指定する ConnectAutomatically が必要です。</span><span class="sxs-lookup"><span data-stu-id="29d31-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="29d31-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="29d31-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="29d31-193">ブール型</span><span class="sxs-lookup"><span data-stu-id="29d31-193">Boolean</span></span>|<span data-ttu-id="29d31-194">かどうか、wifi 接続自動的にでもすると、SSID をブロードキャストしていないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="29d31-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="29d31-195">proxySetting</span></span>|[<span data-ttu-id="29d31-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="29d31-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="29d31-197">Wi-fi 構成のプロキシ設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="29d31-198">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="29d31-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="29d31-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="29d31-199">proxyManualAddress</span></span>|<span data-ttu-id="29d31-200">String</span><span class="sxs-lookup"><span data-stu-id="29d31-200">String</span></span>|<span data-ttu-id="29d31-201">プロキシ サーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="29d31-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="29d31-202">proxyManualPort</span></span>|<span data-ttu-id="29d31-203">Int32</span><span class="sxs-lookup"><span data-stu-id="29d31-203">Int32</span></span>|<span data-ttu-id="29d31-204">プロキシ サーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="29d31-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="29d31-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="29d31-206">String</span><span class="sxs-lookup"><span data-stu-id="29d31-206">String</span></span>|<span data-ttu-id="29d31-207">プロキシ サーバーの構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="29d31-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="29d31-208">forceFIPSCompliance</span></span>|<span data-ttu-id="29d31-209">ブール型</span><span class="sxs-lookup"><span data-stu-id="29d31-209">Boolean</span></span>|<span data-ttu-id="29d31-210">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="29d31-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="29d31-211">応答</span><span class="sxs-lookup"><span data-stu-id="29d31-211">Response</span></span>
<span data-ttu-id="29d31-212">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="29d31-212">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29d31-213">例</span><span class="sxs-lookup"><span data-stu-id="29d31-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="29d31-214">要求</span><span class="sxs-lookup"><span data-stu-id="29d31-214">Request</span></span>
<span data-ttu-id="29d31-215">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29d31-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 787

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="29d31-216">応答</span><span class="sxs-lookup"><span data-stu-id="29d31-216">Response</span></span>
<span data-ttu-id="29d31-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29d31-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





