---
title: IosEduDeviceConfiguration を作成します。
description: 新しい iosEduDeviceConfiguration オブジェクトを作成します。
ms.openlocfilehash: 51aad445c40e89be6033a6444d375cd354d19c28
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072559"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="6d906-103">IosEduDeviceConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="6d906-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="6d906-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6d906-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d906-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d906-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d906-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d906-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d906-107">新しい[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d906-107">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d906-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6d906-108">Prerequisites</span></span>
<span data-ttu-id="6d906-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d906-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d906-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d906-111">Permission type</span></span>|<span data-ttu-id="6d906-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d906-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d906-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d906-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d906-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d906-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d906-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d906-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d906-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d906-116">Not supported.</span></span>|
|<span data-ttu-id="6d906-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d906-117">Application</span></span>|<span data-ttu-id="6d906-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d906-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d906-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d906-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6d906-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d906-120">Request headers</span></span>
|<span data-ttu-id="6d906-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d906-121">Header</span></span>|<span data-ttu-id="6d906-122">値</span><span class="sxs-lookup"><span data-stu-id="6d906-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d906-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d906-123">Authorization</span></span>|<span data-ttu-id="6d906-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6d906-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d906-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d906-125">Accept</span></span>|<span data-ttu-id="6d906-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d906-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d906-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d906-127">Request body</span></span>
<span data-ttu-id="6d906-128">要求の本文に iosEduDeviceConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="6d906-128">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="6d906-129">次の表は、iosEduDeviceConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6d906-129">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="6d906-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d906-130">Property</span></span>|<span data-ttu-id="6d906-131">型</span><span class="sxs-lookup"><span data-stu-id="6d906-131">Type</span></span>|<span data-ttu-id="6d906-132">説明</span><span class="sxs-lookup"><span data-stu-id="6d906-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d906-133">id</span><span class="sxs-lookup"><span data-stu-id="6d906-133">id</span></span>|<span data-ttu-id="6d906-134">String</span><span class="sxs-lookup"><span data-stu-id="6d906-134">String</span></span>|<span data-ttu-id="6d906-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6d906-135">Key of the entity.</span></span> <span data-ttu-id="6d906-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6d906-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d906-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d906-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6d906-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d906-138">DateTimeOffset</span></span>|<span data-ttu-id="6d906-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6d906-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6d906-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6d906-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d906-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6d906-141">roleScopeTagIds</span></span>|<span data-ttu-id="6d906-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6d906-142">String collection</span></span>|<span data-ttu-id="6d906-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="6d906-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6d906-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6d906-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d906-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6d906-145">supportsScopeTags</span></span>|<span data-ttu-id="6d906-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="6d906-146">Boolean</span></span>|<span data-ttu-id="6d906-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6d906-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6d906-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="6d906-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6d906-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="6d906-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6d906-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6d906-150">This property is read-only.</span></span> <span data-ttu-id="6d906-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6d906-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d906-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d906-152">createdDateTime</span></span>|<span data-ttu-id="6d906-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d906-153">DateTimeOffset</span></span>|<span data-ttu-id="6d906-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6d906-154">DateTime the object was created.</span></span> <span data-ttu-id="6d906-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6d906-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d906-156">説明</span><span class="sxs-lookup"><span data-stu-id="6d906-156">description</span></span>|<span data-ttu-id="6d906-157">String</span><span class="sxs-lookup"><span data-stu-id="6d906-157">String</span></span>|<span data-ttu-id="6d906-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6d906-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6d906-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6d906-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d906-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6d906-160">displayName</span></span>|<span data-ttu-id="6d906-161">String</span><span class="sxs-lookup"><span data-stu-id="6d906-161">String</span></span>|<span data-ttu-id="6d906-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6d906-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6d906-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6d906-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d906-164">version</span><span class="sxs-lookup"><span data-stu-id="6d906-164">version</span></span>|<span data-ttu-id="6d906-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6d906-165">Int32</span></span>|<span data-ttu-id="6d906-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6d906-166">Version of the device configuration.</span></span> <span data-ttu-id="6d906-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6d906-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d906-168">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6d906-168">teacherCertificateSettings</span></span>|[<span data-ttu-id="6d906-169">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6d906-169">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="6d906-170">教師の証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="6d906-170">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="6d906-171">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6d906-171">studentCertificateSettings</span></span>|[<span data-ttu-id="6d906-172">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6d906-172">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="6d906-173">受講者用の証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="6d906-173">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="6d906-174">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6d906-174">deviceCertificateSettings</span></span>|[<span data-ttu-id="6d906-175">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6d906-175">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="6d906-176">デバイスの証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="6d906-176">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="6d906-177">応答</span><span class="sxs-lookup"><span data-stu-id="6d906-177">Response</span></span>
<span data-ttu-id="6d906-178">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6d906-178">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d906-179">例</span><span class="sxs-lookup"><span data-stu-id="6d906-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d906-180">要求</span><span class="sxs-lookup"><span data-stu-id="6d906-180">Request</span></span>
<span data-ttu-id="6d906-181">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6d906-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1974

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="6d906-182">応答</span><span class="sxs-lookup"><span data-stu-id="6d906-182">Response</span></span>
<span data-ttu-id="6d906-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6d906-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





