---
title: MacOSWiFiConfiguration の更新
description: MacOSWiFiConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acd3bfceb4dd41ba815ae52868ac48108abda7ca
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963031"
---
# <a name="update-macoswificonfiguration"></a><span data-ttu-id="d98c9-103">MacOSWiFiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d98c9-103">Update macOSWiFiConfiguration</span></span>

> <span data-ttu-id="d98c9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d98c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d98c9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d98c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d98c9-106">[MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-106">Update the properties of a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d98c9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d98c9-107">Prerequisites</span></span>
<span data-ttu-id="d98c9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d98c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d98c9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d98c9-110">Permission type</span></span>|<span data-ttu-id="d98c9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d98c9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d98c9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d98c9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d98c9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98c9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d98c9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d98c9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d98c9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d98c9-115">Not supported.</span></span>|
|<span data-ttu-id="d98c9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d98c9-116">Application</span></span>|<span data-ttu-id="d98c9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d98c9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d98c9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d98c9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d98c9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d98c9-119">Request headers</span></span>
|<span data-ttu-id="d98c9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d98c9-120">Header</span></span>|<span data-ttu-id="d98c9-121">値</span><span class="sxs-lookup"><span data-stu-id="d98c9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d98c9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d98c9-122">Authorization</span></span>|<span data-ttu-id="d98c9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d98c9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d98c9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d98c9-124">Accept</span></span>|<span data-ttu-id="d98c9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d98c9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d98c9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d98c9-126">Request body</span></span>
<span data-ttu-id="d98c9-127">要求本文で、 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-127">In the request body, supply a JSON representation for the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

<span data-ttu-id="d98c9-128">次の表に、 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-128">The following table shows the properties that are required when you create the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>

|<span data-ttu-id="d98c9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d98c9-129">Property</span></span>|<span data-ttu-id="d98c9-130">型</span><span class="sxs-lookup"><span data-stu-id="d98c9-130">Type</span></span>|<span data-ttu-id="d98c9-131">説明</span><span class="sxs-lookup"><span data-stu-id="d98c9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98c9-132">id</span><span class="sxs-lookup"><span data-stu-id="d98c9-132">id</span></span>|<span data-ttu-id="d98c9-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d98c9-133">String</span></span>|<span data-ttu-id="d98c9-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d98c9-134">Key of the entity.</span></span> <span data-ttu-id="d98c9-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d98c9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d98c9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d98c9-137">DateTimeOffset</span></span>|<span data-ttu-id="d98c9-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d98c9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d98c9-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d98c9-140">roleScopeTagIds</span></span>|<span data-ttu-id="d98c9-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d98c9-141">String collection</span></span>|<span data-ttu-id="d98c9-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="d98c9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d98c9-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d98c9-144">supportsScopeTags</span></span>|<span data-ttu-id="d98c9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98c9-145">Boolean</span></span>|<span data-ttu-id="d98c9-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d98c9-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="d98c9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d98c9-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="d98c9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d98c9-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-149">This property is read-only.</span></span> <span data-ttu-id="d98c9-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d98c9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d98c9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d98c9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d98c9-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="d98c9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d98c9-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d98c9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d98c9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d98c9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d98c9-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d98c9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d98c9-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d98c9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d98c9-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d98c9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d98c9-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d98c9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d98c9-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d98c9-163">createdDateTime</span></span>|<span data-ttu-id="d98c9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d98c9-164">DateTimeOffset</span></span>|<span data-ttu-id="d98c9-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d98c9-165">DateTime the object was created.</span></span> <span data-ttu-id="d98c9-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-167">description</span><span class="sxs-lookup"><span data-stu-id="d98c9-167">description</span></span>|<span data-ttu-id="d98c9-168">String</span><span class="sxs-lookup"><span data-stu-id="d98c9-168">String</span></span>|<span data-ttu-id="d98c9-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="d98c9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d98c9-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d98c9-171">displayName</span></span>|<span data-ttu-id="d98c9-172">String</span><span class="sxs-lookup"><span data-stu-id="d98c9-172">String</span></span>|<span data-ttu-id="d98c9-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d98c9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d98c9-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-175">version</span><span class="sxs-lookup"><span data-stu-id="d98c9-175">version</span></span>|<span data-ttu-id="d98c9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d98c9-176">Int32</span></span>|<span data-ttu-id="d98c9-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d98c9-177">Version of the device configuration.</span></span> <span data-ttu-id="d98c9-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d98c9-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d98c9-179">networkName</span><span class="sxs-lookup"><span data-stu-id="d98c9-179">networkName</span></span>|<span data-ttu-id="d98c9-180">String</span><span class="sxs-lookup"><span data-stu-id="d98c9-180">String</span></span>|<span data-ttu-id="d98c9-181">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="d98c9-181">Network Name</span></span>|
|<span data-ttu-id="d98c9-182">ssid</span><span class="sxs-lookup"><span data-stu-id="d98c9-182">ssid</span></span>|<span data-ttu-id="d98c9-183">String</span><span class="sxs-lookup"><span data-stu-id="d98c9-183">String</span></span>|<span data-ttu-id="d98c9-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="d98c9-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="d98c9-185">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="d98c9-185">connectAutomatically</span></span>|<span data-ttu-id="d98c9-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98c9-186">Boolean</span></span>|<span data-ttu-id="d98c9-187">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="d98c9-188">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="d98c9-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="d98c9-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="d98c9-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="d98c9-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98c9-190">Boolean</span></span>|<span data-ttu-id="d98c9-191">ネットワークが名前 (SSID) をブロードキャストしていない場合に接続します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="d98c9-192">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="d98c9-193">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d98c9-193">wiFiSecurityType</span></span>|[<span data-ttu-id="d98c9-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d98c9-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="d98c9-195">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="d98c9-196">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="d98c9-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="d98c9-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="d98c9-197">proxySettings</span></span>|[<span data-ttu-id="d98c9-198">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="d98c9-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="d98c9-199">この Wi-fi 接続のプロキシの種類。</span><span class="sxs-lookup"><span data-stu-id="d98c9-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="d98c9-200">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="d98c9-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="d98c9-201">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="d98c9-201">proxyManualAddress</span></span>|<span data-ttu-id="d98c9-202">String</span><span class="sxs-lookup"><span data-stu-id="d98c9-202">String</span></span>|<span data-ttu-id="d98c9-203">手動構成が選択されている場合のプロキシサーバーの IP アドレスまたは DNS ホスト名。</span><span class="sxs-lookup"><span data-stu-id="d98c9-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="d98c9-204">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="d98c9-204">proxyManualPort</span></span>|<span data-ttu-id="d98c9-205">Int32</span><span class="sxs-lookup"><span data-stu-id="d98c9-205">Int32</span></span>|<span data-ttu-id="d98c9-206">手動構成が選択されている場合のプロキシサーバーのポート。</span><span class="sxs-lookup"><span data-stu-id="d98c9-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="d98c9-207">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="d98c9-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="d98c9-208">String</span><span class="sxs-lookup"><span data-stu-id="d98c9-208">String</span></span>|<span data-ttu-id="d98c9-209">自動構成が選択されている場合のプロキシサーバーの自動構成スクリプトの URL。</span><span class="sxs-lookup"><span data-stu-id="d98c9-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="d98c9-210">この URL は、通常、PAC (プロキシ自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="d98c9-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="d98c9-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="d98c9-211">preSharedKey</span></span>|<span data-ttu-id="d98c9-212">String</span><span class="sxs-lookup"><span data-stu-id="d98c9-212">String</span></span>|<span data-ttu-id="d98c9-213">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="d98c9-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="d98c9-214">応答</span><span class="sxs-lookup"><span data-stu-id="d98c9-214">Response</span></span>
<span data-ttu-id="d98c9-215">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d98c9-215">If successful, this method returns a `200 OK` response code and an updated [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d98c9-216">例</span><span class="sxs-lookup"><span data-stu-id="d98c9-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="d98c9-217">要求</span><span class="sxs-lookup"><span data-stu-id="d98c9-217">Request</span></span>
<span data-ttu-id="d98c9-218">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d98c9-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1450

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="d98c9-219">応答</span><span class="sxs-lookup"><span data-stu-id="d98c9-219">Response</span></span>
<span data-ttu-id="d98c9-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d98c9-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1622

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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





