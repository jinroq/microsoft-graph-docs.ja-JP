---
title: WindowsHealthMonitoringConfiguration を作成する
description: 新しい windowsHealthMonitoringConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fece8f0095067393da3d13b773291b89daa2325d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982173"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="26a53-103">WindowsHealthMonitoringConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="26a53-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="26a53-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26a53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26a53-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="26a53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a53-106">新しい[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="26a53-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26a53-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="26a53-107">Prerequisites</span></span>
<span data-ttu-id="26a53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26a53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a53-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26a53-110">Permission type</span></span>|<span data-ttu-id="26a53-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="26a53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26a53-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26a53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26a53-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a53-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26a53-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26a53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26a53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26a53-115">Not supported.</span></span>|
|<span data-ttu-id="26a53-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26a53-116">Application</span></span>|<span data-ttu-id="26a53-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26a53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26a53-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26a53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="26a53-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26a53-119">Request headers</span></span>
|<span data-ttu-id="26a53-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26a53-120">Header</span></span>|<span data-ttu-id="26a53-121">値</span><span class="sxs-lookup"><span data-stu-id="26a53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26a53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26a53-122">Authorization</span></span>|<span data-ttu-id="26a53-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="26a53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26a53-124">承諾</span><span class="sxs-lookup"><span data-stu-id="26a53-124">Accept</span></span>|<span data-ttu-id="26a53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26a53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26a53-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="26a53-126">Request body</span></span>
<span data-ttu-id="26a53-127">要求本文で、windowsHealthMonitoringConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="26a53-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="26a53-128">次の表に、windowsHealthMonitoringConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="26a53-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="26a53-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26a53-129">Property</span></span>|<span data-ttu-id="26a53-130">型</span><span class="sxs-lookup"><span data-stu-id="26a53-130">Type</span></span>|<span data-ttu-id="26a53-131">説明</span><span class="sxs-lookup"><span data-stu-id="26a53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a53-132">id</span><span class="sxs-lookup"><span data-stu-id="26a53-132">id</span></span>|<span data-ttu-id="26a53-133">文字列</span><span class="sxs-lookup"><span data-stu-id="26a53-133">String</span></span>|<span data-ttu-id="26a53-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="26a53-134">Key of the entity.</span></span> <span data-ttu-id="26a53-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26a53-136">lastModifiedDateTime</span></span>|<span data-ttu-id="26a53-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a53-137">DateTimeOffset</span></span>|<span data-ttu-id="26a53-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="26a53-138">DateTime the object was last modified.</span></span> <span data-ttu-id="26a53-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26a53-140">roleScopeTagIds</span></span>|<span data-ttu-id="26a53-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="26a53-141">String collection</span></span>|<span data-ttu-id="26a53-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="26a53-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26a53-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="26a53-144">supportsScopeTags</span></span>|<span data-ttu-id="26a53-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a53-145">Boolean</span></span>|<span data-ttu-id="26a53-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="26a53-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="26a53-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="26a53-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="26a53-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="26a53-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="26a53-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="26a53-149">This property is read-only.</span></span> <span data-ttu-id="26a53-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26a53-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="26a53-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26a53-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="26a53-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="26a53-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="26a53-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26a53-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="26a53-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26a53-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="26a53-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="26a53-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="26a53-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="26a53-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="26a53-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="26a53-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="26a53-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="26a53-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="26a53-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26a53-163">createdDateTime</span></span>|<span data-ttu-id="26a53-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a53-164">DateTimeOffset</span></span>|<span data-ttu-id="26a53-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="26a53-165">DateTime the object was created.</span></span> <span data-ttu-id="26a53-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-167">description</span><span class="sxs-lookup"><span data-stu-id="26a53-167">description</span></span>|<span data-ttu-id="26a53-168">String</span><span class="sxs-lookup"><span data-stu-id="26a53-168">String</span></span>|<span data-ttu-id="26a53-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="26a53-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26a53-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-171">displayName</span><span class="sxs-lookup"><span data-stu-id="26a53-171">displayName</span></span>|<span data-ttu-id="26a53-172">String</span><span class="sxs-lookup"><span data-stu-id="26a53-172">String</span></span>|<span data-ttu-id="26a53-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="26a53-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26a53-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-175">version</span><span class="sxs-lookup"><span data-stu-id="26a53-175">version</span></span>|<span data-ttu-id="26a53-176">Int32</span><span class="sxs-lookup"><span data-stu-id="26a53-176">Int32</span></span>|<span data-ttu-id="26a53-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="26a53-177">Version of the device configuration.</span></span> <span data-ttu-id="26a53-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26a53-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a53-179">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="26a53-179">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="26a53-180">購入</span><span class="sxs-lookup"><span data-stu-id="26a53-180">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="26a53-181">デバイス上でのデバイスの正常性の監視を有効にします。</span><span class="sxs-lookup"><span data-stu-id="26a53-181">Enables device health monitoring on the device.</span></span> <span data-ttu-id="26a53-182">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="26a53-182">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="26a53-183">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="26a53-183">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="26a53-184">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="26a53-184">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="26a53-185">正常性の監視が有効になっているデバイスから収集されたイベントのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="26a53-185">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="26a53-186">可能な値は、`undefined`、`healthMonitoring`、`bootPerformance` です。</span><span class="sxs-lookup"><span data-stu-id="26a53-186">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|
|<span data-ttu-id="26a53-187">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="26a53-187">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="26a53-188">String</span><span class="sxs-lookup"><span data-stu-id="26a53-188">String</span></span>|<span data-ttu-id="26a53-189">正常性監視が有効になっているデバイスから収集されたイベントのカスタムセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="26a53-189">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="26a53-190">応答</span><span class="sxs-lookup"><span data-stu-id="26a53-190">Response</span></span>
<span data-ttu-id="26a53-191">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26a53-191">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a53-192">例</span><span class="sxs-lookup"><span data-stu-id="26a53-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="26a53-193">要求</span><span class="sxs-lookup"><span data-stu-id="26a53-193">Request</span></span>
<span data-ttu-id="26a53-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26a53-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26a53-195">応答</span><span class="sxs-lookup"><span data-stu-id="26a53-195">Response</span></span>
<span data-ttu-id="26a53-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26a53-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





