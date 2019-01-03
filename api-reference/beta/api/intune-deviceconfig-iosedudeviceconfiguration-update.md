---
title: IosEduDeviceConfiguration を更新します。
description: IosEduDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: afeb9c6a93a3af2d64f59e2613e86462a2914158
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307582"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="4faef-103">IosEduDeviceConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="4faef-103">Update iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="4faef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4faef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4faef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4faef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4faef-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4faef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4faef-107">[IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4faef-107">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4faef-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4faef-108">Prerequisites</span></span>
<span data-ttu-id="4faef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4faef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4faef-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4faef-111">Permission type</span></span>|<span data-ttu-id="4faef-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4faef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4faef-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4faef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4faef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4faef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4faef-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4faef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4faef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4faef-116">Not supported.</span></span>|
|<span data-ttu-id="4faef-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4faef-117">Application</span></span>|<span data-ttu-id="4faef-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4faef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4faef-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4faef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4faef-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4faef-120">Request headers</span></span>
|<span data-ttu-id="4faef-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4faef-121">Header</span></span>|<span data-ttu-id="4faef-122">値</span><span class="sxs-lookup"><span data-stu-id="4faef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4faef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4faef-123">Authorization</span></span>|<span data-ttu-id="4faef-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4faef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4faef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4faef-125">Accept</span></span>|<span data-ttu-id="4faef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4faef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4faef-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4faef-127">Request body</span></span>
<span data-ttu-id="4faef-128">要求の本文に[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4faef-128">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="4faef-129">[IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="4faef-129">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="4faef-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4faef-130">Property</span></span>|<span data-ttu-id="4faef-131">種類</span><span class="sxs-lookup"><span data-stu-id="4faef-131">Type</span></span>|<span data-ttu-id="4faef-132">説明</span><span class="sxs-lookup"><span data-stu-id="4faef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4faef-133">ID</span><span class="sxs-lookup"><span data-stu-id="4faef-133">id</span></span>|<span data-ttu-id="4faef-134">String</span><span class="sxs-lookup"><span data-stu-id="4faef-134">String</span></span>|<span data-ttu-id="4faef-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4faef-135">Key of the entity.</span></span> <span data-ttu-id="4faef-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4faef-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4faef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4faef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4faef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4faef-138">DateTimeOffset</span></span>|<span data-ttu-id="4faef-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4faef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4faef-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4faef-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4faef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4faef-141">roleScopeTagIds</span></span>|<span data-ttu-id="4faef-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4faef-142">String collection</span></span>|<span data-ttu-id="4faef-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="4faef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4faef-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4faef-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4faef-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4faef-145">supportsScopeTags</span></span>|<span data-ttu-id="4faef-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="4faef-146">Boolean</span></span>|<span data-ttu-id="4faef-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4faef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4faef-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="4faef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4faef-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="4faef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4faef-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="4faef-150">This property is read-only.</span></span> <span data-ttu-id="4faef-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4faef-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4faef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4faef-152">createdDateTime</span></span>|<span data-ttu-id="4faef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4faef-153">DateTimeOffset</span></span>|<span data-ttu-id="4faef-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4faef-154">DateTime the object was created.</span></span> <span data-ttu-id="4faef-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4faef-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4faef-156">説明</span><span class="sxs-lookup"><span data-stu-id="4faef-156">description</span></span>|<span data-ttu-id="4faef-157">String</span><span class="sxs-lookup"><span data-stu-id="4faef-157">String</span></span>|<span data-ttu-id="4faef-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="4faef-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4faef-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4faef-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4faef-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4faef-160">displayName</span></span>|<span data-ttu-id="4faef-161">String</span><span class="sxs-lookup"><span data-stu-id="4faef-161">String</span></span>|<span data-ttu-id="4faef-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="4faef-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4faef-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4faef-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4faef-164">version</span><span class="sxs-lookup"><span data-stu-id="4faef-164">version</span></span>|<span data-ttu-id="4faef-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4faef-165">Int32</span></span>|<span data-ttu-id="4faef-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4faef-166">Version of the device configuration.</span></span> <span data-ttu-id="4faef-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4faef-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4faef-168">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="4faef-168">teacherCertificateSettings</span></span>|[<span data-ttu-id="4faef-169">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="4faef-169">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="4faef-170">教師の証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="4faef-170">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="4faef-171">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="4faef-171">studentCertificateSettings</span></span>|[<span data-ttu-id="4faef-172">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="4faef-172">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="4faef-173">受講者用の証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="4faef-173">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="4faef-174">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="4faef-174">deviceCertificateSettings</span></span>|[<span data-ttu-id="4faef-175">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="4faef-175">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="4faef-176">デバイスの証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="4faef-176">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="4faef-177">応答</span><span class="sxs-lookup"><span data-stu-id="4faef-177">Response</span></span>
<span data-ttu-id="4faef-178">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4faef-178">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4faef-179">例</span><span class="sxs-lookup"><span data-stu-id="4faef-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="4faef-180">要求</span><span class="sxs-lookup"><span data-stu-id="4faef-180">Request</span></span>
<span data-ttu-id="4faef-181">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4faef-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1910

{
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

### <a name="response"></a><span data-ttu-id="4faef-182">応答</span><span class="sxs-lookup"><span data-stu-id="4faef-182">Response</span></span>
<span data-ttu-id="4faef-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4faef-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




