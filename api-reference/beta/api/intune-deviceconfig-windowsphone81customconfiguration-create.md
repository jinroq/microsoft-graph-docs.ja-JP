---
title: windowsPhone81CustomConfiguration の作成
description: 新しい windowsPhone81CustomConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29697a6e10fa61b11f627c1db39217a44bae51b0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977514"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="160de-103">windowsPhone81CustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="160de-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="160de-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="160de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="160de-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="160de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="160de-106">新しい [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="160de-106">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="160de-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="160de-107">Prerequisites</span></span>
<span data-ttu-id="160de-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="160de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="160de-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="160de-110">Permission type</span></span>|<span data-ttu-id="160de-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="160de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="160de-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="160de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="160de-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="160de-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="160de-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="160de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="160de-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="160de-115">Not supported.</span></span>|
|<span data-ttu-id="160de-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="160de-116">Application</span></span>|<span data-ttu-id="160de-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="160de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="160de-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="160de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="160de-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="160de-119">Request headers</span></span>
|<span data-ttu-id="160de-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="160de-120">Header</span></span>|<span data-ttu-id="160de-121">値</span><span class="sxs-lookup"><span data-stu-id="160de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="160de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="160de-122">Authorization</span></span>|<span data-ttu-id="160de-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="160de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="160de-124">承諾</span><span class="sxs-lookup"><span data-stu-id="160de-124">Accept</span></span>|<span data-ttu-id="160de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="160de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="160de-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="160de-126">Request body</span></span>
<span data-ttu-id="160de-127">要求本文で、windowsPhone81CustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="160de-127">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="160de-128">次の表に、windowsPhone81CustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="160de-128">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="160de-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="160de-129">Property</span></span>|<span data-ttu-id="160de-130">型</span><span class="sxs-lookup"><span data-stu-id="160de-130">Type</span></span>|<span data-ttu-id="160de-131">説明</span><span class="sxs-lookup"><span data-stu-id="160de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="160de-132">id</span><span class="sxs-lookup"><span data-stu-id="160de-132">id</span></span>|<span data-ttu-id="160de-133">文字列</span><span class="sxs-lookup"><span data-stu-id="160de-133">String</span></span>|<span data-ttu-id="160de-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="160de-134">Key of the entity.</span></span> <span data-ttu-id="160de-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="160de-136">lastModifiedDateTime</span></span>|<span data-ttu-id="160de-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="160de-137">DateTimeOffset</span></span>|<span data-ttu-id="160de-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="160de-138">DateTime the object was last modified.</span></span> <span data-ttu-id="160de-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="160de-140">roleScopeTagIds</span></span>|<span data-ttu-id="160de-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="160de-141">String collection</span></span>|<span data-ttu-id="160de-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="160de-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="160de-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="160de-144">supportsScopeTags</span></span>|<span data-ttu-id="160de-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="160de-145">Boolean</span></span>|<span data-ttu-id="160de-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="160de-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="160de-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="160de-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="160de-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="160de-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="160de-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="160de-149">This property is read-only.</span></span> <span data-ttu-id="160de-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="160de-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="160de-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="160de-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="160de-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="160de-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="160de-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="160de-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="160de-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="160de-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="160de-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="160de-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="160de-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="160de-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="160de-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="160de-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="160de-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="160de-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="160de-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="160de-163">createdDateTime</span></span>|<span data-ttu-id="160de-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="160de-164">DateTimeOffset</span></span>|<span data-ttu-id="160de-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="160de-165">DateTime the object was created.</span></span> <span data-ttu-id="160de-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-167">description</span><span class="sxs-lookup"><span data-stu-id="160de-167">description</span></span>|<span data-ttu-id="160de-168">String</span><span class="sxs-lookup"><span data-stu-id="160de-168">String</span></span>|<span data-ttu-id="160de-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="160de-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="160de-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-171">displayName</span><span class="sxs-lookup"><span data-stu-id="160de-171">displayName</span></span>|<span data-ttu-id="160de-172">String</span><span class="sxs-lookup"><span data-stu-id="160de-172">String</span></span>|<span data-ttu-id="160de-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="160de-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="160de-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-175">version</span><span class="sxs-lookup"><span data-stu-id="160de-175">version</span></span>|<span data-ttu-id="160de-176">Int32</span><span class="sxs-lookup"><span data-stu-id="160de-176">Int32</span></span>|<span data-ttu-id="160de-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="160de-177">Version of the device configuration.</span></span> <span data-ttu-id="160de-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="160de-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="160de-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="160de-179">omaSettings</span></span>|<span data-ttu-id="160de-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="160de-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="160de-181">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="160de-181">OMA settings.</span></span> <span data-ttu-id="160de-182">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="160de-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="160de-183">応答</span><span class="sxs-lookup"><span data-stu-id="160de-183">Response</span></span>
<span data-ttu-id="160de-184">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="160de-184">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="160de-185">例</span><span class="sxs-lookup"><span data-stu-id="160de-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="160de-186">要求</span><span class="sxs-lookup"><span data-stu-id="160de-186">Request</span></span>
<span data-ttu-id="160de-187">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="160de-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1301

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="160de-188">応答</span><span class="sxs-lookup"><span data-stu-id="160de-188">Response</span></span>
<span data-ttu-id="160de-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="160de-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1473

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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





