---
title: iosedudeviceconfiguration 作成する
description: 新しい iosedudeviceconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02a54274513700202ff4c59d43fe8758882bb751
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173746"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="742fd-103">iosedudeviceconfiguration 作成する</span><span class="sxs-lookup"><span data-stu-id="742fd-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="742fd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="742fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="742fd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="742fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="742fd-106">新しい[iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="742fd-106">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="742fd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="742fd-107">Prerequisites</span></span>
<span data-ttu-id="742fd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="742fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="742fd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="742fd-110">Permission type</span></span>|<span data-ttu-id="742fd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="742fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="742fd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="742fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="742fd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="742fd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="742fd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="742fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="742fd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="742fd-115">Not supported.</span></span>|
|<span data-ttu-id="742fd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="742fd-116">Application</span></span>|<span data-ttu-id="742fd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="742fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="742fd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="742fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="742fd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="742fd-119">Request headers</span></span>
|<span data-ttu-id="742fd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="742fd-120">Header</span></span>|<span data-ttu-id="742fd-121">値</span><span class="sxs-lookup"><span data-stu-id="742fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="742fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="742fd-122">Authorization</span></span>|<span data-ttu-id="742fd-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="742fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="742fd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="742fd-124">Accept</span></span>|<span data-ttu-id="742fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="742fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="742fd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="742fd-126">Request body</span></span>
<span data-ttu-id="742fd-127">要求本文で、iosedudeviceconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="742fd-127">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="742fd-128">次の表に、iosedudeviceconfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="742fd-128">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="742fd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="742fd-129">Property</span></span>|<span data-ttu-id="742fd-130">型</span><span class="sxs-lookup"><span data-stu-id="742fd-130">Type</span></span>|<span data-ttu-id="742fd-131">説明</span><span class="sxs-lookup"><span data-stu-id="742fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="742fd-132">id</span><span class="sxs-lookup"><span data-stu-id="742fd-132">id</span></span>|<span data-ttu-id="742fd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="742fd-133">String</span></span>|<span data-ttu-id="742fd-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="742fd-134">Key of the entity.</span></span> <span data-ttu-id="742fd-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="742fd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="742fd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="742fd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="742fd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="742fd-137">DateTimeOffset</span></span>|<span data-ttu-id="742fd-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="742fd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="742fd-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="742fd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="742fd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="742fd-140">roleScopeTagIds</span></span>|<span data-ttu-id="742fd-141">String collection</span><span class="sxs-lookup"><span data-stu-id="742fd-141">String collection</span></span>|<span data-ttu-id="742fd-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="742fd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="742fd-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="742fd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="742fd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="742fd-144">supportsScopeTags</span></span>|<span data-ttu-id="742fd-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="742fd-145">Boolean</span></span>|<span data-ttu-id="742fd-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="742fd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="742fd-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="742fd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="742fd-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="742fd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="742fd-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="742fd-149">This property is read-only.</span></span> <span data-ttu-id="742fd-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="742fd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="742fd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="742fd-151">createdDateTime</span></span>|<span data-ttu-id="742fd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="742fd-152">DateTimeOffset</span></span>|<span data-ttu-id="742fd-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="742fd-153">DateTime the object was created.</span></span> <span data-ttu-id="742fd-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="742fd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="742fd-155">説明</span><span class="sxs-lookup"><span data-stu-id="742fd-155">description</span></span>|<span data-ttu-id="742fd-156">String</span><span class="sxs-lookup"><span data-stu-id="742fd-156">String</span></span>|<span data-ttu-id="742fd-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="742fd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="742fd-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="742fd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="742fd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="742fd-159">displayName</span></span>|<span data-ttu-id="742fd-160">String</span><span class="sxs-lookup"><span data-stu-id="742fd-160">String</span></span>|<span data-ttu-id="742fd-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="742fd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="742fd-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="742fd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="742fd-163">version</span><span class="sxs-lookup"><span data-stu-id="742fd-163">version</span></span>|<span data-ttu-id="742fd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="742fd-164">Int32</span></span>|<span data-ttu-id="742fd-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="742fd-165">Version of the device configuration.</span></span> <span data-ttu-id="742fd-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="742fd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="742fd-167">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="742fd-167">teacherCertificateSettings</span></span>|[<span data-ttu-id="742fd-168">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="742fd-168">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="742fd-169">教師の信頼されたルートと PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="742fd-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="742fd-170">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="742fd-170">studentCertificateSettings</span></span>|[<span data-ttu-id="742fd-171">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="742fd-171">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="742fd-172">学生の信頼できるルート証明書と PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="742fd-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="742fd-173">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="742fd-173">deviceCertificateSettings</span></span>|[<span data-ttu-id="742fd-174">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="742fd-174">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="742fd-175">デバイスの信頼されたルートと PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="742fd-175">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="742fd-176">応答</span><span class="sxs-lookup"><span data-stu-id="742fd-176">Response</span></span>
<span data-ttu-id="742fd-177">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="742fd-177">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="742fd-178">例</span><span class="sxs-lookup"><span data-stu-id="742fd-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="742fd-179">要求</span><span class="sxs-lookup"><span data-stu-id="742fd-179">Request</span></span>
<span data-ttu-id="742fd-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="742fd-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="742fd-181">応答</span><span class="sxs-lookup"><span data-stu-id="742fd-181">Response</span></span>
<span data-ttu-id="742fd-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="742fd-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




