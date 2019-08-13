---
title: WindowsHealthMonitoringConfiguration を作成する
description: 新しい windowsHealthMonitoringConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94f384a638f4cf1ad01018d559c05827de7c0cd2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344540"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="634ba-103">WindowsHealthMonitoringConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="634ba-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="634ba-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="634ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="634ba-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="634ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="634ba-106">新しい[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="634ba-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="634ba-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="634ba-107">Prerequisites</span></span>
<span data-ttu-id="634ba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="634ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="634ba-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="634ba-110">Permission type</span></span>|<span data-ttu-id="634ba-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="634ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="634ba-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="634ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="634ba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="634ba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="634ba-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="634ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="634ba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="634ba-115">Not supported.</span></span>|
|<span data-ttu-id="634ba-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="634ba-116">Application</span></span>|<span data-ttu-id="634ba-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="634ba-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="634ba-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="634ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="634ba-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="634ba-119">Request headers</span></span>
|<span data-ttu-id="634ba-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="634ba-120">Header</span></span>|<span data-ttu-id="634ba-121">値</span><span class="sxs-lookup"><span data-stu-id="634ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="634ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="634ba-122">Authorization</span></span>|<span data-ttu-id="634ba-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="634ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="634ba-124">承諾</span><span class="sxs-lookup"><span data-stu-id="634ba-124">Accept</span></span>|<span data-ttu-id="634ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="634ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="634ba-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="634ba-126">Request body</span></span>
<span data-ttu-id="634ba-127">要求本文で、windowsHealthMonitoringConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="634ba-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="634ba-128">次の表に、windowsHealthMonitoringConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="634ba-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="634ba-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="634ba-129">Property</span></span>|<span data-ttu-id="634ba-130">型</span><span class="sxs-lookup"><span data-stu-id="634ba-130">Type</span></span>|<span data-ttu-id="634ba-131">説明</span><span class="sxs-lookup"><span data-stu-id="634ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="634ba-132">id</span><span class="sxs-lookup"><span data-stu-id="634ba-132">id</span></span>|<span data-ttu-id="634ba-133">文字列</span><span class="sxs-lookup"><span data-stu-id="634ba-133">String</span></span>|<span data-ttu-id="634ba-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="634ba-134">Key of the entity.</span></span> <span data-ttu-id="634ba-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="634ba-136">lastModifiedDateTime</span></span>|<span data-ttu-id="634ba-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="634ba-137">DateTimeOffset</span></span>|<span data-ttu-id="634ba-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="634ba-138">DateTime the object was last modified.</span></span> <span data-ttu-id="634ba-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="634ba-140">roleScopeTagIds</span></span>|<span data-ttu-id="634ba-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="634ba-141">String collection</span></span>|<span data-ttu-id="634ba-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="634ba-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="634ba-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="634ba-144">supportsScopeTags</span></span>|<span data-ttu-id="634ba-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="634ba-145">Boolean</span></span>|<span data-ttu-id="634ba-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="634ba-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="634ba-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="634ba-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="634ba-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="634ba-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="634ba-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="634ba-149">This property is read-only.</span></span> <span data-ttu-id="634ba-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="634ba-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="634ba-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="634ba-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="634ba-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="634ba-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="634ba-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="634ba-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="634ba-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="634ba-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="634ba-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="634ba-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="634ba-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="634ba-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="634ba-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="634ba-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="634ba-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="634ba-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="634ba-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="634ba-163">createdDateTime</span></span>|<span data-ttu-id="634ba-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="634ba-164">DateTimeOffset</span></span>|<span data-ttu-id="634ba-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="634ba-165">DateTime the object was created.</span></span> <span data-ttu-id="634ba-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-167">description</span><span class="sxs-lookup"><span data-stu-id="634ba-167">description</span></span>|<span data-ttu-id="634ba-168">String</span><span class="sxs-lookup"><span data-stu-id="634ba-168">String</span></span>|<span data-ttu-id="634ba-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="634ba-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="634ba-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-171">displayName</span><span class="sxs-lookup"><span data-stu-id="634ba-171">displayName</span></span>|<span data-ttu-id="634ba-172">String</span><span class="sxs-lookup"><span data-stu-id="634ba-172">String</span></span>|<span data-ttu-id="634ba-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="634ba-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="634ba-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-175">version</span><span class="sxs-lookup"><span data-stu-id="634ba-175">version</span></span>|<span data-ttu-id="634ba-176">Int32</span><span class="sxs-lookup"><span data-stu-id="634ba-176">Int32</span></span>|<span data-ttu-id="634ba-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="634ba-177">Version of the device configuration.</span></span> <span data-ttu-id="634ba-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="634ba-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="634ba-179">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="634ba-179">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="634ba-180">購入</span><span class="sxs-lookup"><span data-stu-id="634ba-180">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="634ba-181">デバイス上でのデバイスの正常性の監視を有効にします。</span><span class="sxs-lookup"><span data-stu-id="634ba-181">Enables device health monitoring on the device.</span></span> <span data-ttu-id="634ba-182">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="634ba-182">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="634ba-183">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="634ba-183">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="634ba-184">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="634ba-184">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="634ba-185">正常性の監視が有効になっているデバイスから収集されたイベントのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="634ba-185">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="634ba-186">可能な値は、`undefined`、`healthMonitoring`、`bootPerformance` です。</span><span class="sxs-lookup"><span data-stu-id="634ba-186">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|
|<span data-ttu-id="634ba-187">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="634ba-187">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="634ba-188">String</span><span class="sxs-lookup"><span data-stu-id="634ba-188">String</span></span>|<span data-ttu-id="634ba-189">正常性監視が有効になっているデバイスから収集されたイベントのカスタムセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="634ba-189">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="634ba-190">応答</span><span class="sxs-lookup"><span data-stu-id="634ba-190">Response</span></span>
<span data-ttu-id="634ba-191">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="634ba-191">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="634ba-192">例</span><span class="sxs-lookup"><span data-stu-id="634ba-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="634ba-193">要求</span><span class="sxs-lookup"><span data-stu-id="634ba-193">Request</span></span>
<span data-ttu-id="634ba-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="634ba-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1244

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
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
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```

### <a name="response"></a><span data-ttu-id="634ba-195">応答</span><span class="sxs-lookup"><span data-stu-id="634ba-195">Response</span></span>
<span data-ttu-id="634ba-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="634ba-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1416

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
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
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```






