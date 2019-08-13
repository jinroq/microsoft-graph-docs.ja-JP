---
title: MacOSTrustedRootCertificate の更新
description: MacOSTrustedRootCertificate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f732d1e565957c02dba5cba7c54527500e5e6c7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315121"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="b89ff-103">MacOSTrustedRootCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="b89ff-103">Update macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="b89ff-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b89ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b89ff-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b89ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b89ff-106">[MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b89ff-106">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b89ff-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b89ff-107">Prerequisites</span></span>
<span data-ttu-id="b89ff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b89ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b89ff-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b89ff-110">Permission type</span></span>|<span data-ttu-id="b89ff-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b89ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b89ff-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b89ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b89ff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b89ff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b89ff-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b89ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b89ff-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b89ff-115">Not supported.</span></span>|
|<span data-ttu-id="b89ff-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b89ff-116">Application</span></span>|<span data-ttu-id="b89ff-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b89ff-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b89ff-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b89ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="b89ff-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b89ff-119">Request headers</span></span>
|<span data-ttu-id="b89ff-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b89ff-120">Header</span></span>|<span data-ttu-id="b89ff-121">値</span><span class="sxs-lookup"><span data-stu-id="b89ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b89ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b89ff-122">Authorization</span></span>|<span data-ttu-id="b89ff-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b89ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b89ff-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b89ff-124">Accept</span></span>|<span data-ttu-id="b89ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b89ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b89ff-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b89ff-126">Request body</span></span>
<span data-ttu-id="b89ff-127">要求本文で、 [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b89ff-127">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="b89ff-128">次の表に、 [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b89ff-128">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="b89ff-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b89ff-129">Property</span></span>|<span data-ttu-id="b89ff-130">型</span><span class="sxs-lookup"><span data-stu-id="b89ff-130">Type</span></span>|<span data-ttu-id="b89ff-131">説明</span><span class="sxs-lookup"><span data-stu-id="b89ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b89ff-132">id</span><span class="sxs-lookup"><span data-stu-id="b89ff-132">id</span></span>|<span data-ttu-id="b89ff-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b89ff-133">String</span></span>|<span data-ttu-id="b89ff-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b89ff-134">Key of the entity.</span></span> <span data-ttu-id="b89ff-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b89ff-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b89ff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b89ff-137">DateTimeOffset</span></span>|<span data-ttu-id="b89ff-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b89ff-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b89ff-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b89ff-140">roleScopeTagIds</span></span>|<span data-ttu-id="b89ff-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b89ff-141">String collection</span></span>|<span data-ttu-id="b89ff-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b89ff-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b89ff-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b89ff-144">supportsScopeTags</span></span>|<span data-ttu-id="b89ff-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b89ff-145">Boolean</span></span>|<span data-ttu-id="b89ff-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b89ff-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b89ff-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="b89ff-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b89ff-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="b89ff-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b89ff-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="b89ff-149">This property is read-only.</span></span> <span data-ttu-id="b89ff-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b89ff-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b89ff-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b89ff-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b89ff-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="b89ff-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b89ff-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b89ff-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b89ff-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b89ff-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b89ff-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b89ff-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b89ff-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b89ff-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b89ff-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b89ff-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b89ff-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b89ff-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b89ff-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b89ff-163">createdDateTime</span></span>|<span data-ttu-id="b89ff-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b89ff-164">DateTimeOffset</span></span>|<span data-ttu-id="b89ff-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b89ff-165">DateTime the object was created.</span></span> <span data-ttu-id="b89ff-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-167">description</span><span class="sxs-lookup"><span data-stu-id="b89ff-167">description</span></span>|<span data-ttu-id="b89ff-168">String</span><span class="sxs-lookup"><span data-stu-id="b89ff-168">String</span></span>|<span data-ttu-id="b89ff-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b89ff-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b89ff-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b89ff-171">displayName</span></span>|<span data-ttu-id="b89ff-172">String</span><span class="sxs-lookup"><span data-stu-id="b89ff-172">String</span></span>|<span data-ttu-id="b89ff-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b89ff-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b89ff-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-175">version</span><span class="sxs-lookup"><span data-stu-id="b89ff-175">version</span></span>|<span data-ttu-id="b89ff-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b89ff-176">Int32</span></span>|<span data-ttu-id="b89ff-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b89ff-177">Version of the device configuration.</span></span> <span data-ttu-id="b89ff-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b89ff-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b89ff-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b89ff-179">trustedRootCertificate</span></span>|<span data-ttu-id="b89ff-180">Binary</span><span class="sxs-lookup"><span data-stu-id="b89ff-180">Binary</span></span>|<span data-ttu-id="b89ff-181">信頼されたルート証明書。</span><span class="sxs-lookup"><span data-stu-id="b89ff-181">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="b89ff-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="b89ff-182">certFileName</span></span>|<span data-ttu-id="b89ff-183">String</span><span class="sxs-lookup"><span data-stu-id="b89ff-183">String</span></span>|<span data-ttu-id="b89ff-184">UI に表示されるファイル名。</span><span class="sxs-lookup"><span data-stu-id="b89ff-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="b89ff-185">応答</span><span class="sxs-lookup"><span data-stu-id="b89ff-185">Response</span></span>
<span data-ttu-id="b89ff-186">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b89ff-186">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b89ff-187">例</span><span class="sxs-lookup"><span data-stu-id="b89ff-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="b89ff-188">要求</span><span class="sxs-lookup"><span data-stu-id="b89ff-188">Request</span></span>
<span data-ttu-id="b89ff-189">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b89ff-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 1138

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="b89ff-190">応答</span><span class="sxs-lookup"><span data-stu-id="b89ff-190">Response</span></span>
<span data-ttu-id="b89ff-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b89ff-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1310

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```






