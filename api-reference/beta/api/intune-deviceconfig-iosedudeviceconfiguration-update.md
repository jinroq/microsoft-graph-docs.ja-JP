---
title: iosedudeviceconfiguration の更新
description: iosedudeviceconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f79818685efad4f26f26a3dfca9b687ae054ffa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972152"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="3a9c1-103">iosedudeviceconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="3a9c1-103">Update iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="3a9c1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a9c1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a9c1-106">[iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-106">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a9c1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3a9c1-107">Prerequisites</span></span>
<span data-ttu-id="3a9c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a9c1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a9c1-110">Permission type</span></span>|<span data-ttu-id="3a9c1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a9c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a9c1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a9c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a9c1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9c1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a9c1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a9c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a9c1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-115">Not supported.</span></span>|
|<span data-ttu-id="3a9c1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a9c1-116">Application</span></span>|<span data-ttu-id="3a9c1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a9c1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a9c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3a9c1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a9c1-119">Request headers</span></span>
|<span data-ttu-id="3a9c1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a9c1-120">Header</span></span>|<span data-ttu-id="3a9c1-121">値</span><span class="sxs-lookup"><span data-stu-id="3a9c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a9c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a9c1-122">Authorization</span></span>|<span data-ttu-id="3a9c1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a9c1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3a9c1-124">Accept</span></span>|<span data-ttu-id="3a9c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3a9c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a9c1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a9c1-126">Request body</span></span>
<span data-ttu-id="3a9c1-127">要求本文で、 [iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-127">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="3a9c1-128">次の表に、 [iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-128">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="3a9c1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a9c1-129">Property</span></span>|<span data-ttu-id="3a9c1-130">型</span><span class="sxs-lookup"><span data-stu-id="3a9c1-130">Type</span></span>|<span data-ttu-id="3a9c1-131">説明</span><span class="sxs-lookup"><span data-stu-id="3a9c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a9c1-132">id</span><span class="sxs-lookup"><span data-stu-id="3a9c1-132">id</span></span>|<span data-ttu-id="3a9c1-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3a9c1-133">String</span></span>|<span data-ttu-id="3a9c1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-134">Key of the entity.</span></span> <span data-ttu-id="3a9c1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3a9c1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9c1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a9c1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3a9c1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a9c1-137">DateTimeOffset</span></span>|<span data-ttu-id="3a9c1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3a9c1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3a9c1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9c1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a9c1-140">roleScopeTagIds</span></span>|<span data-ttu-id="3a9c1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3a9c1-141">String collection</span></span>|<span data-ttu-id="3a9c1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a9c1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3a9c1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9c1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3a9c1-144">supportsScopeTags</span></span>|<span data-ttu-id="3a9c1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a9c1-145">Boolean</span></span>|<span data-ttu-id="3a9c1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3a9c1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3a9c1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3a9c1-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-149">This property is read-only.</span></span> <span data-ttu-id="3a9c1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3a9c1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9c1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a9c1-151">createdDateTime</span></span>|<span data-ttu-id="3a9c1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a9c1-152">DateTimeOffset</span></span>|<span data-ttu-id="3a9c1-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-153">DateTime the object was created.</span></span> <span data-ttu-id="3a9c1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3a9c1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9c1-155">description</span><span class="sxs-lookup"><span data-stu-id="3a9c1-155">description</span></span>|<span data-ttu-id="3a9c1-156">String</span><span class="sxs-lookup"><span data-stu-id="3a9c1-156">String</span></span>|<span data-ttu-id="3a9c1-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3a9c1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3a9c1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9c1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3a9c1-159">displayName</span></span>|<span data-ttu-id="3a9c1-160">String</span><span class="sxs-lookup"><span data-stu-id="3a9c1-160">String</span></span>|<span data-ttu-id="3a9c1-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3a9c1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3a9c1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9c1-163">version</span><span class="sxs-lookup"><span data-stu-id="3a9c1-163">version</span></span>|<span data-ttu-id="3a9c1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3a9c1-164">Int32</span></span>|<span data-ttu-id="3a9c1-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-165">Version of the device configuration.</span></span> <span data-ttu-id="3a9c1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3a9c1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9c1-167">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="3a9c1-167">teacherCertificateSettings</span></span>|[<span data-ttu-id="3a9c1-168">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="3a9c1-168">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="3a9c1-169">教師の信頼されたルートと PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="3a9c1-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="3a9c1-170">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="3a9c1-170">studentCertificateSettings</span></span>|[<span data-ttu-id="3a9c1-171">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="3a9c1-171">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="3a9c1-172">学生の信頼できるルート証明書と PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="3a9c1-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="3a9c1-173">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="3a9c1-173">deviceCertificateSettings</span></span>|[<span data-ttu-id="3a9c1-174">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="3a9c1-174">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="3a9c1-175">デバイスの信頼されたルートと PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="3a9c1-175">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="3a9c1-176">応答</span><span class="sxs-lookup"><span data-stu-id="3a9c1-176">Response</span></span>
<span data-ttu-id="3a9c1-177">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)デバイスオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-177">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a9c1-178">例</span><span class="sxs-lookup"><span data-stu-id="3a9c1-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a9c1-179">要求</span><span class="sxs-lookup"><span data-stu-id="3a9c1-179">Request</span></span>
<span data-ttu-id="3a9c1-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1910

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="3a9c1-181">応答</span><span class="sxs-lookup"><span data-stu-id="3a9c1-181">Response</span></span>
<span data-ttu-id="3a9c1-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3a9c1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2082

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




