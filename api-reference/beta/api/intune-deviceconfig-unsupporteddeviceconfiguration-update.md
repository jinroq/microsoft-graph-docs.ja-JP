---
title: アン Supporteddevic/の更新
description: 非 Supporteddevic/オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e45c93c27ce31704b6a24391307f4e40252fbf90
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338556"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="62697-103">アン Supporteddevic/の更新</span><span class="sxs-lookup"><span data-stu-id="62697-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="62697-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62697-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62697-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62697-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62697-106">非[Supporteddevic/](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="62697-106">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62697-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="62697-107">Prerequisites</span></span>
<span data-ttu-id="62697-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62697-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62697-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62697-110">Permission type</span></span>|<span data-ttu-id="62697-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="62697-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62697-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62697-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62697-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62697-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62697-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62697-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62697-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62697-115">Not supported.</span></span>|
|<span data-ttu-id="62697-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62697-116">Application</span></span>|<span data-ttu-id="62697-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62697-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62697-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62697-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="62697-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62697-119">Request headers</span></span>
|<span data-ttu-id="62697-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62697-120">Header</span></span>|<span data-ttu-id="62697-121">値</span><span class="sxs-lookup"><span data-stu-id="62697-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62697-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62697-122">Authorization</span></span>|<span data-ttu-id="62697-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="62697-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62697-124">承諾</span><span class="sxs-lookup"><span data-stu-id="62697-124">Accept</span></span>|<span data-ttu-id="62697-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62697-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62697-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="62697-126">Request body</span></span>
<span data-ttu-id="62697-127">要求本文で、[アン Supporteddevic/](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="62697-127">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="62697-128">次の表に、[アン Supporteddevicの](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="62697-128">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="62697-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62697-129">Property</span></span>|<span data-ttu-id="62697-130">型</span><span class="sxs-lookup"><span data-stu-id="62697-130">Type</span></span>|<span data-ttu-id="62697-131">説明</span><span class="sxs-lookup"><span data-stu-id="62697-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62697-132">id</span><span class="sxs-lookup"><span data-stu-id="62697-132">id</span></span>|<span data-ttu-id="62697-133">文字列</span><span class="sxs-lookup"><span data-stu-id="62697-133">String</span></span>|<span data-ttu-id="62697-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="62697-134">Key of the entity.</span></span> <span data-ttu-id="62697-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62697-136">lastModifiedDateTime</span></span>|<span data-ttu-id="62697-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62697-137">DateTimeOffset</span></span>|<span data-ttu-id="62697-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="62697-138">DateTime the object was last modified.</span></span> <span data-ttu-id="62697-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62697-140">roleScopeTagIds</span></span>|<span data-ttu-id="62697-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="62697-141">String collection</span></span>|<span data-ttu-id="62697-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="62697-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62697-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62697-144">supportsScopeTags</span></span>|<span data-ttu-id="62697-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="62697-145">Boolean</span></span>|<span data-ttu-id="62697-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62697-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62697-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="62697-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62697-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="62697-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62697-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="62697-149">This property is read-only.</span></span> <span data-ttu-id="62697-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="62697-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="62697-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="62697-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="62697-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="62697-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="62697-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="62697-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="62697-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="62697-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="62697-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="62697-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="62697-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="62697-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="62697-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="62697-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="62697-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="62697-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="62697-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62697-163">createdDateTime</span></span>|<span data-ttu-id="62697-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62697-164">DateTimeOffset</span></span>|<span data-ttu-id="62697-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="62697-165">DateTime the object was created.</span></span> <span data-ttu-id="62697-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-167">description</span><span class="sxs-lookup"><span data-stu-id="62697-167">description</span></span>|<span data-ttu-id="62697-168">String</span><span class="sxs-lookup"><span data-stu-id="62697-168">String</span></span>|<span data-ttu-id="62697-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="62697-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62697-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-171">displayName</span><span class="sxs-lookup"><span data-stu-id="62697-171">displayName</span></span>|<span data-ttu-id="62697-172">String</span><span class="sxs-lookup"><span data-stu-id="62697-172">String</span></span>|<span data-ttu-id="62697-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="62697-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62697-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-175">version</span><span class="sxs-lookup"><span data-stu-id="62697-175">version</span></span>|<span data-ttu-id="62697-176">Int32</span><span class="sxs-lookup"><span data-stu-id="62697-176">Int32</span></span>|<span data-ttu-id="62697-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="62697-177">Version of the device configuration.</span></span> <span data-ttu-id="62697-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62697-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62697-179">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="62697-179">originalEntityTypeName</span></span>|<span data-ttu-id="62697-180">String</span><span class="sxs-lookup"><span data-stu-id="62697-180">String</span></span>|<span data-ttu-id="62697-181">それ以外の場合に返されるエンティティの種類。</span><span class="sxs-lookup"><span data-stu-id="62697-181">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="62697-182">詳細</span><span class="sxs-lookup"><span data-stu-id="62697-182">details</span></span>|<span data-ttu-id="62697-183">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62697-183">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="62697-184">エンティティがサポートされていない理由について説明します。</span><span class="sxs-lookup"><span data-stu-id="62697-184">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="62697-185">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="62697-185">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="62697-186">応答</span><span class="sxs-lookup"><span data-stu-id="62697-186">Response</span></span>
<span data-ttu-id="62697-187">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された非[supporteddevicの](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62697-187">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62697-188">例</span><span class="sxs-lookup"><span data-stu-id="62697-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="62697-189">要求</span><span class="sxs-lookup"><span data-stu-id="62697-189">Request</span></span>
<span data-ttu-id="62697-190">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62697-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1291

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
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
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="62697-191">応答</span><span class="sxs-lookup"><span data-stu-id="62697-191">Response</span></span>
<span data-ttu-id="62697-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62697-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1463

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
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
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```






