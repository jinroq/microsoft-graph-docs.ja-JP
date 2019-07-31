---
title: WindowsWifiConfiguration を作成する
description: 新しい windowsWifiConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06b16d33dc96c283c73f89f6f412a59f44c352a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981858"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="7e2ed-103">WindowsWifiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="7e2ed-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="7e2ed-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e2ed-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e2ed-106">新しい[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-106">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e2ed-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e2ed-107">Prerequisites</span></span>
<span data-ttu-id="7e2ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e2ed-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e2ed-110">Permission type</span></span>|<span data-ttu-id="7e2ed-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e2ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e2ed-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e2ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e2ed-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2ed-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e2ed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e2ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e2ed-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-115">Not supported.</span></span>|
|<span data-ttu-id="7e2ed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e2ed-116">Application</span></span>|<span data-ttu-id="7e2ed-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e2ed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e2ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7e2ed-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e2ed-119">Request headers</span></span>
|<span data-ttu-id="7e2ed-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e2ed-120">Header</span></span>|<span data-ttu-id="7e2ed-121">値</span><span class="sxs-lookup"><span data-stu-id="7e2ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e2ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e2ed-122">Authorization</span></span>|<span data-ttu-id="7e2ed-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e2ed-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7e2ed-124">Accept</span></span>|<span data-ttu-id="7e2ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e2ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e2ed-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e2ed-126">Request body</span></span>
<span data-ttu-id="7e2ed-127">要求本文で、windowsWifiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-127">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="7e2ed-128">次の表に、windowsWifiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-128">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="7e2ed-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e2ed-129">Property</span></span>|<span data-ttu-id="7e2ed-130">型</span><span class="sxs-lookup"><span data-stu-id="7e2ed-130">Type</span></span>|<span data-ttu-id="7e2ed-131">説明</span><span class="sxs-lookup"><span data-stu-id="7e2ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e2ed-132">id</span><span class="sxs-lookup"><span data-stu-id="7e2ed-132">id</span></span>|<span data-ttu-id="7e2ed-133">文字列</span><span class="sxs-lookup"><span data-stu-id="7e2ed-133">String</span></span>|<span data-ttu-id="7e2ed-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-134">Key of the entity.</span></span> <span data-ttu-id="7e2ed-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e2ed-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7e2ed-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e2ed-137">DateTimeOffset</span></span>|<span data-ttu-id="7e2ed-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7e2ed-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e2ed-140">roleScopeTagIds</span></span>|<span data-ttu-id="7e2ed-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7e2ed-141">String collection</span></span>|<span data-ttu-id="7e2ed-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7e2ed-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7e2ed-144">supportsScopeTags</span></span>|<span data-ttu-id="7e2ed-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e2ed-145">Boolean</span></span>|<span data-ttu-id="7e2ed-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7e2ed-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7e2ed-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7e2ed-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-149">This property is read-only.</span></span> <span data-ttu-id="7e2ed-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7e2ed-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7e2ed-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7e2ed-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7e2ed-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7e2ed-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7e2ed-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7e2ed-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7e2ed-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7e2ed-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7e2ed-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="7e2ed-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7e2ed-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="7e2ed-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7e2ed-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7e2ed-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e2ed-163">createdDateTime</span></span>|<span data-ttu-id="7e2ed-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e2ed-164">DateTimeOffset</span></span>|<span data-ttu-id="7e2ed-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-165">DateTime the object was created.</span></span> <span data-ttu-id="7e2ed-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-167">description</span><span class="sxs-lookup"><span data-stu-id="7e2ed-167">description</span></span>|<span data-ttu-id="7e2ed-168">String</span><span class="sxs-lookup"><span data-stu-id="7e2ed-168">String</span></span>|<span data-ttu-id="7e2ed-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7e2ed-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7e2ed-171">displayName</span></span>|<span data-ttu-id="7e2ed-172">String</span><span class="sxs-lookup"><span data-stu-id="7e2ed-172">String</span></span>|<span data-ttu-id="7e2ed-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7e2ed-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-175">version</span><span class="sxs-lookup"><span data-stu-id="7e2ed-175">version</span></span>|<span data-ttu-id="7e2ed-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2ed-176">Int32</span></span>|<span data-ttu-id="7e2ed-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-177">Version of the device configuration.</span></span> <span data-ttu-id="7e2ed-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e2ed-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e2ed-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="7e2ed-179">preSharedKey</span></span>|<span data-ttu-id="7e2ed-180">String</span><span class="sxs-lookup"><span data-stu-id="7e2ed-180">String</span></span>|<span data-ttu-id="7e2ed-181">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="7e2ed-182">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="7e2ed-182">wifiSecurityType</span></span>|[<span data-ttu-id="7e2ed-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="7e2ed-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="7e2ed-184">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-184">Specify the Wifi Security Type.</span></span> <span data-ttu-id="7e2ed-185">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="7e2ed-186">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="7e2ed-186">meteredConnectionLimit</span></span>|[<span data-ttu-id="7e2ed-187">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="7e2ed-187">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="7e2ed-188">Wifi 接続の従量制課金接続制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-188">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="7e2ed-189">可能な値は、`unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-189">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="7e2ed-190">ssid</span><span class="sxs-lookup"><span data-stu-id="7e2ed-190">ssid</span></span>|<span data-ttu-id="7e2ed-191">String</span><span class="sxs-lookup"><span data-stu-id="7e2ed-191">String</span></span>|<span data-ttu-id="7e2ed-192">Wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-192">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="7e2ed-193">networkName</span><span class="sxs-lookup"><span data-stu-id="7e2ed-193">networkName</span></span>|<span data-ttu-id="7e2ed-194">String</span><span class="sxs-lookup"><span data-stu-id="7e2ed-194">String</span></span>|<span data-ttu-id="7e2ed-195">ネットワーク構成名を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-195">Specify the network configuration name.</span></span>|
|<span data-ttu-id="7e2ed-196">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="7e2ed-196">connectAutomatically</span></span>|<span data-ttu-id="7e2ed-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e2ed-197">Boolean</span></span>|<span data-ttu-id="7e2ed-198">範囲内で wifi 接続を自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-198">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="7e2ed-199">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="7e2ed-199">connectToPreferredNetwork</span></span>|<span data-ttu-id="7e2ed-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e2ed-200">Boolean</span></span>|<span data-ttu-id="7e2ed-201">この接続に既に接続されている場合に、wifi 接続がより優先度の高いネットワークに接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-201">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="7e2ed-202">ConnectAutomatically 自動的に true になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-202">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="7e2ed-203">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="7e2ed-203">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="7e2ed-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e2ed-204">Boolean</span></span>|<span data-ttu-id="7e2ed-205">SSID がブロードキャストされていない場合でも、wifi 接続が自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-205">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="7e2ed-206">proxySetting</span><span class="sxs-lookup"><span data-stu-id="7e2ed-206">proxySetting</span></span>|[<span data-ttu-id="7e2ed-207">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="7e2ed-207">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="7e2ed-208">Wi-fi 構成のプロキシ設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-208">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="7e2ed-209">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-209">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="7e2ed-210">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="7e2ed-210">proxyManualAddress</span></span>|<span data-ttu-id="7e2ed-211">String</span><span class="sxs-lookup"><span data-stu-id="7e2ed-211">String</span></span>|<span data-ttu-id="7e2ed-212">プロキシサーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-212">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="7e2ed-213">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="7e2ed-213">proxyManualPort</span></span>|<span data-ttu-id="7e2ed-214">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2ed-214">Int32</span></span>|<span data-ttu-id="7e2ed-215">プロキシサーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-215">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="7e2ed-216">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="7e2ed-216">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="7e2ed-217">String</span><span class="sxs-lookup"><span data-stu-id="7e2ed-217">String</span></span>|<span data-ttu-id="7e2ed-218">プロキシサーバー構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-218">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="7e2ed-219">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="7e2ed-219">forceFIPSCompliance</span></span>|<span data-ttu-id="7e2ed-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e2ed-220">Boolean</span></span>|<span data-ttu-id="7e2ed-221">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-221">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="7e2ed-222">応答</span><span class="sxs-lookup"><span data-stu-id="7e2ed-222">Response</span></span>
<span data-ttu-id="7e2ed-223">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-223">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e2ed-224">例</span><span class="sxs-lookup"><span data-stu-id="7e2ed-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e2ed-225">要求</span><span class="sxs-lookup"><span data-stu-id="7e2ed-225">Request</span></span>
<span data-ttu-id="7e2ed-226">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="7e2ed-227">応答</span><span class="sxs-lookup"><span data-stu-id="7e2ed-227">Response</span></span>
<span data-ttu-id="7e2ed-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e2ed-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1731

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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





