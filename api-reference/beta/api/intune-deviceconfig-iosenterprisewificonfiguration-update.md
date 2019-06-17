---
title: IosEnterpriseWiFiConfiguration の更新
description: IosEnterpriseWiFiConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e48a9dafd287594d56236cb93809a2137a6b285
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966734"
---
# <a name="update-iosenterprisewificonfiguration"></a><span data-ttu-id="cb75e-103">IosEnterpriseWiFiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="cb75e-103">Update iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="cb75e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb75e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb75e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb75e-106">[IosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-106">Update the properties of a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb75e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cb75e-107">Prerequisites</span></span>
<span data-ttu-id="cb75e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb75e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb75e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb75e-110">Permission type</span></span>|<span data-ttu-id="cb75e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb75e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb75e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb75e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb75e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb75e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb75e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb75e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb75e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb75e-115">Not supported.</span></span>|
|<span data-ttu-id="cb75e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb75e-116">Application</span></span>|<span data-ttu-id="cb75e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb75e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb75e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb75e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cb75e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb75e-119">Request headers</span></span>
|<span data-ttu-id="cb75e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb75e-120">Header</span></span>|<span data-ttu-id="cb75e-121">値</span><span class="sxs-lookup"><span data-stu-id="cb75e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb75e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb75e-122">Authorization</span></span>|<span data-ttu-id="cb75e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb75e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cb75e-124">Accept</span></span>|<span data-ttu-id="cb75e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb75e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb75e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb75e-126">Request body</span></span>
<span data-ttu-id="cb75e-127">要求本文で、 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-127">In the request body, supply a JSON representation for the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="cb75e-128">次の表に、 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-128">The following table shows the properties that are required when you create the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="cb75e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb75e-129">Property</span></span>|<span data-ttu-id="cb75e-130">型</span><span class="sxs-lookup"><span data-stu-id="cb75e-130">Type</span></span>|<span data-ttu-id="cb75e-131">説明</span><span class="sxs-lookup"><span data-stu-id="cb75e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb75e-132">id</span><span class="sxs-lookup"><span data-stu-id="cb75e-132">id</span></span>|<span data-ttu-id="cb75e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="cb75e-133">String</span></span>|<span data-ttu-id="cb75e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cb75e-134">Key of the entity.</span></span> <span data-ttu-id="cb75e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb75e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cb75e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb75e-137">DateTimeOffset</span></span>|<span data-ttu-id="cb75e-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="cb75e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cb75e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb75e-140">roleScopeTagIds</span></span>|<span data-ttu-id="cb75e-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="cb75e-141">String collection</span></span>|<span data-ttu-id="cb75e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="cb75e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cb75e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cb75e-144">supportsScopeTags</span></span>|<span data-ttu-id="cb75e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb75e-145">Boolean</span></span>|<span data-ttu-id="cb75e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cb75e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="cb75e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cb75e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="cb75e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cb75e-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-149">This property is read-only.</span></span> <span data-ttu-id="cb75e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cb75e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cb75e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cb75e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cb75e-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="cb75e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cb75e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cb75e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cb75e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cb75e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cb75e-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="cb75e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cb75e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="cb75e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cb75e-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="cb75e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cb75e-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="cb75e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cb75e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb75e-163">createdDateTime</span></span>|<span data-ttu-id="cb75e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb75e-164">DateTimeOffset</span></span>|<span data-ttu-id="cb75e-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cb75e-165">DateTime the object was created.</span></span> <span data-ttu-id="cb75e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-167">description</span><span class="sxs-lookup"><span data-stu-id="cb75e-167">description</span></span>|<span data-ttu-id="cb75e-168">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-168">String</span></span>|<span data-ttu-id="cb75e-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="cb75e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb75e-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="cb75e-171">displayName</span></span>|<span data-ttu-id="cb75e-172">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-172">String</span></span>|<span data-ttu-id="cb75e-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="cb75e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb75e-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-175">version</span><span class="sxs-lookup"><span data-stu-id="cb75e-175">version</span></span>|<span data-ttu-id="cb75e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="cb75e-176">Int32</span></span>|<span data-ttu-id="cb75e-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cb75e-177">Version of the device configuration.</span></span> <span data-ttu-id="cb75e-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb75e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-179">networkName</span><span class="sxs-lookup"><span data-stu-id="cb75e-179">networkName</span></span>|<span data-ttu-id="cb75e-180">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-180">String</span></span>|<span data-ttu-id="cb75e-181">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されたネットワーク名</span><span class="sxs-lookup"><span data-stu-id="cb75e-181">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-182">ssid</span><span class="sxs-lookup"><span data-stu-id="cb75e-182">ssid</span></span>|<span data-ttu-id="cb75e-183">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-183">String</span></span>|<span data-ttu-id="cb75e-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="cb75e-185">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-185">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-186">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="cb75e-186">connectAutomatically</span></span>|<span data-ttu-id="cb75e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb75e-187">Boolean</span></span>|<span data-ttu-id="cb75e-188">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="cb75e-189">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="cb75e-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="cb75e-190">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-190">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="cb75e-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="cb75e-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb75e-192">Boolean</span></span>|<span data-ttu-id="cb75e-193">ネットワークが名前 (SSID) をブロードキャストしていない場合に接続します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-193">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="cb75e-194">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="cb75e-195">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-195">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="cb75e-196">wiFiSecurityType</span></span>|[<span data-ttu-id="cb75e-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="cb75e-197">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="cb75e-198">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="cb75e-199">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="cb75e-199">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="cb75e-200">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="cb75e-200">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="cb75e-201">proxySettings</span><span class="sxs-lookup"><span data-stu-id="cb75e-201">proxySettings</span></span>|[<span data-ttu-id="cb75e-202">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="cb75e-202">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="cb75e-203">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されたこの wi-fi 接続のプロキシの種類。</span><span class="sxs-lookup"><span data-stu-id="cb75e-203">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="cb75e-204">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-204">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="cb75e-205">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="cb75e-205">proxyManualAddress</span></span>|<span data-ttu-id="cb75e-206">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-206">String</span></span>|<span data-ttu-id="cb75e-207">手動構成が選択されている場合のプロキシサーバーの IP アドレスまたは DNS ホスト名。</span><span class="sxs-lookup"><span data-stu-id="cb75e-207">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="cb75e-208">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-208">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-209">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="cb75e-209">proxyManualPort</span></span>|<span data-ttu-id="cb75e-210">Int32</span><span class="sxs-lookup"><span data-stu-id="cb75e-210">Int32</span></span>|<span data-ttu-id="cb75e-211">手動構成が選択されている場合のプロキシサーバーのポート。</span><span class="sxs-lookup"><span data-stu-id="cb75e-211">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="cb75e-212">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-212">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-213">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="cb75e-213">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="cb75e-214">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-214">String</span></span>|<span data-ttu-id="cb75e-215">自動構成が選択されている場合のプロキシサーバーの自動構成スクリプトの URL。</span><span class="sxs-lookup"><span data-stu-id="cb75e-215">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="cb75e-216">この URL は、通常、PAC (プロキシ自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-216">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="cb75e-217">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-217">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-218">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="cb75e-218">preSharedKey</span></span>|<span data-ttu-id="cb75e-219">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-219">String</span></span>|<span data-ttu-id="cb75e-220">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="cb75e-220">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="cb75e-221">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-221">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="cb75e-222">eapType</span><span class="sxs-lookup"><span data-stu-id="cb75e-222">eapType</span></span>|[<span data-ttu-id="cb75e-223">eapType</span><span class="sxs-lookup"><span data-stu-id="cb75e-223">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="cb75e-224">拡張認証プロトコル (EAP)。</span><span class="sxs-lookup"><span data-stu-id="cb75e-224">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="cb75e-225">Wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-225">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="cb75e-226">使用可能な値: `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="cb75e-226">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="cb75e-227">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb75e-227">eapFastConfiguration</span></span>|[<span data-ttu-id="cb75e-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb75e-228">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="cb75e-229">Eap-fast が選択した EAP の種類の場合、eap-fast 構成オプション。</span><span class="sxs-lookup"><span data-stu-id="cb75e-229">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="cb75e-230">使用可能な値は、`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously` です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-230">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="cb75e-231">Trustedserverの形式</span><span class="sxs-lookup"><span data-stu-id="cb75e-231">trustedServerCertificateNames</span></span>|<span data-ttu-id="cb75e-232">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="cb75e-232">String collection</span></span>|<span data-ttu-id="cb75e-233">Eap の種類が eap-tls/TTLS/ファストまたは PEAP に構成されている場合の、信頼されたサーバー証明書の名前。</span><span class="sxs-lookup"><span data-stu-id="cb75e-233">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="cb75e-234">これは、信頼できる証明機関 (CA) によって発行された証明書で使用される一般的な名前です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-234">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="cb75e-235">この情報を指定すると、エンドユーザーがこの Wi-fi ネットワークに接続したときに、エンドユーザーのデバイスに表示される [動的信頼] ダイアログをバイパスすることができます。</span><span class="sxs-lookup"><span data-stu-id="cb75e-235">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="cb75e-236">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb75e-236">authenticationMethod</span></span>|[<span data-ttu-id="cb75e-237">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb75e-237">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="cb75e-238">EAP の種類が PEAP または EAP-TLS に構成されている場合の認証方法。</span><span class="sxs-lookup"><span data-stu-id="cb75e-238">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="cb75e-239">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-239">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="cb75e-240">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="cb75e-240">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="cb75e-241">None Apauthenticationmethod_ Apttlstype</span><span class="sxs-lookup"><span data-stu-id="cb75e-241">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="cb75e-242">Eap の種類が EAP-TLS で、Authenticationmethod がユーザー名とパスワードの場合に認証を行うための非 EAP メソッド。</span><span class="sxs-lookup"><span data-stu-id="cb75e-242">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="cb75e-243">使用可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-243">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="cb75e-244">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="cb75e-244">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="cb75e-245">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-245">String</span></span>|<span data-ttu-id="cb75e-246">Eap の種類が EAP-TLS、eap-fast、または PEAP に構成されている場合は、id プライバシー (外部 Id) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="cb75e-246">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="cb75e-247">このプロパティは、入力したテキストでユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="cb75e-247">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="cb75e-248">たとえば、' anonymous ' を使用すると、この Wi-fi 接続で実際のユーザー名を使用して認証する各ユーザーは、' anonymous ' と表示されます。</span><span class="sxs-lookup"><span data-stu-id="cb75e-248">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="cb75e-249">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="cb75e-249">usernameFormatString</span></span>|<span data-ttu-id="cb75e-250">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-250">String</span></span>|<span data-ttu-id="cb75e-251">Wifi に接続するためのユーザー名を作成するために使用されるユーザー名の形式文字列</span><span class="sxs-lookup"><span data-stu-id="cb75e-251">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="cb75e-252">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="cb75e-252">passwordFormatString</span></span>|<span data-ttu-id="cb75e-253">String</span><span class="sxs-lookup"><span data-stu-id="cb75e-253">String</span></span>|<span data-ttu-id="cb75e-254">Wifi に接続するためのパスワードを作成するために使用されるパスワード形式の文字列</span><span class="sxs-lookup"><span data-stu-id="cb75e-254">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="cb75e-255">応答</span><span class="sxs-lookup"><span data-stu-id="cb75e-255">Response</span></span>
<span data-ttu-id="cb75e-256">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb75e-256">If successful, this method returns a `200 OK` response code and an updated [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb75e-257">例</span><span class="sxs-lookup"><span data-stu-id="cb75e-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb75e-258">要求</span><span class="sxs-lookup"><span data-stu-id="cb75e-258">Request</span></span>
<span data-ttu-id="cb75e-259">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cb75e-259">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1974

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```

### <a name="response"></a><span data-ttu-id="cb75e-260">応答</span><span class="sxs-lookup"><span data-stu-id="cb75e-260">Response</span></span>
<span data-ttu-id="cb75e-p128">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb75e-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2146

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```





