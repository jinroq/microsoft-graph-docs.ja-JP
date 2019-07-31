---
title: IosEduDeviceConfiguration 作成する
description: 新しい iosEduDeviceConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0179535d78b364e22d103c8de83f8b7befc9a97
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948363"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="77bbb-103">IosEduDeviceConfiguration 作成する</span><span class="sxs-lookup"><span data-stu-id="77bbb-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="77bbb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77bbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77bbb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="77bbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77bbb-106">新しい[Iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="77bbb-106">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77bbb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="77bbb-107">Prerequisites</span></span>
<span data-ttu-id="77bbb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77bbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77bbb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77bbb-110">Permission type</span></span>|<span data-ttu-id="77bbb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="77bbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77bbb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77bbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77bbb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77bbb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77bbb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77bbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77bbb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77bbb-115">Not supported.</span></span>|
|<span data-ttu-id="77bbb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77bbb-116">Application</span></span>|<span data-ttu-id="77bbb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77bbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77bbb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77bbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77bbb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77bbb-119">Request headers</span></span>
|<span data-ttu-id="77bbb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77bbb-120">Header</span></span>|<span data-ttu-id="77bbb-121">値</span><span class="sxs-lookup"><span data-stu-id="77bbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77bbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77bbb-122">Authorization</span></span>|<span data-ttu-id="77bbb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="77bbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77bbb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="77bbb-124">Accept</span></span>|<span data-ttu-id="77bbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77bbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77bbb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="77bbb-126">Request body</span></span>
<span data-ttu-id="77bbb-127">要求本文で、iosEduDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77bbb-127">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="77bbb-128">次の表に、iosEduDeviceConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="77bbb-128">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="77bbb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77bbb-129">Property</span></span>|<span data-ttu-id="77bbb-130">型</span><span class="sxs-lookup"><span data-stu-id="77bbb-130">Type</span></span>|<span data-ttu-id="77bbb-131">説明</span><span class="sxs-lookup"><span data-stu-id="77bbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77bbb-132">id</span><span class="sxs-lookup"><span data-stu-id="77bbb-132">id</span></span>|<span data-ttu-id="77bbb-133">文字列</span><span class="sxs-lookup"><span data-stu-id="77bbb-133">String</span></span>|<span data-ttu-id="77bbb-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="77bbb-134">Key of the entity.</span></span> <span data-ttu-id="77bbb-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77bbb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="77bbb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77bbb-137">DateTimeOffset</span></span>|<span data-ttu-id="77bbb-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="77bbb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="77bbb-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77bbb-140">roleScopeTagIds</span></span>|<span data-ttu-id="77bbb-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="77bbb-141">String collection</span></span>|<span data-ttu-id="77bbb-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="77bbb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77bbb-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77bbb-144">supportsScopeTags</span></span>|<span data-ttu-id="77bbb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="77bbb-145">Boolean</span></span>|<span data-ttu-id="77bbb-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="77bbb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77bbb-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="77bbb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77bbb-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="77bbb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77bbb-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="77bbb-149">This property is read-only.</span></span> <span data-ttu-id="77bbb-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="77bbb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="77bbb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="77bbb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="77bbb-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="77bbb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="77bbb-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="77bbb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="77bbb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="77bbb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="77bbb-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="77bbb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="77bbb-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="77bbb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="77bbb-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="77bbb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="77bbb-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="77bbb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="77bbb-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77bbb-163">createdDateTime</span></span>|<span data-ttu-id="77bbb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77bbb-164">DateTimeOffset</span></span>|<span data-ttu-id="77bbb-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="77bbb-165">DateTime the object was created.</span></span> <span data-ttu-id="77bbb-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-167">description</span><span class="sxs-lookup"><span data-stu-id="77bbb-167">description</span></span>|<span data-ttu-id="77bbb-168">String</span><span class="sxs-lookup"><span data-stu-id="77bbb-168">String</span></span>|<span data-ttu-id="77bbb-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="77bbb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77bbb-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="77bbb-171">displayName</span></span>|<span data-ttu-id="77bbb-172">String</span><span class="sxs-lookup"><span data-stu-id="77bbb-172">String</span></span>|<span data-ttu-id="77bbb-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="77bbb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77bbb-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-175">version</span><span class="sxs-lookup"><span data-stu-id="77bbb-175">version</span></span>|<span data-ttu-id="77bbb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="77bbb-176">Int32</span></span>|<span data-ttu-id="77bbb-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="77bbb-177">Version of the device configuration.</span></span> <span data-ttu-id="77bbb-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77bbb-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77bbb-179">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="77bbb-179">teacherCertificateSettings</span></span>|[<span data-ttu-id="77bbb-180">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="77bbb-180">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="77bbb-181">教師の信頼されたルートと PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="77bbb-181">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="77bbb-182">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="77bbb-182">studentCertificateSettings</span></span>|[<span data-ttu-id="77bbb-183">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="77bbb-183">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="77bbb-184">学生の信頼できるルート証明書と PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="77bbb-184">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="77bbb-185">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="77bbb-185">deviceCertificateSettings</span></span>|[<span data-ttu-id="77bbb-186">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="77bbb-186">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="77bbb-187">デバイスの信頼されたルートと PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="77bbb-187">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="77bbb-188">応答</span><span class="sxs-lookup"><span data-stu-id="77bbb-188">Response</span></span>
<span data-ttu-id="77bbb-189">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77bbb-189">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77bbb-190">例</span><span class="sxs-lookup"><span data-stu-id="77bbb-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="77bbb-191">要求</span><span class="sxs-lookup"><span data-stu-id="77bbb-191">Request</span></span>
<span data-ttu-id="77bbb-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77bbb-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2683

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
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
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```

### <a name="response"></a><span data-ttu-id="77bbb-193">応答</span><span class="sxs-lookup"><span data-stu-id="77bbb-193">Response</span></span>
<span data-ttu-id="77bbb-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77bbb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2855

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
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
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```





