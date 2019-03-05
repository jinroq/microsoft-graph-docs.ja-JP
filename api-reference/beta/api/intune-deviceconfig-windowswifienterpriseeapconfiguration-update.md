---
title: windowsWifiEnterpriseEAPConfiguration の更新
description: windowsWifiEnterpriseEAPConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 401dcfcc24b5b528d4c85c661993682fbf3bbfa3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141301"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="c0179-103">windowsWifiEnterpriseEAPConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="c0179-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="c0179-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0179-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0179-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0179-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0179-106">[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c0179-106">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0179-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c0179-107">Prerequisites</span></span>
<span data-ttu-id="c0179-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c0179-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0179-110">Permission type</span></span>|<span data-ttu-id="c0179-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0179-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0179-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0179-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0179-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0179-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0179-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0179-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0179-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0179-115">Not supported.</span></span>|
|<span data-ttu-id="c0179-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0179-116">Application</span></span>|<span data-ttu-id="c0179-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0179-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0179-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0179-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c0179-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0179-119">Request headers</span></span>
|<span data-ttu-id="c0179-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0179-120">Header</span></span>|<span data-ttu-id="c0179-121">値</span><span class="sxs-lookup"><span data-stu-id="c0179-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0179-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0179-122">Authorization</span></span>|<span data-ttu-id="c0179-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c0179-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0179-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c0179-124">Accept</span></span>|<span data-ttu-id="c0179-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0179-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0179-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0179-126">Request body</span></span>
<span data-ttu-id="c0179-127">要求本文で、 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-127">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="c0179-128">次の表に、 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c0179-128">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="c0179-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0179-129">Property</span></span>|<span data-ttu-id="c0179-130">型</span><span class="sxs-lookup"><span data-stu-id="c0179-130">Type</span></span>|<span data-ttu-id="c0179-131">説明</span><span class="sxs-lookup"><span data-stu-id="c0179-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0179-132">id</span><span class="sxs-lookup"><span data-stu-id="c0179-132">id</span></span>|<span data-ttu-id="c0179-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c0179-133">String</span></span>|<span data-ttu-id="c0179-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c0179-134">Key of the entity.</span></span> <span data-ttu-id="c0179-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0179-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0179-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0179-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c0179-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0179-137">DateTimeOffset</span></span>|<span data-ttu-id="c0179-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c0179-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c0179-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0179-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0179-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c0179-140">roleScopeTagIds</span></span>|<span data-ttu-id="c0179-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c0179-141">String collection</span></span>|<span data-ttu-id="c0179-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c0179-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c0179-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0179-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0179-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c0179-144">supportsScopeTags</span></span>|<span data-ttu-id="c0179-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0179-145">Boolean</span></span>|<span data-ttu-id="c0179-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0179-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c0179-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="c0179-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c0179-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="c0179-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c0179-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c0179-149">This property is read-only.</span></span> <span data-ttu-id="c0179-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0179-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0179-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0179-151">createdDateTime</span></span>|<span data-ttu-id="c0179-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0179-152">DateTimeOffset</span></span>|<span data-ttu-id="c0179-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c0179-153">DateTime the object was created.</span></span> <span data-ttu-id="c0179-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0179-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0179-155">説明</span><span class="sxs-lookup"><span data-stu-id="c0179-155">description</span></span>|<span data-ttu-id="c0179-156">String</span><span class="sxs-lookup"><span data-stu-id="c0179-156">String</span></span>|<span data-ttu-id="c0179-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c0179-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c0179-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0179-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0179-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c0179-159">displayName</span></span>|<span data-ttu-id="c0179-160">String</span><span class="sxs-lookup"><span data-stu-id="c0179-160">String</span></span>|<span data-ttu-id="c0179-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c0179-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c0179-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0179-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0179-163">version</span><span class="sxs-lookup"><span data-stu-id="c0179-163">version</span></span>|<span data-ttu-id="c0179-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c0179-164">Int32</span></span>|<span data-ttu-id="c0179-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c0179-165">Version of the device configuration.</span></span> <span data-ttu-id="c0179-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0179-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0179-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="c0179-167">preSharedKey</span></span>|<span data-ttu-id="c0179-168">String</span><span class="sxs-lookup"><span data-stu-id="c0179-168">String</span></span>|<span data-ttu-id="c0179-169">これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="c0179-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="c0179-170">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-170">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c0179-171">wifiSecurityType</span></span>|[<span data-ttu-id="c0179-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c0179-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="c0179-173">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="c0179-174">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c0179-174">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c0179-175">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="c0179-175">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="c0179-176">meteredconnectionlimit</span><span class="sxs-lookup"><span data-stu-id="c0179-176">meteredConnectionLimit</span></span>|[<span data-ttu-id="c0179-177">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="c0179-177">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="c0179-178">wifi 接続の従量制課金接続制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-178">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="c0179-179">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c0179-179">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c0179-180">可能な値は `unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="c0179-180">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="c0179-181">ssid</span><span class="sxs-lookup"><span data-stu-id="c0179-181">ssid</span></span>|<span data-ttu-id="c0179-182">String</span><span class="sxs-lookup"><span data-stu-id="c0179-182">String</span></span>|<span data-ttu-id="c0179-183">wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-183">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="c0179-184">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-184">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-185">networkname</span><span class="sxs-lookup"><span data-stu-id="c0179-185">networkName</span></span>|<span data-ttu-id="c0179-186">String</span><span class="sxs-lookup"><span data-stu-id="c0179-186">String</span></span>|<span data-ttu-id="c0179-187">ネットワーク構成名を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-187">Specify the network configuration name.</span></span> <span data-ttu-id="c0179-188">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-188">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-189">connectautomatically に</span><span class="sxs-lookup"><span data-stu-id="c0179-189">connectAutomatically</span></span>|<span data-ttu-id="c0179-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0179-190">Boolean</span></span>|<span data-ttu-id="c0179-191">範囲内で wifi 接続を自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-191">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="c0179-192">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-193">connecttopreferrednetwork</span><span class="sxs-lookup"><span data-stu-id="c0179-193">connectToPreferredNetwork</span></span>|<span data-ttu-id="c0179-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0179-194">Boolean</span></span>|<span data-ttu-id="c0179-195">この接続に既に接続されている場合に、wifi 接続がより優先度の高いネットワークに接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-195">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="c0179-196">connectautomatically 自動的に true になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0179-196">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="c0179-197">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-198">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="c0179-198">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c0179-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0179-199">Boolean</span></span>|<span data-ttu-id="c0179-200">SSID がブロードキャストされていない場合でも、wifi 接続が自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-200">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="c0179-201">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-202">proxysetting</span><span class="sxs-lookup"><span data-stu-id="c0179-202">proxySetting</span></span>|[<span data-ttu-id="c0179-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="c0179-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="c0179-204">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承した wi-fi 構成のプロキシ設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-204">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="c0179-205">可能な値は `none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="c0179-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="c0179-206">proxymanualaddress</span><span class="sxs-lookup"><span data-stu-id="c0179-206">proxyManualAddress</span></span>|<span data-ttu-id="c0179-207">String</span><span class="sxs-lookup"><span data-stu-id="c0179-207">String</span></span>|<span data-ttu-id="c0179-208">プロキシサーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-208">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="c0179-209">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-210">proxymanualport</span><span class="sxs-lookup"><span data-stu-id="c0179-210">proxyManualPort</span></span>|<span data-ttu-id="c0179-211">Int32</span><span class="sxs-lookup"><span data-stu-id="c0179-211">Int32</span></span>|<span data-ttu-id="c0179-212">プロキシサーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-212">Specify the port for the proxy server.</span></span> <span data-ttu-id="c0179-213">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="c0179-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="c0179-215">String</span><span class="sxs-lookup"><span data-stu-id="c0179-215">String</span></span>|<span data-ttu-id="c0179-216">プロキシサーバー構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-216">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="c0179-217">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-217">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-218">forcefipscompliance</span><span class="sxs-lookup"><span data-stu-id="c0179-218">forceFIPSCompliance</span></span>|<span data-ttu-id="c0179-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0179-219">Boolean</span></span>|<span data-ttu-id="c0179-220">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-220">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="c0179-221">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0179-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="c0179-222">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="c0179-222">networkSingleSignOn</span></span>|[<span data-ttu-id="c0179-223">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="c0179-223">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="c0179-224">ネットワークのシングルサインオンの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-224">Specify the network single sign on type.</span></span> <span data-ttu-id="c0179-225">可能な値は `disabled`、`prelogon`、`postlogon` です。</span><span class="sxs-lookup"><span data-stu-id="c0179-225">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="c0179-226">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="c0179-226">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="c0179-227">Int32</span><span class="sxs-lookup"><span data-stu-id="c0179-227">Int32</span></span>|<span data-ttu-id="c0179-228">[最大認証タイムアウト (秒)] を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-228">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="c0179-229">有効な範囲: 1-120</span><span class="sxs-lookup"><span data-stu-id="c0179-229">Valid range: 1-120</span></span>|
|<span data-ttu-id="c0179-230">promptforadditionalauthenticationcredentials</span><span class="sxs-lookup"><span data-stu-id="c0179-230">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="c0179-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0179-231">Boolean</span></span>|<span data-ttu-id="c0179-232">wifi 接続で追加の認証資格情報を求めるメッセージを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-232">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="c0179-233">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="c0179-233">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="c0179-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0179-234">Boolean</span></span>|<span data-ttu-id="c0179-235">wifi 接続で、ペアワイズマスターキーのキャッシュを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-235">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="c0179-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="c0179-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="c0179-237">Int32</span><span class="sxs-lookup"><span data-stu-id="c0179-237">Int32</span></span>|<span data-ttu-id="c0179-238">最大ペアワイズマスターキーキャッシュ時間を指定します (分単位)。</span><span class="sxs-lookup"><span data-stu-id="c0179-238">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="c0179-239">有効な範囲: 5-1440</span><span class="sxs-lookup"><span data-stu-id="c0179-239">Valid range: 5-1440</span></span>|
|<span data-ttu-id="c0179-240">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="c0179-240">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="c0179-241">Int32</span><span class="sxs-lookup"><span data-stu-id="c0179-241">Int32</span></span>|<span data-ttu-id="c0179-242">キャッシュ内のペアワイズマスターキーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-242">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="c0179-243">有効な範囲: 1-255</span><span class="sxs-lookup"><span data-stu-id="c0179-243">Valid range: 1-255</span></span>|
|<span data-ttu-id="c0179-244">enablepreauthentication 認証</span><span class="sxs-lookup"><span data-stu-id="c0179-244">enablePreAuthentication</span></span>|<span data-ttu-id="c0179-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0179-245">Boolean</span></span>|<span data-ttu-id="c0179-246">事前認証を有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-246">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="c0179-247">maximumpreauthenticationattempts</span><span class="sxs-lookup"><span data-stu-id="c0179-247">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="c0179-248">Int32</span><span class="sxs-lookup"><span data-stu-id="c0179-248">Int32</span></span>|<span data-ttu-id="c0179-249">事前認証の最大試行回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-249">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="c0179-250">有効な範囲: 1-16</span><span class="sxs-lookup"><span data-stu-id="c0179-250">Valid range: 1-16</span></span>|
|<span data-ttu-id="c0179-251">eaptype</span><span class="sxs-lookup"><span data-stu-id="c0179-251">eapType</span></span>|[<span data-ttu-id="c0179-252">eaptype</span><span class="sxs-lookup"><span data-stu-id="c0179-252">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="c0179-253">拡張認証プロトコル (EAP)。</span><span class="sxs-lookup"><span data-stu-id="c0179-253">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="c0179-254">wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="c0179-254">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="c0179-255">使用可能な値: `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="c0179-255">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="c0179-256">trustedserverの形式</span><span class="sxs-lookup"><span data-stu-id="c0179-256">trustedServerCertificateNames</span></span>|<span data-ttu-id="c0179-257">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c0179-257">String collection</span></span>|<span data-ttu-id="c0179-258">信頼されたサーバー証明書の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-258">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="c0179-259">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c0179-259">authenticationMethod</span></span>|[<span data-ttu-id="c0179-260">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c0179-260">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="c0179-261">認証方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-261">Specify the authentication method.</span></span> <span data-ttu-id="c0179-262">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="c0179-262">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="c0179-263">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="c0179-263">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="c0179-264">none apauthenticationmethod_ apttlstype</span><span class="sxs-lookup"><span data-stu-id="c0179-264">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="c0179-265">EAP TTLS の内部認証プロトコルを指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-265">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="c0179-266">使用可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="c0179-266">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c0179-267">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="c0179-267">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="c0179-268">String</span><span class="sxs-lookup"><span data-stu-id="c0179-268">String</span></span>|<span data-ttu-id="c0179-269">EAP TTLS または PEAP を使用している場合は、プライバシー保護のために、ユーザー名を置換する文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0179-269">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="c0179-270">応答</span><span class="sxs-lookup"><span data-stu-id="c0179-270">Response</span></span>
<span data-ttu-id="c0179-271">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c0179-271">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0179-272">例</span><span class="sxs-lookup"><span data-stu-id="c0179-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0179-273">要求</span><span class="sxs-lookup"><span data-stu-id="c0179-273">Request</span></span>
<span data-ttu-id="c0179-274">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0179-274">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c0179-275">応答</span><span class="sxs-lookup"><span data-stu-id="c0179-275">Response</span></span>
<span data-ttu-id="c0179-p131">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0179-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




