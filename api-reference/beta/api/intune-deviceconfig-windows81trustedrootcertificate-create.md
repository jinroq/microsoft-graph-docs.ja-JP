---
title: Windows81TrustedRootCertificate を作成する
description: 新しい windows81TrustedRootCertificate オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f3c38ff8695eff9b194f51dfb74580b1a845eea2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974928"
---
# <a name="create-windows81trustedrootcertificate"></a><span data-ttu-id="a206d-103">Windows81TrustedRootCertificate を作成する</span><span class="sxs-lookup"><span data-stu-id="a206d-103">Create windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="a206d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a206d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a206d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a206d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a206d-106">新しい[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a206d-106">Create a new [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a206d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a206d-107">Prerequisites</span></span>
<span data-ttu-id="a206d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a206d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a206d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a206d-110">Permission type</span></span>|<span data-ttu-id="a206d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a206d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a206d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a206d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a206d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a206d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a206d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a206d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a206d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a206d-115">Not supported.</span></span>|
|<span data-ttu-id="a206d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a206d-116">Application</span></span>|<span data-ttu-id="a206d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a206d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a206d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a206d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="a206d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a206d-119">Request headers</span></span>
|<span data-ttu-id="a206d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a206d-120">Header</span></span>|<span data-ttu-id="a206d-121">値</span><span class="sxs-lookup"><span data-stu-id="a206d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a206d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a206d-122">Authorization</span></span>|<span data-ttu-id="a206d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a206d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a206d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a206d-124">Accept</span></span>|<span data-ttu-id="a206d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a206d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a206d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a206d-126">Request body</span></span>
<span data-ttu-id="a206d-127">要求本文で、windows81TrustedRootCertificate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a206d-127">In the request body, supply a JSON representation for the windows81TrustedRootCertificate object.</span></span>

<span data-ttu-id="a206d-128">次の表に、windows81TrustedRootCertificate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a206d-128">The following table shows the properties that are required when you create the windows81TrustedRootCertificate.</span></span>

|<span data-ttu-id="a206d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a206d-129">Property</span></span>|<span data-ttu-id="a206d-130">型</span><span class="sxs-lookup"><span data-stu-id="a206d-130">Type</span></span>|<span data-ttu-id="a206d-131">説明</span><span class="sxs-lookup"><span data-stu-id="a206d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a206d-132">id</span><span class="sxs-lookup"><span data-stu-id="a206d-132">id</span></span>|<span data-ttu-id="a206d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a206d-133">String</span></span>|<span data-ttu-id="a206d-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a206d-134">Key of the entity.</span></span> <span data-ttu-id="a206d-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a206d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a206d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a206d-137">DateTimeOffset</span></span>|<span data-ttu-id="a206d-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a206d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a206d-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a206d-140">roleScopeTagIds</span></span>|<span data-ttu-id="a206d-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a206d-141">String collection</span></span>|<span data-ttu-id="a206d-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a206d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a206d-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a206d-144">supportsScopeTags</span></span>|<span data-ttu-id="a206d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a206d-145">Boolean</span></span>|<span data-ttu-id="a206d-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a206d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a206d-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a206d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a206d-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a206d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a206d-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a206d-149">This property is read-only.</span></span> <span data-ttu-id="a206d-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a206d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a206d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a206d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a206d-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="a206d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a206d-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a206d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a206d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a206d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a206d-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="a206d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a206d-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="a206d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a206d-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="a206d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a206d-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="a206d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a206d-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a206d-163">createdDateTime</span></span>|<span data-ttu-id="a206d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a206d-164">DateTimeOffset</span></span>|<span data-ttu-id="a206d-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a206d-165">DateTime the object was created.</span></span> <span data-ttu-id="a206d-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-167">description</span><span class="sxs-lookup"><span data-stu-id="a206d-167">description</span></span>|<span data-ttu-id="a206d-168">String</span><span class="sxs-lookup"><span data-stu-id="a206d-168">String</span></span>|<span data-ttu-id="a206d-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a206d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a206d-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a206d-171">displayName</span></span>|<span data-ttu-id="a206d-172">String</span><span class="sxs-lookup"><span data-stu-id="a206d-172">String</span></span>|<span data-ttu-id="a206d-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a206d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a206d-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-175">version</span><span class="sxs-lookup"><span data-stu-id="a206d-175">version</span></span>|<span data-ttu-id="a206d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a206d-176">Int32</span></span>|<span data-ttu-id="a206d-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a206d-177">Version of the device configuration.</span></span> <span data-ttu-id="a206d-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a206d-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a206d-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a206d-179">trustedRootCertificate</span></span>|<span data-ttu-id="a206d-180">Binary</span><span class="sxs-lookup"><span data-stu-id="a206d-180">Binary</span></span>|<span data-ttu-id="a206d-181">信頼できるルート証明書</span><span class="sxs-lookup"><span data-stu-id="a206d-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="a206d-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="a206d-182">certFileName</span></span>|<span data-ttu-id="a206d-183">String</span><span class="sxs-lookup"><span data-stu-id="a206d-183">String</span></span>|<span data-ttu-id="a206d-184">UI に表示されるファイル名。</span><span class="sxs-lookup"><span data-stu-id="a206d-184">File name to display in UI.</span></span>|
|<span data-ttu-id="a206d-185">destinationStore</span><span class="sxs-lookup"><span data-stu-id="a206d-185">destinationStore</span></span>|[<span data-ttu-id="a206d-186">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="a206d-186">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="a206d-187">信頼されたルート証明書の保存先の場所。</span><span class="sxs-lookup"><span data-stu-id="a206d-187">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="a206d-188">可能な値は、`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate` です。</span><span class="sxs-lookup"><span data-stu-id="a206d-188">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="a206d-189">応答</span><span class="sxs-lookup"><span data-stu-id="a206d-189">Response</span></span>
<span data-ttu-id="a206d-190">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a206d-190">If successful, this method returns a `201 Created` response code and a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a206d-191">例</span><span class="sxs-lookup"><span data-stu-id="a206d-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="a206d-192">要求</span><span class="sxs-lookup"><span data-stu-id="a206d-192">Request</span></span>
<span data-ttu-id="a206d-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a206d-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
Content-type: application/json
Content-length: 1198

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="a206d-194">応答</span><span class="sxs-lookup"><span data-stu-id="a206d-194">Response</span></span>
<span data-ttu-id="a206d-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a206d-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1370

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```





