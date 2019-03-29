---
title: windowsWifiEnterpriseEAPConfiguration の更新
description: windowsWifiEnterpriseEAPConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38b16bf4acaa71063c132836a9285fb570502fdc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961267"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="0a2f9-103">windowsWifiEnterpriseEAPConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="0a2f9-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="0a2f9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a2f9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a2f9-106">[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-106">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a2f9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0a2f9-107">Prerequisites</span></span>
<span data-ttu-id="0a2f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a2f9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a2f9-110">Permission type</span></span>|<span data-ttu-id="0a2f9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a2f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a2f9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a2f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a2f9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a2f9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a2f9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a2f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a2f9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-115">Not supported.</span></span>|
|<span data-ttu-id="0a2f9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a2f9-116">Application</span></span>|<span data-ttu-id="0a2f9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a2f9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a2f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0a2f9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a2f9-119">Request headers</span></span>
|<span data-ttu-id="0a2f9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a2f9-120">Header</span></span>|<span data-ttu-id="0a2f9-121">値</span><span class="sxs-lookup"><span data-stu-id="0a2f9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a2f9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a2f9-122">Authorization</span></span>|<span data-ttu-id="0a2f9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a2f9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0a2f9-124">Accept</span></span>|<span data-ttu-id="0a2f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a2f9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a2f9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a2f9-126">Request body</span></span>
<span data-ttu-id="0a2f9-127">要求本文で、 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-127">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="0a2f9-128">次の表に、 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-128">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="0a2f9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a2f9-129">Property</span></span>|<span data-ttu-id="0a2f9-130">型</span><span class="sxs-lookup"><span data-stu-id="0a2f9-130">Type</span></span>|<span data-ttu-id="0a2f9-131">説明</span><span class="sxs-lookup"><span data-stu-id="0a2f9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a2f9-132">id</span><span class="sxs-lookup"><span data-stu-id="0a2f9-132">id</span></span>|<span data-ttu-id="0a2f9-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0a2f9-133">String</span></span>|<span data-ttu-id="0a2f9-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-134">Key of the entity.</span></span> <span data-ttu-id="0a2f9-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a2f9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a2f9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0a2f9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a2f9-137">DateTimeOffset</span></span>|<span data-ttu-id="0a2f9-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0a2f9-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a2f9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a2f9-140">roleScopeTagIds</span></span>|<span data-ttu-id="0a2f9-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0a2f9-141">String collection</span></span>|<span data-ttu-id="0a2f9-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0a2f9-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a2f9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0a2f9-144">supportsScopeTags</span></span>|<span data-ttu-id="0a2f9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2f9-145">Boolean</span></span>|<span data-ttu-id="0a2f9-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0a2f9-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0a2f9-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0a2f9-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-149">This property is read-only.</span></span> <span data-ttu-id="0a2f9-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a2f9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a2f9-151">createdDateTime</span></span>|<span data-ttu-id="0a2f9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a2f9-152">DateTimeOffset</span></span>|<span data-ttu-id="0a2f9-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-153">DateTime the object was created.</span></span> <span data-ttu-id="0a2f9-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a2f9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-155">description</span><span class="sxs-lookup"><span data-stu-id="0a2f9-155">description</span></span>|<span data-ttu-id="0a2f9-156">String</span><span class="sxs-lookup"><span data-stu-id="0a2f9-156">String</span></span>|<span data-ttu-id="0a2f9-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a2f9-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a2f9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0a2f9-159">displayName</span></span>|<span data-ttu-id="0a2f9-160">String</span><span class="sxs-lookup"><span data-stu-id="0a2f9-160">String</span></span>|<span data-ttu-id="0a2f9-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a2f9-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a2f9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-163">version</span><span class="sxs-lookup"><span data-stu-id="0a2f9-163">version</span></span>|<span data-ttu-id="0a2f9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0a2f9-164">Int32</span></span>|<span data-ttu-id="0a2f9-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-165">Version of the device configuration.</span></span> <span data-ttu-id="0a2f9-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a2f9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="0a2f9-167">preSharedKey</span></span>|<span data-ttu-id="0a2f9-168">String</span><span class="sxs-lookup"><span data-stu-id="0a2f9-168">String</span></span>|<span data-ttu-id="0a2f9-169">これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="0a2f9-170">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-170">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0a2f9-171">wifiSecurityType</span></span>|[<span data-ttu-id="0a2f9-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0a2f9-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="0a2f9-173">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="0a2f9-174">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-174">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="0a2f9-175">可能な値は `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-175">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="0a2f9-176">meteredconnectionlimit</span><span class="sxs-lookup"><span data-stu-id="0a2f9-176">meteredConnectionLimit</span></span>|[<span data-ttu-id="0a2f9-177">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="0a2f9-177">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="0a2f9-178">wifi 接続の従量制課金接続制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-178">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="0a2f9-179">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-179">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="0a2f9-180">使用可能な値は、`unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-180">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="0a2f9-181">ssid</span><span class="sxs-lookup"><span data-stu-id="0a2f9-181">ssid</span></span>|<span data-ttu-id="0a2f9-182">String</span><span class="sxs-lookup"><span data-stu-id="0a2f9-182">String</span></span>|<span data-ttu-id="0a2f9-183">wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-183">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="0a2f9-184">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-184">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-185">networkname</span><span class="sxs-lookup"><span data-stu-id="0a2f9-185">networkName</span></span>|<span data-ttu-id="0a2f9-186">String</span><span class="sxs-lookup"><span data-stu-id="0a2f9-186">String</span></span>|<span data-ttu-id="0a2f9-187">ネットワーク構成名を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-187">Specify the network configuration name.</span></span> <span data-ttu-id="0a2f9-188">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-188">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-189">connectautomatically に</span><span class="sxs-lookup"><span data-stu-id="0a2f9-189">connectAutomatically</span></span>|<span data-ttu-id="0a2f9-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2f9-190">Boolean</span></span>|<span data-ttu-id="0a2f9-191">範囲内で wifi 接続を自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-191">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="0a2f9-192">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-193">connecttopreferrednetwork</span><span class="sxs-lookup"><span data-stu-id="0a2f9-193">connectToPreferredNetwork</span></span>|<span data-ttu-id="0a2f9-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2f9-194">Boolean</span></span>|<span data-ttu-id="0a2f9-195">この接続に既に接続されている場合に、wifi 接続がより優先度の高いネットワークに接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-195">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="0a2f9-196">connectautomatically 自動的に true になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-196">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="0a2f9-197">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-198">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0a2f9-198">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0a2f9-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2f9-199">Boolean</span></span>|<span data-ttu-id="0a2f9-200">SSID がブロードキャストされていない場合でも、wifi 接続が自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-200">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="0a2f9-201">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-202">proxysetting</span><span class="sxs-lookup"><span data-stu-id="0a2f9-202">proxySetting</span></span>|[<span data-ttu-id="0a2f9-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="0a2f9-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="0a2f9-204">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承した wi-fi 構成のプロキシ設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-204">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="0a2f9-205">使用可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="0a2f9-206">proxymanualaddress</span><span class="sxs-lookup"><span data-stu-id="0a2f9-206">proxyManualAddress</span></span>|<span data-ttu-id="0a2f9-207">String</span><span class="sxs-lookup"><span data-stu-id="0a2f9-207">String</span></span>|<span data-ttu-id="0a2f9-208">プロキシサーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-208">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="0a2f9-209">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-210">proxymanualport</span><span class="sxs-lookup"><span data-stu-id="0a2f9-210">proxyManualPort</span></span>|<span data-ttu-id="0a2f9-211">Int32</span><span class="sxs-lookup"><span data-stu-id="0a2f9-211">Int32</span></span>|<span data-ttu-id="0a2f9-212">プロキシサーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-212">Specify the port for the proxy server.</span></span> <span data-ttu-id="0a2f9-213">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="0a2f9-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="0a2f9-215">String</span><span class="sxs-lookup"><span data-stu-id="0a2f9-215">String</span></span>|<span data-ttu-id="0a2f9-216">プロキシサーバー構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-216">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="0a2f9-217">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-217">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-218">forcefipscompliance</span><span class="sxs-lookup"><span data-stu-id="0a2f9-218">forceFIPSCompliance</span></span>|<span data-ttu-id="0a2f9-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2f9-219">Boolean</span></span>|<span data-ttu-id="0a2f9-220">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-220">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="0a2f9-221">[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="0a2f9-222">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="0a2f9-222">networkSingleSignOn</span></span>|[<span data-ttu-id="0a2f9-223">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="0a2f9-223">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="0a2f9-224">ネットワークのシングルサインオンの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-224">Specify the network single sign on type.</span></span> <span data-ttu-id="0a2f9-225">使用可能な値は、`disabled`、`prelogon`、`postlogon` です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-225">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="0a2f9-226">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="0a2f9-226">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="0a2f9-227">Int32</span><span class="sxs-lookup"><span data-stu-id="0a2f9-227">Int32</span></span>|<span data-ttu-id="0a2f9-228">[最大認証タイムアウト (秒)] を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-228">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="0a2f9-229">有効な範囲: 1-120</span><span class="sxs-lookup"><span data-stu-id="0a2f9-229">Valid range: 1-120</span></span>|
|<span data-ttu-id="0a2f9-230">promptforadditionalauthenticationcredentials</span><span class="sxs-lookup"><span data-stu-id="0a2f9-230">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="0a2f9-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2f9-231">Boolean</span></span>|<span data-ttu-id="0a2f9-232">wifi 接続で追加の認証資格情報を求めるメッセージを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-232">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="0a2f9-233">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="0a2f9-233">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="0a2f9-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2f9-234">Boolean</span></span>|<span data-ttu-id="0a2f9-235">wifi 接続で、ペアワイズマスターキーのキャッシュを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-235">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="0a2f9-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="0a2f9-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="0a2f9-237">Int32</span><span class="sxs-lookup"><span data-stu-id="0a2f9-237">Int32</span></span>|<span data-ttu-id="0a2f9-238">最大ペアワイズマスターキーキャッシュ時間を指定します (分単位)。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-238">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="0a2f9-239">有効な範囲: 5-1440</span><span class="sxs-lookup"><span data-stu-id="0a2f9-239">Valid range: 5-1440</span></span>|
|<span data-ttu-id="0a2f9-240">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="0a2f9-240">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="0a2f9-241">Int32</span><span class="sxs-lookup"><span data-stu-id="0a2f9-241">Int32</span></span>|<span data-ttu-id="0a2f9-242">キャッシュ内のペアワイズマスターキーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-242">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="0a2f9-243">有効な範囲: 1-255</span><span class="sxs-lookup"><span data-stu-id="0a2f9-243">Valid range: 1-255</span></span>|
|<span data-ttu-id="0a2f9-244">enablepreauthentication 認証</span><span class="sxs-lookup"><span data-stu-id="0a2f9-244">enablePreAuthentication</span></span>|<span data-ttu-id="0a2f9-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2f9-245">Boolean</span></span>|<span data-ttu-id="0a2f9-246">事前認証を有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-246">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="0a2f9-247">maximumpreauthenticationattempts</span><span class="sxs-lookup"><span data-stu-id="0a2f9-247">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="0a2f9-248">Int32</span><span class="sxs-lookup"><span data-stu-id="0a2f9-248">Int32</span></span>|<span data-ttu-id="0a2f9-249">事前認証の最大試行回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-249">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="0a2f9-250">有効な範囲: 1-16</span><span class="sxs-lookup"><span data-stu-id="0a2f9-250">Valid range: 1-16</span></span>|
|<span data-ttu-id="0a2f9-251">eaptype</span><span class="sxs-lookup"><span data-stu-id="0a2f9-251">eapType</span></span>|[<span data-ttu-id="0a2f9-252">eaptype</span><span class="sxs-lookup"><span data-stu-id="0a2f9-252">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="0a2f9-253">拡張認証プロトコル (EAP)。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-253">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="0a2f9-254">wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-254">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="0a2f9-255">可能な値は `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-255">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="0a2f9-256">trustedserverの形式</span><span class="sxs-lookup"><span data-stu-id="0a2f9-256">trustedServerCertificateNames</span></span>|<span data-ttu-id="0a2f9-257">String collection</span><span class="sxs-lookup"><span data-stu-id="0a2f9-257">String collection</span></span>|<span data-ttu-id="0a2f9-258">信頼されたサーバー証明書の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-258">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="0a2f9-259">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0a2f9-259">authenticationMethod</span></span>|[<span data-ttu-id="0a2f9-260">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0a2f9-260">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="0a2f9-261">認証方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-261">Specify the authentication method.</span></span> <span data-ttu-id="0a2f9-262">可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-262">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="0a2f9-263">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="0a2f9-263">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="0a2f9-264">none apauthenticationmethod_ apttlstype</span><span class="sxs-lookup"><span data-stu-id="0a2f9-264">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="0a2f9-265">EAP TTLS の内部認証プロトコルを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-265">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="0a2f9-266">可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-266">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="0a2f9-267">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="0a2f9-267">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="0a2f9-268">String</span><span class="sxs-lookup"><span data-stu-id="0a2f9-268">String</span></span>|<span data-ttu-id="0a2f9-269">EAP TTLS または PEAP を使用している場合は、プライバシー保護のために、ユーザー名を置換する文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-269">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="0a2f9-270">応答</span><span class="sxs-lookup"><span data-stu-id="0a2f9-270">Response</span></span>
<span data-ttu-id="0a2f9-271">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-271">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a2f9-272">例</span><span class="sxs-lookup"><span data-stu-id="0a2f9-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a2f9-273">要求</span><span class="sxs-lookup"><span data-stu-id="0a2f9-273">Request</span></span>
<span data-ttu-id="0a2f9-274">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-274">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a2f9-275">応答</span><span class="sxs-lookup"><span data-stu-id="0a2f9-275">Response</span></span>
<span data-ttu-id="0a2f9-p131">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a2f9-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




