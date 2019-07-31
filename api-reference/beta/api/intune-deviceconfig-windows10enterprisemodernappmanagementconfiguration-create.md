---
title: windows10EnterpriseModernAppManagementConfiguration の作成
description: 新しい windows10EnterpriseModernAppManagementConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ac0439fc996df50b1b043d940cb1c4569957665
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976862"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="36480-103">windows10EnterpriseModernAppManagementConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="36480-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="36480-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36480-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36480-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36480-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36480-106">新しい [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="36480-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36480-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="36480-107">Prerequisites</span></span>
<span data-ttu-id="36480-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36480-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36480-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36480-110">Permission type</span></span>|<span data-ttu-id="36480-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="36480-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36480-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36480-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36480-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36480-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36480-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36480-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36480-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36480-115">Not supported.</span></span>|
|<span data-ttu-id="36480-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36480-116">Application</span></span>|<span data-ttu-id="36480-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36480-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36480-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36480-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36480-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36480-119">Request headers</span></span>
|<span data-ttu-id="36480-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36480-120">Header</span></span>|<span data-ttu-id="36480-121">値</span><span class="sxs-lookup"><span data-stu-id="36480-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36480-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36480-122">Authorization</span></span>|<span data-ttu-id="36480-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="36480-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36480-124">承諾</span><span class="sxs-lookup"><span data-stu-id="36480-124">Accept</span></span>|<span data-ttu-id="36480-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36480-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36480-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="36480-126">Request body</span></span>
<span data-ttu-id="36480-127">要求本文で、windows10EnterpriseModernAppManagementConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="36480-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="36480-128">次の表に、windows10EnterpriseModernAppManagementConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="36480-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="36480-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36480-129">Property</span></span>|<span data-ttu-id="36480-130">型</span><span class="sxs-lookup"><span data-stu-id="36480-130">Type</span></span>|<span data-ttu-id="36480-131">説明</span><span class="sxs-lookup"><span data-stu-id="36480-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36480-132">id</span><span class="sxs-lookup"><span data-stu-id="36480-132">id</span></span>|<span data-ttu-id="36480-133">文字列</span><span class="sxs-lookup"><span data-stu-id="36480-133">String</span></span>|<span data-ttu-id="36480-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="36480-134">Key of the entity.</span></span> <span data-ttu-id="36480-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36480-136">lastModifiedDateTime</span></span>|<span data-ttu-id="36480-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36480-137">DateTimeOffset</span></span>|<span data-ttu-id="36480-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="36480-138">DateTime the object was last modified.</span></span> <span data-ttu-id="36480-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36480-140">roleScopeTagIds</span></span>|<span data-ttu-id="36480-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="36480-141">String collection</span></span>|<span data-ttu-id="36480-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="36480-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36480-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="36480-144">supportsScopeTags</span></span>|<span data-ttu-id="36480-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="36480-145">Boolean</span></span>|<span data-ttu-id="36480-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="36480-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36480-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="36480-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36480-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="36480-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36480-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="36480-149">This property is read-only.</span></span> <span data-ttu-id="36480-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36480-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="36480-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36480-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="36480-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="36480-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="36480-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36480-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="36480-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36480-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="36480-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="36480-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="36480-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="36480-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="36480-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="36480-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="36480-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="36480-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="36480-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36480-163">createdDateTime</span></span>|<span data-ttu-id="36480-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36480-164">DateTimeOffset</span></span>|<span data-ttu-id="36480-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="36480-165">DateTime the object was created.</span></span> <span data-ttu-id="36480-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-167">description</span><span class="sxs-lookup"><span data-stu-id="36480-167">description</span></span>|<span data-ttu-id="36480-168">String</span><span class="sxs-lookup"><span data-stu-id="36480-168">String</span></span>|<span data-ttu-id="36480-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="36480-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36480-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-171">displayName</span><span class="sxs-lookup"><span data-stu-id="36480-171">displayName</span></span>|<span data-ttu-id="36480-172">String</span><span class="sxs-lookup"><span data-stu-id="36480-172">String</span></span>|<span data-ttu-id="36480-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="36480-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36480-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-175">version</span><span class="sxs-lookup"><span data-stu-id="36480-175">version</span></span>|<span data-ttu-id="36480-176">Int32</span><span class="sxs-lookup"><span data-stu-id="36480-176">Int32</span></span>|<span data-ttu-id="36480-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="36480-177">Version of the device configuration.</span></span> <span data-ttu-id="36480-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36480-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36480-179">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="36480-179">uninstallBuiltInApps</span></span>|<span data-ttu-id="36480-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="36480-180">Boolean</span></span>|<span data-ttu-id="36480-181">組み込みの Windows アプリの固定リストをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="36480-181">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="36480-182">応答</span><span class="sxs-lookup"><span data-stu-id="36480-182">Response</span></span>
<span data-ttu-id="36480-183">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="36480-183">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36480-184">例</span><span class="sxs-lookup"><span data-stu-id="36480-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="36480-185">要求</span><span class="sxs-lookup"><span data-stu-id="36480-185">Request</span></span>
<span data-ttu-id="36480-186">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36480-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="36480-187">応答</span><span class="sxs-lookup"><span data-stu-id="36480-187">Response</span></span>
<span data-ttu-id="36480-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36480-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





