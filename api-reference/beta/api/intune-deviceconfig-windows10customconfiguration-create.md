---
title: windows10CustomConfiguration の作成
description: 新しい windows10CustomConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 68e2abeff871d45a1e581f3d829ee5db9d6d53a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946132"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="45cd3-103">windows10CustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="45cd3-103">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="45cd3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45cd3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45cd3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45cd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45cd3-106">新しい [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="45cd3-106">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45cd3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="45cd3-107">Prerequisites</span></span>
<span data-ttu-id="45cd3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45cd3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45cd3-110">Permission type</span></span>|<span data-ttu-id="45cd3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="45cd3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45cd3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45cd3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45cd3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45cd3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45cd3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45cd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45cd3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45cd3-115">Not supported.</span></span>|
|<span data-ttu-id="45cd3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45cd3-116">Application</span></span>|<span data-ttu-id="45cd3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45cd3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45cd3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45cd3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45cd3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45cd3-119">Request headers</span></span>
|<span data-ttu-id="45cd3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45cd3-120">Header</span></span>|<span data-ttu-id="45cd3-121">値</span><span class="sxs-lookup"><span data-stu-id="45cd3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45cd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45cd3-122">Authorization</span></span>|<span data-ttu-id="45cd3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="45cd3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45cd3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="45cd3-124">Accept</span></span>|<span data-ttu-id="45cd3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45cd3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45cd3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="45cd3-126">Request body</span></span>
<span data-ttu-id="45cd3-127">要求本文で、windows10CustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="45cd3-127">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="45cd3-128">次の表に、windows10CustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="45cd3-128">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="45cd3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45cd3-129">Property</span></span>|<span data-ttu-id="45cd3-130">型</span><span class="sxs-lookup"><span data-stu-id="45cd3-130">Type</span></span>|<span data-ttu-id="45cd3-131">説明</span><span class="sxs-lookup"><span data-stu-id="45cd3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45cd3-132">id</span><span class="sxs-lookup"><span data-stu-id="45cd3-132">id</span></span>|<span data-ttu-id="45cd3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="45cd3-133">String</span></span>|<span data-ttu-id="45cd3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="45cd3-134">Key of the entity.</span></span> <span data-ttu-id="45cd3-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45cd3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="45cd3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45cd3-137">DateTimeOffset</span></span>|<span data-ttu-id="45cd3-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="45cd3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="45cd3-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45cd3-140">roleScopeTagIds</span></span>|<span data-ttu-id="45cd3-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="45cd3-141">String collection</span></span>|<span data-ttu-id="45cd3-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="45cd3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="45cd3-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="45cd3-144">supportsScopeTags</span></span>|<span data-ttu-id="45cd3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="45cd3-145">Boolean</span></span>|<span data-ttu-id="45cd3-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="45cd3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45cd3-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="45cd3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45cd3-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="45cd3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45cd3-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="45cd3-149">This property is read-only.</span></span> <span data-ttu-id="45cd3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45cd3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="45cd3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45cd3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="45cd3-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="45cd3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="45cd3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45cd3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="45cd3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45cd3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="45cd3-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="45cd3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="45cd3-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="45cd3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="45cd3-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="45cd3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="45cd3-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="45cd3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="45cd3-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45cd3-163">createdDateTime</span></span>|<span data-ttu-id="45cd3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45cd3-164">DateTimeOffset</span></span>|<span data-ttu-id="45cd3-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="45cd3-165">DateTime the object was created.</span></span> <span data-ttu-id="45cd3-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-167">description</span><span class="sxs-lookup"><span data-stu-id="45cd3-167">description</span></span>|<span data-ttu-id="45cd3-168">String</span><span class="sxs-lookup"><span data-stu-id="45cd3-168">String</span></span>|<span data-ttu-id="45cd3-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="45cd3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45cd3-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="45cd3-171">displayName</span></span>|<span data-ttu-id="45cd3-172">String</span><span class="sxs-lookup"><span data-stu-id="45cd3-172">String</span></span>|<span data-ttu-id="45cd3-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="45cd3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45cd3-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-175">version</span><span class="sxs-lookup"><span data-stu-id="45cd3-175">version</span></span>|<span data-ttu-id="45cd3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="45cd3-176">Int32</span></span>|<span data-ttu-id="45cd3-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="45cd3-177">Version of the device configuration.</span></span> <span data-ttu-id="45cd3-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="45cd3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45cd3-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="45cd3-179">omaSettings</span></span>|<span data-ttu-id="45cd3-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="45cd3-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="45cd3-181">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="45cd3-181">OMA settings.</span></span> <span data-ttu-id="45cd3-182">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="45cd3-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="45cd3-183">応答</span><span class="sxs-lookup"><span data-stu-id="45cd3-183">Response</span></span>
<span data-ttu-id="45cd3-184">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="45cd3-184">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45cd3-185">例</span><span class="sxs-lookup"><span data-stu-id="45cd3-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="45cd3-186">要求</span><span class="sxs-lookup"><span data-stu-id="45cd3-186">Request</span></span>
<span data-ttu-id="45cd3-187">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45cd3-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="45cd3-188">応答</span><span class="sxs-lookup"><span data-stu-id="45cd3-188">Response</span></span>
<span data-ttu-id="45cd3-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="45cd3-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





