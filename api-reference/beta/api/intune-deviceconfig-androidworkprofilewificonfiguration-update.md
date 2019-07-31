---
title: AndroidWorkProfileWiFiConfiguration の更新
description: AndroidWorkProfileWiFiConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5ce1b0f71d5f16a378ffe096deb18810d8e097d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950281"
---
# <a name="update-androidworkprofilewificonfiguration"></a><span data-ttu-id="9ef77-103">AndroidWorkProfileWiFiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="9ef77-103">Update androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="9ef77-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ef77-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ef77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ef77-106">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-106">Update the properties of a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ef77-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9ef77-107">Prerequisites</span></span>
<span data-ttu-id="9ef77-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ef77-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ef77-110">Permission type</span></span>|<span data-ttu-id="9ef77-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ef77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ef77-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ef77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ef77-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef77-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ef77-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ef77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ef77-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef77-115">Not supported.</span></span>|
|<span data-ttu-id="9ef77-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ef77-116">Application</span></span>|<span data-ttu-id="9ef77-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef77-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ef77-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ef77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ef77-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ef77-119">Request headers</span></span>
|<span data-ttu-id="9ef77-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ef77-120">Header</span></span>|<span data-ttu-id="9ef77-121">値</span><span class="sxs-lookup"><span data-stu-id="9ef77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ef77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ef77-122">Authorization</span></span>|<span data-ttu-id="9ef77-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ef77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ef77-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9ef77-124">Accept</span></span>|<span data-ttu-id="9ef77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ef77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ef77-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ef77-126">Request body</span></span>
<span data-ttu-id="9ef77-127">要求本文で、 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-127">In the request body, supply a JSON representation for the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

<span data-ttu-id="9ef77-128">次の表に、 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-128">The following table shows the properties that are required when you create the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span>

|<span data-ttu-id="9ef77-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ef77-129">Property</span></span>|<span data-ttu-id="9ef77-130">型</span><span class="sxs-lookup"><span data-stu-id="9ef77-130">Type</span></span>|<span data-ttu-id="9ef77-131">説明</span><span class="sxs-lookup"><span data-stu-id="9ef77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef77-132">id</span><span class="sxs-lookup"><span data-stu-id="9ef77-132">id</span></span>|<span data-ttu-id="9ef77-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9ef77-133">String</span></span>|<span data-ttu-id="9ef77-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9ef77-134">Key of the entity.</span></span> <span data-ttu-id="9ef77-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ef77-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9ef77-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ef77-137">DateTimeOffset</span></span>|<span data-ttu-id="9ef77-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="9ef77-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9ef77-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ef77-140">roleScopeTagIds</span></span>|<span data-ttu-id="9ef77-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9ef77-141">String collection</span></span>|<span data-ttu-id="9ef77-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9ef77-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ef77-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ef77-144">supportsScopeTags</span></span>|<span data-ttu-id="9ef77-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ef77-145">Boolean</span></span>|<span data-ttu-id="9ef77-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ef77-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9ef77-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ef77-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9ef77-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ef77-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-149">This property is read-only.</span></span> <span data-ttu-id="9ef77-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ef77-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9ef77-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ef77-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9ef77-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="9ef77-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9ef77-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ef77-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9ef77-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ef77-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9ef77-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="9ef77-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9ef77-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="9ef77-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9ef77-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="9ef77-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9ef77-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="9ef77-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9ef77-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ef77-163">createdDateTime</span></span>|<span data-ttu-id="9ef77-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ef77-164">DateTimeOffset</span></span>|<span data-ttu-id="9ef77-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9ef77-165">DateTime the object was created.</span></span> <span data-ttu-id="9ef77-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-167">description</span><span class="sxs-lookup"><span data-stu-id="9ef77-167">description</span></span>|<span data-ttu-id="9ef77-168">String</span><span class="sxs-lookup"><span data-stu-id="9ef77-168">String</span></span>|<span data-ttu-id="9ef77-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="9ef77-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ef77-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9ef77-171">displayName</span></span>|<span data-ttu-id="9ef77-172">String</span><span class="sxs-lookup"><span data-stu-id="9ef77-172">String</span></span>|<span data-ttu-id="9ef77-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="9ef77-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ef77-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-175">version</span><span class="sxs-lookup"><span data-stu-id="9ef77-175">version</span></span>|<span data-ttu-id="9ef77-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9ef77-176">Int32</span></span>|<span data-ttu-id="9ef77-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9ef77-177">Version of the device configuration.</span></span> <span data-ttu-id="9ef77-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ef77-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ef77-179">networkName</span><span class="sxs-lookup"><span data-stu-id="9ef77-179">networkName</span></span>|<span data-ttu-id="9ef77-180">String</span><span class="sxs-lookup"><span data-stu-id="9ef77-180">String</span></span>|<span data-ttu-id="9ef77-181">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="9ef77-181">Network Name</span></span>|
|<span data-ttu-id="9ef77-182">ssid</span><span class="sxs-lookup"><span data-stu-id="9ef77-182">ssid</span></span>|<span data-ttu-id="9ef77-183">String</span><span class="sxs-lookup"><span data-stu-id="9ef77-183">String</span></span>|<span data-ttu-id="9ef77-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="9ef77-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="9ef77-185">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="9ef77-185">connectAutomatically</span></span>|<span data-ttu-id="9ef77-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ef77-186">Boolean</span></span>|<span data-ttu-id="9ef77-187">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="9ef77-188">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="9ef77-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="9ef77-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9ef77-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9ef77-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ef77-190">Boolean</span></span>|<span data-ttu-id="9ef77-191">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="9ef77-192">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9ef77-192">wiFiSecurityType</span></span>|[<span data-ttu-id="9ef77-193">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9ef77-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="9ef77-194">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="9ef77-195">可能な値は、`open`、`wpaEnterprise`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="9ef77-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="9ef77-196">応答</span><span class="sxs-lookup"><span data-stu-id="9ef77-196">Response</span></span>
<span data-ttu-id="9ef77-197">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ef77-197">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ef77-198">例</span><span class="sxs-lookup"><span data-stu-id="9ef77-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ef77-199">要求</span><span class="sxs-lookup"><span data-stu-id="9ef77-199">Request</span></span>
<span data-ttu-id="9ef77-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ef77-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1219

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="9ef77-201">応答</span><span class="sxs-lookup"><span data-stu-id="9ef77-201">Response</span></span>
<span data-ttu-id="9ef77-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ef77-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1391

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
  "id": "8400d131-d131-8400-31d1-008431d10084",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```





