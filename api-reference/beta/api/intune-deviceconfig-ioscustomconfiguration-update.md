---
title: iosCustomConfiguration の更新
description: iosCustomConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 734198b171d58ad47d445eb2036d699e785952d4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339569"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="ef626-103">iosCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ef626-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="ef626-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef626-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef626-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ef626-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef626-106">[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ef626-106">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef626-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ef626-107">Prerequisites</span></span>
<span data-ttu-id="ef626-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef626-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef626-110">Permission type</span></span>|<span data-ttu-id="ef626-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef626-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef626-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ef626-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef626-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef626-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef626-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef626-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef626-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef626-115">Not supported.</span></span>|
|<span data-ttu-id="ef626-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef626-116">Application</span></span>|<span data-ttu-id="ef626-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef626-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef626-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef626-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef626-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef626-119">Request headers</span></span>
|<span data-ttu-id="ef626-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef626-120">Header</span></span>|<span data-ttu-id="ef626-121">値</span><span class="sxs-lookup"><span data-stu-id="ef626-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef626-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef626-122">Authorization</span></span>|<span data-ttu-id="ef626-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ef626-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef626-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ef626-124">Accept</span></span>|<span data-ttu-id="ef626-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef626-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef626-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ef626-126">Request body</span></span>
<span data-ttu-id="ef626-127">要求本文で、[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef626-127">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="ef626-128">次の表に、[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ef626-128">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="ef626-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef626-129">Property</span></span>|<span data-ttu-id="ef626-130">型</span><span class="sxs-lookup"><span data-stu-id="ef626-130">Type</span></span>|<span data-ttu-id="ef626-131">説明</span><span class="sxs-lookup"><span data-stu-id="ef626-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef626-132">id</span><span class="sxs-lookup"><span data-stu-id="ef626-132">id</span></span>|<span data-ttu-id="ef626-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ef626-133">String</span></span>|<span data-ttu-id="ef626-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ef626-134">Key of the entity.</span></span> <span data-ttu-id="ef626-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef626-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ef626-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef626-137">DateTimeOffset</span></span>|<span data-ttu-id="ef626-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ef626-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ef626-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef626-140">roleScopeTagIds</span></span>|<span data-ttu-id="ef626-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ef626-141">String collection</span></span>|<span data-ttu-id="ef626-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ef626-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef626-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ef626-144">supportsScopeTags</span></span>|<span data-ttu-id="ef626-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef626-145">Boolean</span></span>|<span data-ttu-id="ef626-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ef626-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ef626-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="ef626-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ef626-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="ef626-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ef626-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ef626-149">This property is read-only.</span></span> <span data-ttu-id="ef626-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef626-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ef626-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef626-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ef626-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="ef626-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ef626-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef626-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ef626-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef626-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ef626-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ef626-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ef626-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ef626-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ef626-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ef626-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ef626-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ef626-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ef626-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef626-163">createdDateTime</span></span>|<span data-ttu-id="ef626-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef626-164">DateTimeOffset</span></span>|<span data-ttu-id="ef626-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ef626-165">DateTime the object was created.</span></span> <span data-ttu-id="ef626-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-167">description</span><span class="sxs-lookup"><span data-stu-id="ef626-167">description</span></span>|<span data-ttu-id="ef626-168">String</span><span class="sxs-lookup"><span data-stu-id="ef626-168">String</span></span>|<span data-ttu-id="ef626-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ef626-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef626-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ef626-171">displayName</span></span>|<span data-ttu-id="ef626-172">String</span><span class="sxs-lookup"><span data-stu-id="ef626-172">String</span></span>|<span data-ttu-id="ef626-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ef626-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef626-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-175">version</span><span class="sxs-lookup"><span data-stu-id="ef626-175">version</span></span>|<span data-ttu-id="ef626-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ef626-176">Int32</span></span>|<span data-ttu-id="ef626-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ef626-177">Version of the device configuration.</span></span> <span data-ttu-id="ef626-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef626-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef626-179">payloadName</span><span class="sxs-lookup"><span data-stu-id="ef626-179">payloadName</span></span>|<span data-ttu-id="ef626-180">String</span><span class="sxs-lookup"><span data-stu-id="ef626-180">String</span></span>|<span data-ttu-id="ef626-181">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="ef626-181">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="ef626-182">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="ef626-182">payloadFileName</span></span>|<span data-ttu-id="ef626-183">String</span><span class="sxs-lookup"><span data-stu-id="ef626-183">String</span></span>|<span data-ttu-id="ef626-184">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="ef626-184">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="ef626-185">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="ef626-185">\*.xml).</span></span>|
|<span data-ttu-id="ef626-186">payload</span><span class="sxs-lookup"><span data-stu-id="ef626-186">payload</span></span>|<span data-ttu-id="ef626-187">Binary</span><span class="sxs-lookup"><span data-stu-id="ef626-187">Binary</span></span>|<span data-ttu-id="ef626-188">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="ef626-188">Payload.</span></span> <span data-ttu-id="ef626-189">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="ef626-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="ef626-190">応答</span><span class="sxs-lookup"><span data-stu-id="ef626-190">Response</span></span>
<span data-ttu-id="ef626-191">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ef626-191">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef626-192">例</span><span class="sxs-lookup"><span data-stu-id="ef626-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef626-193">要求</span><span class="sxs-lookup"><span data-stu-id="ef626-193">Request</span></span>
<span data-ttu-id="ef626-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ef626-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1144

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="ef626-195">応答</span><span class="sxs-lookup"><span data-stu-id="ef626-195">Response</span></span>
<span data-ttu-id="ef626-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ef626-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1316

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```






