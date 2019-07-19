---
title: Androidforwork Trustedrootcertificate の更新
description: Androidforwork Trustedrootcertificate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0501ee47f62c3d241a2e8e8ebe7f987a2d57914e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970395"
---
# <a name="update-androidforworktrustedrootcertificate"></a><span data-ttu-id="2ccf3-103">Androidforwork Trustedrootcertificate の更新</span><span class="sxs-lookup"><span data-stu-id="2ccf3-103">Update androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="2ccf3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ccf3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ccf3-106">[Androidforwork Trustedrootcertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-106">Update the properties of a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ccf3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ccf3-107">Prerequisites</span></span>
<span data-ttu-id="2ccf3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ccf3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ccf3-110">Permission type</span></span>|<span data-ttu-id="2ccf3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ccf3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ccf3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ccf3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ccf3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ccf3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ccf3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ccf3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ccf3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-115">Not supported.</span></span>|
|<span data-ttu-id="2ccf3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ccf3-116">Application</span></span>|<span data-ttu-id="2ccf3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ccf3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ccf3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="2ccf3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ccf3-119">Request headers</span></span>
|<span data-ttu-id="2ccf3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ccf3-120">Header</span></span>|<span data-ttu-id="2ccf3-121">値</span><span class="sxs-lookup"><span data-stu-id="2ccf3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ccf3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ccf3-122">Authorization</span></span>|<span data-ttu-id="2ccf3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ccf3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2ccf3-124">Accept</span></span>|<span data-ttu-id="2ccf3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ccf3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ccf3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ccf3-126">Request body</span></span>
<span data-ttu-id="2ccf3-127">要求本文で、 [Androidforwork Trustedrootcertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-127">In the request body, supply a JSON representation for the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="2ccf3-128">次の表に、 [Androidforwork Trustedrootcertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-128">The following table shows the properties that are required when you create the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span></span>

|<span data-ttu-id="2ccf3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ccf3-129">Property</span></span>|<span data-ttu-id="2ccf3-130">型</span><span class="sxs-lookup"><span data-stu-id="2ccf3-130">Type</span></span>|<span data-ttu-id="2ccf3-131">説明</span><span class="sxs-lookup"><span data-stu-id="2ccf3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ccf3-132">id</span><span class="sxs-lookup"><span data-stu-id="2ccf3-132">id</span></span>|<span data-ttu-id="2ccf3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2ccf3-133">String</span></span>|<span data-ttu-id="2ccf3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-134">Key of the entity.</span></span> <span data-ttu-id="2ccf3-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ccf3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2ccf3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ccf3-137">DateTimeOffset</span></span>|<span data-ttu-id="2ccf3-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2ccf3-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ccf3-140">roleScopeTagIds</span></span>|<span data-ttu-id="2ccf3-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="2ccf3-141">String collection</span></span>|<span data-ttu-id="2ccf3-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2ccf3-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2ccf3-144">supportsScopeTags</span></span>|<span data-ttu-id="2ccf3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ccf3-145">Boolean</span></span>|<span data-ttu-id="2ccf3-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2ccf3-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2ccf3-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2ccf3-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-149">This property is read-only.</span></span> <span data-ttu-id="2ccf3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2ccf3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2ccf3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2ccf3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2ccf3-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2ccf3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2ccf3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2ccf3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2ccf3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2ccf3-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2ccf3-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="2ccf3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2ccf3-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="2ccf3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2ccf3-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2ccf3-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ccf3-163">createdDateTime</span></span>|<span data-ttu-id="2ccf3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ccf3-164">DateTimeOffset</span></span>|<span data-ttu-id="2ccf3-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-165">DateTime the object was created.</span></span> <span data-ttu-id="2ccf3-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-167">description</span><span class="sxs-lookup"><span data-stu-id="2ccf3-167">description</span></span>|<span data-ttu-id="2ccf3-168">String</span><span class="sxs-lookup"><span data-stu-id="2ccf3-168">String</span></span>|<span data-ttu-id="2ccf3-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2ccf3-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2ccf3-171">displayName</span></span>|<span data-ttu-id="2ccf3-172">String</span><span class="sxs-lookup"><span data-stu-id="2ccf3-172">String</span></span>|<span data-ttu-id="2ccf3-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2ccf3-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-175">version</span><span class="sxs-lookup"><span data-stu-id="2ccf3-175">version</span></span>|<span data-ttu-id="2ccf3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2ccf3-176">Int32</span></span>|<span data-ttu-id="2ccf3-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-177">Version of the device configuration.</span></span> <span data-ttu-id="2ccf3-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ccf3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ccf3-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2ccf3-179">trustedRootCertificate</span></span>|<span data-ttu-id="2ccf3-180">Binary</span><span class="sxs-lookup"><span data-stu-id="2ccf3-180">Binary</span></span>|<span data-ttu-id="2ccf3-181">信頼できるルート証明書</span><span class="sxs-lookup"><span data-stu-id="2ccf3-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="2ccf3-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="2ccf3-182">certFileName</span></span>|<span data-ttu-id="2ccf3-183">String</span><span class="sxs-lookup"><span data-stu-id="2ccf3-183">String</span></span>|<span data-ttu-id="2ccf3-184">UI に表示されるファイル名。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="2ccf3-185">応答</span><span class="sxs-lookup"><span data-stu-id="2ccf3-185">Response</span></span>
<span data-ttu-id="2ccf3-186">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Androidforwork trustedrootcertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-186">If successful, this method returns a `200 OK` response code and an updated [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ccf3-187">例</span><span class="sxs-lookup"><span data-stu-id="2ccf3-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ccf3-188">要求</span><span class="sxs-lookup"><span data-stu-id="2ccf3-188">Request</span></span>
<span data-ttu-id="2ccf3-189">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="2ccf3-190">応答</span><span class="sxs-lookup"><span data-stu-id="2ccf3-190">Response</span></span>
<span data-ttu-id="2ccf3-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ccf3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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





