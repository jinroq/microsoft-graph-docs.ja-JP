---
title: AndroidWiFiConfiguration を作成する
description: 新しい androidWiFiConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebed9652afea7371bfe6133b0841af1bc1dc533c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340927"
---
# <a name="create-androidwificonfiguration"></a><span data-ttu-id="3f8dd-103">AndroidWiFiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="3f8dd-103">Create androidWiFiConfiguration</span></span>

> <span data-ttu-id="3f8dd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f8dd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f8dd-106">新しい[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-106">Create a new [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f8dd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3f8dd-107">Prerequisites</span></span>
<span data-ttu-id="3f8dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f8dd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f8dd-110">Permission type</span></span>|<span data-ttu-id="3f8dd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f8dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f8dd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f8dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f8dd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f8dd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f8dd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f8dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f8dd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-115">Not supported.</span></span>|
|<span data-ttu-id="3f8dd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f8dd-116">Application</span></span>|<span data-ttu-id="3f8dd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f8dd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f8dd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f8dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f8dd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f8dd-119">Request headers</span></span>
|<span data-ttu-id="3f8dd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f8dd-120">Header</span></span>|<span data-ttu-id="3f8dd-121">値</span><span class="sxs-lookup"><span data-stu-id="3f8dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f8dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f8dd-122">Authorization</span></span>|<span data-ttu-id="3f8dd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f8dd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3f8dd-124">Accept</span></span>|<span data-ttu-id="3f8dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f8dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f8dd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f8dd-126">Request body</span></span>
<span data-ttu-id="3f8dd-127">要求本文で、androidWiFiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-127">In the request body, supply a JSON representation for the androidWiFiConfiguration object.</span></span>

<span data-ttu-id="3f8dd-128">次の表に、androidWiFiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-128">The following table shows the properties that are required when you create the androidWiFiConfiguration.</span></span>

|<span data-ttu-id="3f8dd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f8dd-129">Property</span></span>|<span data-ttu-id="3f8dd-130">型</span><span class="sxs-lookup"><span data-stu-id="3f8dd-130">Type</span></span>|<span data-ttu-id="3f8dd-131">説明</span><span class="sxs-lookup"><span data-stu-id="3f8dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f8dd-132">id</span><span class="sxs-lookup"><span data-stu-id="3f8dd-132">id</span></span>|<span data-ttu-id="3f8dd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3f8dd-133">String</span></span>|<span data-ttu-id="3f8dd-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-134">Key of the entity.</span></span> <span data-ttu-id="3f8dd-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f8dd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3f8dd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f8dd-137">DateTimeOffset</span></span>|<span data-ttu-id="3f8dd-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3f8dd-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f8dd-140">roleScopeTagIds</span></span>|<span data-ttu-id="3f8dd-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3f8dd-141">String collection</span></span>|<span data-ttu-id="3f8dd-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3f8dd-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3f8dd-144">supportsScopeTags</span></span>|<span data-ttu-id="3f8dd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f8dd-145">Boolean</span></span>|<span data-ttu-id="3f8dd-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3f8dd-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3f8dd-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3f8dd-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-149">This property is read-only.</span></span> <span data-ttu-id="3f8dd-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f8dd-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3f8dd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f8dd-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3f8dd-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3f8dd-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f8dd-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3f8dd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f8dd-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3f8dd-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3f8dd-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="3f8dd-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3f8dd-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="3f8dd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3f8dd-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3f8dd-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f8dd-163">createdDateTime</span></span>|<span data-ttu-id="3f8dd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f8dd-164">DateTimeOffset</span></span>|<span data-ttu-id="3f8dd-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-165">DateTime the object was created.</span></span> <span data-ttu-id="3f8dd-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-167">description</span><span class="sxs-lookup"><span data-stu-id="3f8dd-167">description</span></span>|<span data-ttu-id="3f8dd-168">String</span><span class="sxs-lookup"><span data-stu-id="3f8dd-168">String</span></span>|<span data-ttu-id="3f8dd-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f8dd-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-171">displayName</span><span class="sxs-lookup"><span data-stu-id="3f8dd-171">displayName</span></span>|<span data-ttu-id="3f8dd-172">String</span><span class="sxs-lookup"><span data-stu-id="3f8dd-172">String</span></span>|<span data-ttu-id="3f8dd-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f8dd-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-175">version</span><span class="sxs-lookup"><span data-stu-id="3f8dd-175">version</span></span>|<span data-ttu-id="3f8dd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3f8dd-176">Int32</span></span>|<span data-ttu-id="3f8dd-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-177">Version of the device configuration.</span></span> <span data-ttu-id="3f8dd-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f8dd-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f8dd-179">networkName</span><span class="sxs-lookup"><span data-stu-id="3f8dd-179">networkName</span></span>|<span data-ttu-id="3f8dd-180">String</span><span class="sxs-lookup"><span data-stu-id="3f8dd-180">String</span></span>|<span data-ttu-id="3f8dd-181">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="3f8dd-181">Network Name</span></span>|
|<span data-ttu-id="3f8dd-182">ssid</span><span class="sxs-lookup"><span data-stu-id="3f8dd-182">ssid</span></span>|<span data-ttu-id="3f8dd-183">String</span><span class="sxs-lookup"><span data-stu-id="3f8dd-183">String</span></span>|<span data-ttu-id="3f8dd-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="3f8dd-185">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="3f8dd-185">connectAutomatically</span></span>|<span data-ttu-id="3f8dd-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f8dd-186">Boolean</span></span>|<span data-ttu-id="3f8dd-187">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="3f8dd-188">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="3f8dd-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="3f8dd-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3f8dd-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f8dd-190">Boolean</span></span>|<span data-ttu-id="3f8dd-191">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="3f8dd-192">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3f8dd-192">wiFiSecurityType</span></span>|[<span data-ttu-id="3f8dd-193">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3f8dd-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="3f8dd-194">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="3f8dd-195">可能な値は、`open`、`wpaEnterprise`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="3f8dd-196">応答</span><span class="sxs-lookup"><span data-stu-id="3f8dd-196">Response</span></span>
<span data-ttu-id="3f8dd-197">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-197">If successful, this method returns a `201 Created` response code and a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f8dd-198">例</span><span class="sxs-lookup"><span data-stu-id="3f8dd-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f8dd-199">要求</span><span class="sxs-lookup"><span data-stu-id="3f8dd-199">Request</span></span>
<span data-ttu-id="3f8dd-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1208

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="3f8dd-201">応答</span><span class="sxs-lookup"><span data-stu-id="3f8dd-201">Response</span></span>
<span data-ttu-id="3f8dd-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f8dd-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1380

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
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






