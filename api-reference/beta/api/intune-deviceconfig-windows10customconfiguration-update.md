---
title: windows10CustomConfiguration の更新
description: windows10CustomConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f69891e9ac5b215cfc914b350829e7ecb462f4bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973458"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="accc1-103">windows10CustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="accc1-103">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="accc1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="accc1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="accc1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="accc1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="accc1-106">[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="accc1-106">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="accc1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="accc1-107">Prerequisites</span></span>
<span data-ttu-id="accc1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="accc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="accc1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="accc1-110">Permission type</span></span>|<span data-ttu-id="accc1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="accc1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="accc1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="accc1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="accc1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="accc1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="accc1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="accc1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="accc1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="accc1-115">Not supported.</span></span>|
|<span data-ttu-id="accc1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="accc1-116">Application</span></span>|<span data-ttu-id="accc1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="accc1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="accc1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="accc1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="accc1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="accc1-119">Request headers</span></span>
|<span data-ttu-id="accc1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="accc1-120">Header</span></span>|<span data-ttu-id="accc1-121">値</span><span class="sxs-lookup"><span data-stu-id="accc1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="accc1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="accc1-122">Authorization</span></span>|<span data-ttu-id="accc1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="accc1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="accc1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="accc1-124">Accept</span></span>|<span data-ttu-id="accc1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="accc1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="accc1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="accc1-126">Request body</span></span>
<span data-ttu-id="accc1-127">要求本文で、[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="accc1-127">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="accc1-128">次の表に、[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="accc1-128">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="accc1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="accc1-129">Property</span></span>|<span data-ttu-id="accc1-130">型</span><span class="sxs-lookup"><span data-stu-id="accc1-130">Type</span></span>|<span data-ttu-id="accc1-131">説明</span><span class="sxs-lookup"><span data-stu-id="accc1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="accc1-132">id</span><span class="sxs-lookup"><span data-stu-id="accc1-132">id</span></span>|<span data-ttu-id="accc1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="accc1-133">String</span></span>|<span data-ttu-id="accc1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="accc1-134">Key of the entity.</span></span> <span data-ttu-id="accc1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="accc1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="accc1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="accc1-137">DateTimeOffset</span></span>|<span data-ttu-id="accc1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="accc1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="accc1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="accc1-140">roleScopeTagIds</span></span>|<span data-ttu-id="accc1-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="accc1-141">String collection</span></span>|<span data-ttu-id="accc1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="accc1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="accc1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="accc1-144">supportsScopeTags</span></span>|<span data-ttu-id="accc1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="accc1-145">Boolean</span></span>|<span data-ttu-id="accc1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="accc1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="accc1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="accc1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="accc1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="accc1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="accc1-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="accc1-149">This property is read-only.</span></span> <span data-ttu-id="accc1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="accc1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="accc1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="accc1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="accc1-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="accc1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="accc1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="accc1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="accc1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="accc1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="accc1-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="accc1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="accc1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="accc1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="accc1-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="accc1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="accc1-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="accc1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="accc1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="accc1-163">createdDateTime</span></span>|<span data-ttu-id="accc1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="accc1-164">DateTimeOffset</span></span>|<span data-ttu-id="accc1-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="accc1-165">DateTime the object was created.</span></span> <span data-ttu-id="accc1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-167">description</span><span class="sxs-lookup"><span data-stu-id="accc1-167">description</span></span>|<span data-ttu-id="accc1-168">String</span><span class="sxs-lookup"><span data-stu-id="accc1-168">String</span></span>|<span data-ttu-id="accc1-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="accc1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="accc1-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="accc1-171">displayName</span></span>|<span data-ttu-id="accc1-172">String</span><span class="sxs-lookup"><span data-stu-id="accc1-172">String</span></span>|<span data-ttu-id="accc1-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="accc1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="accc1-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-175">version</span><span class="sxs-lookup"><span data-stu-id="accc1-175">version</span></span>|<span data-ttu-id="accc1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="accc1-176">Int32</span></span>|<span data-ttu-id="accc1-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="accc1-177">Version of the device configuration.</span></span> <span data-ttu-id="accc1-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="accc1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="accc1-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="accc1-179">omaSettings</span></span>|<span data-ttu-id="accc1-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="accc1-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="accc1-181">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="accc1-181">OMA settings.</span></span> <span data-ttu-id="accc1-182">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="accc1-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="accc1-183">応答</span><span class="sxs-lookup"><span data-stu-id="accc1-183">Response</span></span>
<span data-ttu-id="accc1-184">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="accc1-184">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="accc1-185">例</span><span class="sxs-lookup"><span data-stu-id="accc1-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="accc1-186">要求</span><span class="sxs-lookup"><span data-stu-id="accc1-186">Request</span></span>
<span data-ttu-id="accc1-187">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="accc1-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1296

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="accc1-188">応答</span><span class="sxs-lookup"><span data-stu-id="accc1-188">Response</span></span>
<span data-ttu-id="accc1-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="accc1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1468

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```





