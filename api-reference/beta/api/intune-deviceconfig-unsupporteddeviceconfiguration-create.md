---
title: アン Supporteddevicの作成
description: 新しいアン Supporteddevic/オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6bd1cf05b8effcaa4bedd79fa6cf5c4f99044b59
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338575"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="4c875-103">アン Supporteddevicの作成</span><span class="sxs-lookup"><span data-stu-id="4c875-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="4c875-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c875-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c875-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c875-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c875-106">新しい[アン Supporteddevic/](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c875-106">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c875-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c875-107">Prerequisites</span></span>
<span data-ttu-id="4c875-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c875-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c875-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c875-110">Permission type</span></span>|<span data-ttu-id="4c875-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c875-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c875-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c875-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c875-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c875-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c875-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c875-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c875-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c875-115">Not supported.</span></span>|
|<span data-ttu-id="4c875-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c875-116">Application</span></span>|<span data-ttu-id="4c875-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c875-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c875-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c875-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4c875-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c875-119">Request headers</span></span>
|<span data-ttu-id="4c875-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c875-120">Header</span></span>|<span data-ttu-id="4c875-121">値</span><span class="sxs-lookup"><span data-stu-id="4c875-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c875-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c875-122">Authorization</span></span>|<span data-ttu-id="4c875-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c875-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c875-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4c875-124">Accept</span></span>|<span data-ttu-id="4c875-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c875-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c875-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c875-126">Request body</span></span>
<span data-ttu-id="4c875-127">要求本文で、アン Supporteddevic/オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c875-127">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="4c875-128">次の表に、アン Supporteddevicの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4c875-128">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="4c875-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c875-129">Property</span></span>|<span data-ttu-id="4c875-130">型</span><span class="sxs-lookup"><span data-stu-id="4c875-130">Type</span></span>|<span data-ttu-id="4c875-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c875-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c875-132">id</span><span class="sxs-lookup"><span data-stu-id="4c875-132">id</span></span>|<span data-ttu-id="4c875-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4c875-133">String</span></span>|<span data-ttu-id="4c875-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4c875-134">Key of the entity.</span></span> <span data-ttu-id="4c875-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c875-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4c875-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c875-137">DateTimeOffset</span></span>|<span data-ttu-id="4c875-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4c875-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4c875-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4c875-140">roleScopeTagIds</span></span>|<span data-ttu-id="4c875-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="4c875-141">String collection</span></span>|<span data-ttu-id="4c875-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="4c875-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4c875-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4c875-144">supportsScopeTags</span></span>|<span data-ttu-id="4c875-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c875-145">Boolean</span></span>|<span data-ttu-id="4c875-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c875-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4c875-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="4c875-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4c875-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="4c875-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4c875-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="4c875-149">This property is read-only.</span></span> <span data-ttu-id="4c875-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4c875-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4c875-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4c875-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4c875-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="4c875-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4c875-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4c875-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4c875-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4c875-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4c875-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="4c875-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4c875-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="4c875-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4c875-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="4c875-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4c875-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="4c875-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4c875-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c875-163">createdDateTime</span></span>|<span data-ttu-id="4c875-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c875-164">DateTimeOffset</span></span>|<span data-ttu-id="4c875-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4c875-165">DateTime the object was created.</span></span> <span data-ttu-id="4c875-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-167">description</span><span class="sxs-lookup"><span data-stu-id="4c875-167">description</span></span>|<span data-ttu-id="4c875-168">String</span><span class="sxs-lookup"><span data-stu-id="4c875-168">String</span></span>|<span data-ttu-id="4c875-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="4c875-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4c875-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4c875-171">displayName</span></span>|<span data-ttu-id="4c875-172">String</span><span class="sxs-lookup"><span data-stu-id="4c875-172">String</span></span>|<span data-ttu-id="4c875-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="4c875-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4c875-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-175">version</span><span class="sxs-lookup"><span data-stu-id="4c875-175">version</span></span>|<span data-ttu-id="4c875-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4c875-176">Int32</span></span>|<span data-ttu-id="4c875-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4c875-177">Version of the device configuration.</span></span> <span data-ttu-id="4c875-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c875-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c875-179">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="4c875-179">originalEntityTypeName</span></span>|<span data-ttu-id="4c875-180">String</span><span class="sxs-lookup"><span data-stu-id="4c875-180">String</span></span>|<span data-ttu-id="4c875-181">それ以外の場合に返されるエンティティの種類。</span><span class="sxs-lookup"><span data-stu-id="4c875-181">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="4c875-182">詳細</span><span class="sxs-lookup"><span data-stu-id="4c875-182">details</span></span>|<span data-ttu-id="4c875-183">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c875-183">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="4c875-184">エンティティがサポートされていない理由について説明します。</span><span class="sxs-lookup"><span data-stu-id="4c875-184">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="4c875-185">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="4c875-185">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4c875-186">応答</span><span class="sxs-lookup"><span data-stu-id="4c875-186">Response</span></span>
<span data-ttu-id="4c875-187">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[アン supporteddevicの](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c875-187">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c875-188">例</span><span class="sxs-lookup"><span data-stu-id="4c875-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c875-189">要求</span><span class="sxs-lookup"><span data-stu-id="4c875-189">Request</span></span>
<span data-ttu-id="4c875-190">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c875-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4c875-191">応答</span><span class="sxs-lookup"><span data-stu-id="4c875-191">Response</span></span>
<span data-ttu-id="4c875-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c875-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






