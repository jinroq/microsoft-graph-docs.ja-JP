---
title: windows10EnterpriseModernAppManagementConfiguration の更新
description: windows10EnterpriseModernAppManagementConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d9263c2b7471a51c257ee92fadd749af16a3b65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975509"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="42cf8-103">windows10EnterpriseModernAppManagementConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="42cf8-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="42cf8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42cf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42cf8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="42cf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42cf8-106">[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="42cf8-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42cf8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="42cf8-107">Prerequisites</span></span>
<span data-ttu-id="42cf8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42cf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42cf8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42cf8-110">Permission type</span></span>|<span data-ttu-id="42cf8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="42cf8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42cf8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="42cf8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42cf8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42cf8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42cf8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42cf8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42cf8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42cf8-115">Not supported.</span></span>|
|<span data-ttu-id="42cf8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42cf8-116">Application</span></span>|<span data-ttu-id="42cf8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42cf8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42cf8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42cf8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42cf8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42cf8-119">Request headers</span></span>
|<span data-ttu-id="42cf8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42cf8-120">Header</span></span>|<span data-ttu-id="42cf8-121">値</span><span class="sxs-lookup"><span data-stu-id="42cf8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42cf8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42cf8-122">Authorization</span></span>|<span data-ttu-id="42cf8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="42cf8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42cf8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="42cf8-124">Accept</span></span>|<span data-ttu-id="42cf8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42cf8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42cf8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="42cf8-126">Request body</span></span>
<span data-ttu-id="42cf8-127">要求本文で、[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="42cf8-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="42cf8-128">次の表に、[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="42cf8-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="42cf8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42cf8-129">Property</span></span>|<span data-ttu-id="42cf8-130">型</span><span class="sxs-lookup"><span data-stu-id="42cf8-130">Type</span></span>|<span data-ttu-id="42cf8-131">説明</span><span class="sxs-lookup"><span data-stu-id="42cf8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42cf8-132">id</span><span class="sxs-lookup"><span data-stu-id="42cf8-132">id</span></span>|<span data-ttu-id="42cf8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="42cf8-133">String</span></span>|<span data-ttu-id="42cf8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="42cf8-134">Key of the entity.</span></span> <span data-ttu-id="42cf8-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42cf8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="42cf8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42cf8-137">DateTimeOffset</span></span>|<span data-ttu-id="42cf8-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="42cf8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="42cf8-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42cf8-140">roleScopeTagIds</span></span>|<span data-ttu-id="42cf8-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="42cf8-141">String collection</span></span>|<span data-ttu-id="42cf8-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="42cf8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42cf8-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="42cf8-144">supportsScopeTags</span></span>|<span data-ttu-id="42cf8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="42cf8-145">Boolean</span></span>|<span data-ttu-id="42cf8-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="42cf8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="42cf8-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="42cf8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="42cf8-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="42cf8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="42cf8-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="42cf8-149">This property is read-only.</span></span> <span data-ttu-id="42cf8-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42cf8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="42cf8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42cf8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="42cf8-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="42cf8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="42cf8-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42cf8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="42cf8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42cf8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="42cf8-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="42cf8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="42cf8-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="42cf8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="42cf8-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="42cf8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="42cf8-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="42cf8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="42cf8-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42cf8-163">createdDateTime</span></span>|<span data-ttu-id="42cf8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42cf8-164">DateTimeOffset</span></span>|<span data-ttu-id="42cf8-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="42cf8-165">DateTime the object was created.</span></span> <span data-ttu-id="42cf8-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-167">description</span><span class="sxs-lookup"><span data-stu-id="42cf8-167">description</span></span>|<span data-ttu-id="42cf8-168">String</span><span class="sxs-lookup"><span data-stu-id="42cf8-168">String</span></span>|<span data-ttu-id="42cf8-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="42cf8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42cf8-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="42cf8-171">displayName</span></span>|<span data-ttu-id="42cf8-172">String</span><span class="sxs-lookup"><span data-stu-id="42cf8-172">String</span></span>|<span data-ttu-id="42cf8-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="42cf8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42cf8-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-175">version</span><span class="sxs-lookup"><span data-stu-id="42cf8-175">version</span></span>|<span data-ttu-id="42cf8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="42cf8-176">Int32</span></span>|<span data-ttu-id="42cf8-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="42cf8-177">Version of the device configuration.</span></span> <span data-ttu-id="42cf8-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="42cf8-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42cf8-179">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="42cf8-179">uninstallBuiltInApps</span></span>|<span data-ttu-id="42cf8-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="42cf8-180">Boolean</span></span>|<span data-ttu-id="42cf8-181">組み込みの Windows アプリの固定リストをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="42cf8-181">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="42cf8-182">応答</span><span class="sxs-lookup"><span data-stu-id="42cf8-182">Response</span></span>
<span data-ttu-id="42cf8-183">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="42cf8-183">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42cf8-184">例</span><span class="sxs-lookup"><span data-stu-id="42cf8-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="42cf8-185">要求</span><span class="sxs-lookup"><span data-stu-id="42cf8-185">Request</span></span>
<span data-ttu-id="42cf8-186">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="42cf8-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1087

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
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
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="42cf8-187">応答</span><span class="sxs-lookup"><span data-stu-id="42cf8-187">Response</span></span>
<span data-ttu-id="42cf8-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="42cf8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1259

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
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
  "uninstallBuiltInApps": true
}
```





