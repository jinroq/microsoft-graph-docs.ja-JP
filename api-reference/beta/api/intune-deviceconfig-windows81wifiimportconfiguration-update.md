---
title: Windows81WifiImportConfiguration の更新
description: Windows81WifiImportConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e7034fa178f60f5e443d46de41375730c0d6beb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314071"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="72577-103">Windows81WifiImportConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="72577-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="72577-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72577-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72577-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="72577-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72577-106">[Windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="72577-106">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72577-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="72577-107">Prerequisites</span></span>
<span data-ttu-id="72577-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72577-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72577-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72577-110">Permission type</span></span>|<span data-ttu-id="72577-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="72577-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72577-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72577-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72577-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72577-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72577-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72577-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72577-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72577-115">Not supported.</span></span>|
|<span data-ttu-id="72577-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72577-116">Application</span></span>|<span data-ttu-id="72577-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72577-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72577-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72577-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="72577-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72577-119">Request headers</span></span>
|<span data-ttu-id="72577-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72577-120">Header</span></span>|<span data-ttu-id="72577-121">値</span><span class="sxs-lookup"><span data-stu-id="72577-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72577-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72577-122">Authorization</span></span>|<span data-ttu-id="72577-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="72577-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72577-124">承諾</span><span class="sxs-lookup"><span data-stu-id="72577-124">Accept</span></span>|<span data-ttu-id="72577-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72577-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72577-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="72577-126">Request body</span></span>
<span data-ttu-id="72577-127">要求本文で、 [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="72577-127">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="72577-128">次の表に、 [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="72577-128">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="72577-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72577-129">Property</span></span>|<span data-ttu-id="72577-130">型</span><span class="sxs-lookup"><span data-stu-id="72577-130">Type</span></span>|<span data-ttu-id="72577-131">説明</span><span class="sxs-lookup"><span data-stu-id="72577-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72577-132">id</span><span class="sxs-lookup"><span data-stu-id="72577-132">id</span></span>|<span data-ttu-id="72577-133">文字列</span><span class="sxs-lookup"><span data-stu-id="72577-133">String</span></span>|<span data-ttu-id="72577-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="72577-134">Key of the entity.</span></span> <span data-ttu-id="72577-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72577-136">lastModifiedDateTime</span></span>|<span data-ttu-id="72577-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72577-137">DateTimeOffset</span></span>|<span data-ttu-id="72577-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="72577-138">DateTime the object was last modified.</span></span> <span data-ttu-id="72577-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="72577-140">roleScopeTagIds</span></span>|<span data-ttu-id="72577-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="72577-141">String collection</span></span>|<span data-ttu-id="72577-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="72577-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="72577-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="72577-144">supportsScopeTags</span></span>|<span data-ttu-id="72577-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="72577-145">Boolean</span></span>|<span data-ttu-id="72577-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="72577-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="72577-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="72577-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="72577-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="72577-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="72577-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="72577-149">This property is read-only.</span></span> <span data-ttu-id="72577-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="72577-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="72577-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="72577-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="72577-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="72577-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="72577-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="72577-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="72577-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="72577-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="72577-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="72577-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="72577-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="72577-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="72577-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="72577-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="72577-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="72577-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="72577-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72577-163">createdDateTime</span></span>|<span data-ttu-id="72577-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72577-164">DateTimeOffset</span></span>|<span data-ttu-id="72577-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="72577-165">DateTime the object was created.</span></span> <span data-ttu-id="72577-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-167">description</span><span class="sxs-lookup"><span data-stu-id="72577-167">description</span></span>|<span data-ttu-id="72577-168">String</span><span class="sxs-lookup"><span data-stu-id="72577-168">String</span></span>|<span data-ttu-id="72577-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="72577-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="72577-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-171">displayName</span><span class="sxs-lookup"><span data-stu-id="72577-171">displayName</span></span>|<span data-ttu-id="72577-172">String</span><span class="sxs-lookup"><span data-stu-id="72577-172">String</span></span>|<span data-ttu-id="72577-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="72577-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="72577-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-175">version</span><span class="sxs-lookup"><span data-stu-id="72577-175">version</span></span>|<span data-ttu-id="72577-176">Int32</span><span class="sxs-lookup"><span data-stu-id="72577-176">Int32</span></span>|<span data-ttu-id="72577-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="72577-177">Version of the device configuration.</span></span> <span data-ttu-id="72577-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72577-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72577-179">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="72577-179">payloadFileName</span></span>|<span data-ttu-id="72577-180">String</span><span class="sxs-lookup"><span data-stu-id="72577-180">String</span></span>|<span data-ttu-id="72577-181">ペイロードファイル名 (\* .xml)。</span><span class="sxs-lookup"><span data-stu-id="72577-181">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="72577-182">profileName</span><span class="sxs-lookup"><span data-stu-id="72577-182">profileName</span></span>|<span data-ttu-id="72577-183">String</span><span class="sxs-lookup"><span data-stu-id="72577-183">String</span></span>|<span data-ttu-id="72577-184">UI に表示されるプロファイル名。</span><span class="sxs-lookup"><span data-stu-id="72577-184">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="72577-185">payload</span><span class="sxs-lookup"><span data-stu-id="72577-185">payload</span></span>|<span data-ttu-id="72577-186">Binary</span><span class="sxs-lookup"><span data-stu-id="72577-186">Binary</span></span>|<span data-ttu-id="72577-187">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="72577-187">Payload.</span></span> <span data-ttu-id="72577-188">(UTF8 でエンコードされたバイト配列)。</span><span class="sxs-lookup"><span data-stu-id="72577-188">(UTF8 encoded byte array).</span></span> <span data-ttu-id="72577-189">これは、Wi-fi エンドポイントへの接続に使用したデバイスに保存された XML ファイルです。</span><span class="sxs-lookup"><span data-stu-id="72577-189">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="72577-190">応答</span><span class="sxs-lookup"><span data-stu-id="72577-190">Response</span></span>
<span data-ttu-id="72577-191">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="72577-191">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72577-192">例</span><span class="sxs-lookup"><span data-stu-id="72577-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="72577-193">要求</span><span class="sxs-lookup"><span data-stu-id="72577-193">Request</span></span>
<span data-ttu-id="72577-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="72577-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1154

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="72577-195">応答</span><span class="sxs-lookup"><span data-stu-id="72577-195">Response</span></span>
<span data-ttu-id="72577-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72577-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1326

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```






