---
title: IosWiFiConfiguration を作成する
description: 新しい iosWiFiConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ada1336be3243931bf88a91d44a522900fa2b8ef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338981"
---
# <a name="create-ioswificonfiguration"></a><span data-ttu-id="12998-103">IosWiFiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="12998-103">Create iosWiFiConfiguration</span></span>

> <span data-ttu-id="12998-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12998-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12998-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="12998-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12998-106">新しい[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="12998-106">Create a new [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12998-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="12998-107">Prerequisites</span></span>
<span data-ttu-id="12998-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12998-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12998-110">Permission type</span></span>|<span data-ttu-id="12998-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="12998-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12998-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12998-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12998-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12998-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12998-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12998-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12998-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12998-115">Not supported.</span></span>|
|<span data-ttu-id="12998-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12998-116">Application</span></span>|<span data-ttu-id="12998-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12998-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12998-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12998-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12998-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12998-119">Request headers</span></span>
|<span data-ttu-id="12998-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12998-120">Header</span></span>|<span data-ttu-id="12998-121">値</span><span class="sxs-lookup"><span data-stu-id="12998-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12998-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12998-122">Authorization</span></span>|<span data-ttu-id="12998-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="12998-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12998-124">承諾</span><span class="sxs-lookup"><span data-stu-id="12998-124">Accept</span></span>|<span data-ttu-id="12998-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12998-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12998-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="12998-126">Request body</span></span>
<span data-ttu-id="12998-127">要求本文で、iosWiFiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="12998-127">In the request body, supply a JSON representation for the iosWiFiConfiguration object.</span></span>

<span data-ttu-id="12998-128">次の表に、iosWiFiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="12998-128">The following table shows the properties that are required when you create the iosWiFiConfiguration.</span></span>

|<span data-ttu-id="12998-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12998-129">Property</span></span>|<span data-ttu-id="12998-130">型</span><span class="sxs-lookup"><span data-stu-id="12998-130">Type</span></span>|<span data-ttu-id="12998-131">説明</span><span class="sxs-lookup"><span data-stu-id="12998-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12998-132">id</span><span class="sxs-lookup"><span data-stu-id="12998-132">id</span></span>|<span data-ttu-id="12998-133">文字列</span><span class="sxs-lookup"><span data-stu-id="12998-133">String</span></span>|<span data-ttu-id="12998-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="12998-134">Key of the entity.</span></span> <span data-ttu-id="12998-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12998-136">lastModifiedDateTime</span></span>|<span data-ttu-id="12998-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12998-137">DateTimeOffset</span></span>|<span data-ttu-id="12998-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="12998-138">DateTime the object was last modified.</span></span> <span data-ttu-id="12998-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12998-140">roleScopeTagIds</span></span>|<span data-ttu-id="12998-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="12998-141">String collection</span></span>|<span data-ttu-id="12998-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="12998-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="12998-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="12998-144">supportsScopeTags</span></span>|<span data-ttu-id="12998-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="12998-145">Boolean</span></span>|<span data-ttu-id="12998-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="12998-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="12998-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="12998-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="12998-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="12998-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="12998-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="12998-149">This property is read-only.</span></span> <span data-ttu-id="12998-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12998-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="12998-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12998-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="12998-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="12998-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="12998-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12998-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="12998-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12998-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="12998-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="12998-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="12998-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="12998-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="12998-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="12998-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="12998-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="12998-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="12998-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12998-163">createdDateTime</span></span>|<span data-ttu-id="12998-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12998-164">DateTimeOffset</span></span>|<span data-ttu-id="12998-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="12998-165">DateTime the object was created.</span></span> <span data-ttu-id="12998-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-167">description</span><span class="sxs-lookup"><span data-stu-id="12998-167">description</span></span>|<span data-ttu-id="12998-168">String</span><span class="sxs-lookup"><span data-stu-id="12998-168">String</span></span>|<span data-ttu-id="12998-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="12998-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="12998-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-171">displayName</span><span class="sxs-lookup"><span data-stu-id="12998-171">displayName</span></span>|<span data-ttu-id="12998-172">String</span><span class="sxs-lookup"><span data-stu-id="12998-172">String</span></span>|<span data-ttu-id="12998-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="12998-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="12998-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-175">version</span><span class="sxs-lookup"><span data-stu-id="12998-175">version</span></span>|<span data-ttu-id="12998-176">Int32</span><span class="sxs-lookup"><span data-stu-id="12998-176">Int32</span></span>|<span data-ttu-id="12998-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="12998-177">Version of the device configuration.</span></span> <span data-ttu-id="12998-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="12998-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12998-179">networkName</span><span class="sxs-lookup"><span data-stu-id="12998-179">networkName</span></span>|<span data-ttu-id="12998-180">String</span><span class="sxs-lookup"><span data-stu-id="12998-180">String</span></span>|<span data-ttu-id="12998-181">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="12998-181">Network Name</span></span>|
|<span data-ttu-id="12998-182">ssid</span><span class="sxs-lookup"><span data-stu-id="12998-182">ssid</span></span>|<span data-ttu-id="12998-183">String</span><span class="sxs-lookup"><span data-stu-id="12998-183">String</span></span>|<span data-ttu-id="12998-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="12998-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="12998-185">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="12998-185">connectAutomatically</span></span>|<span data-ttu-id="12998-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="12998-186">Boolean</span></span>|<span data-ttu-id="12998-187">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="12998-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="12998-188">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="12998-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="12998-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="12998-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="12998-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="12998-190">Boolean</span></span>|<span data-ttu-id="12998-191">ネットワークが名前 (SSID) をブロードキャストしていない場合に接続します。</span><span class="sxs-lookup"><span data-stu-id="12998-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="12998-192">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="12998-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="12998-193">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="12998-193">wiFiSecurityType</span></span>|[<span data-ttu-id="12998-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="12998-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="12998-195">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="12998-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="12998-196">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="12998-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="12998-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="12998-197">proxySettings</span></span>|[<span data-ttu-id="12998-198">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="12998-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="12998-199">この Wi-fi 接続のプロキシの種類。</span><span class="sxs-lookup"><span data-stu-id="12998-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="12998-200">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="12998-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="12998-201">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="12998-201">proxyManualAddress</span></span>|<span data-ttu-id="12998-202">String</span><span class="sxs-lookup"><span data-stu-id="12998-202">String</span></span>|<span data-ttu-id="12998-203">手動構成が選択されている場合のプロキシサーバーの IP アドレスまたは DNS ホスト名。</span><span class="sxs-lookup"><span data-stu-id="12998-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="12998-204">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="12998-204">proxyManualPort</span></span>|<span data-ttu-id="12998-205">Int32</span><span class="sxs-lookup"><span data-stu-id="12998-205">Int32</span></span>|<span data-ttu-id="12998-206">手動構成が選択されている場合のプロキシサーバーのポート。</span><span class="sxs-lookup"><span data-stu-id="12998-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="12998-207">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="12998-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="12998-208">String</span><span class="sxs-lookup"><span data-stu-id="12998-208">String</span></span>|<span data-ttu-id="12998-209">自動構成が選択されている場合のプロキシサーバーの自動構成スクリプトの URL。</span><span class="sxs-lookup"><span data-stu-id="12998-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="12998-210">この URL は、通常、PAC (プロキシ自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="12998-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="12998-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="12998-211">preSharedKey</span></span>|<span data-ttu-id="12998-212">String</span><span class="sxs-lookup"><span data-stu-id="12998-212">String</span></span>|<span data-ttu-id="12998-213">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="12998-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="12998-214">応答</span><span class="sxs-lookup"><span data-stu-id="12998-214">Response</span></span>
<span data-ttu-id="12998-215">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12998-215">If successful, this method returns a `201 Created` response code and a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12998-216">例</span><span class="sxs-lookup"><span data-stu-id="12998-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="12998-217">要求</span><span class="sxs-lookup"><span data-stu-id="12998-217">Request</span></span>
<span data-ttu-id="12998-218">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12998-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1448

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="12998-219">応答</span><span class="sxs-lookup"><span data-stu-id="12998-219">Response</span></span>
<span data-ttu-id="12998-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12998-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1620

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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






