---
title: IosPkcsCertificateProfile を作成します。
description: 新しい iosPkcsCertificateProfile オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: dcfd75460e370d02dcb05c54a99685cfe148459d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305405"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="008d4-103">IosPkcsCertificateProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="008d4-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="008d4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="008d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="008d4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="008d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="008d4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="008d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="008d4-107">新しい[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="008d4-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="008d4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="008d4-108">Prerequisites</span></span>
<span data-ttu-id="008d4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="008d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="008d4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="008d4-111">Permission type</span></span>|<span data-ttu-id="008d4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="008d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="008d4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="008d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="008d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="008d4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="008d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="008d4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="008d4-116">Not supported.</span></span>|
|<span data-ttu-id="008d4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="008d4-117">Application</span></span>|<span data-ttu-id="008d4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="008d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="008d4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="008d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="008d4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="008d4-120">Request headers</span></span>
|<span data-ttu-id="008d4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="008d4-121">Header</span></span>|<span data-ttu-id="008d4-122">値</span><span class="sxs-lookup"><span data-stu-id="008d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="008d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="008d4-123">Authorization</span></span>|<span data-ttu-id="008d4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="008d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="008d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="008d4-125">Accept</span></span>|<span data-ttu-id="008d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="008d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="008d4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="008d4-127">Request body</span></span>
<span data-ttu-id="008d4-128">要求の本文に iosPkcsCertificateProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="008d4-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="008d4-129">次の表は、iosPkcsCertificateProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="008d4-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="008d4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="008d4-130">Property</span></span>|<span data-ttu-id="008d4-131">種類</span><span class="sxs-lookup"><span data-stu-id="008d4-131">Type</span></span>|<span data-ttu-id="008d4-132">説明</span><span class="sxs-lookup"><span data-stu-id="008d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="008d4-133">ID</span><span class="sxs-lookup"><span data-stu-id="008d4-133">id</span></span>|<span data-ttu-id="008d4-134">String</span><span class="sxs-lookup"><span data-stu-id="008d4-134">String</span></span>|<span data-ttu-id="008d4-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="008d4-135">Key of the entity.</span></span> <span data-ttu-id="008d4-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="008d4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="008d4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="008d4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="008d4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="008d4-138">DateTimeOffset</span></span>|<span data-ttu-id="008d4-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="008d4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="008d4-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="008d4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="008d4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="008d4-141">roleScopeTagIds</span></span>|<span data-ttu-id="008d4-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="008d4-142">String collection</span></span>|<span data-ttu-id="008d4-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="008d4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="008d4-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="008d4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="008d4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="008d4-145">supportsScopeTags</span></span>|<span data-ttu-id="008d4-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="008d4-146">Boolean</span></span>|<span data-ttu-id="008d4-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="008d4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="008d4-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="008d4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="008d4-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="008d4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="008d4-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="008d4-150">This property is read-only.</span></span> <span data-ttu-id="008d4-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="008d4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="008d4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="008d4-152">createdDateTime</span></span>|<span data-ttu-id="008d4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="008d4-153">DateTimeOffset</span></span>|<span data-ttu-id="008d4-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="008d4-154">DateTime the object was created.</span></span> <span data-ttu-id="008d4-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="008d4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="008d4-156">説明</span><span class="sxs-lookup"><span data-stu-id="008d4-156">description</span></span>|<span data-ttu-id="008d4-157">String</span><span class="sxs-lookup"><span data-stu-id="008d4-157">String</span></span>|<span data-ttu-id="008d4-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="008d4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="008d4-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="008d4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="008d4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="008d4-160">displayName</span></span>|<span data-ttu-id="008d4-161">String</span><span class="sxs-lookup"><span data-stu-id="008d4-161">String</span></span>|<span data-ttu-id="008d4-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="008d4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="008d4-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="008d4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="008d4-164">version</span><span class="sxs-lookup"><span data-stu-id="008d4-164">version</span></span>|<span data-ttu-id="008d4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="008d4-165">Int32</span></span>|<span data-ttu-id="008d4-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="008d4-166">Version of the device configuration.</span></span> <span data-ttu-id="008d4-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="008d4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="008d4-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="008d4-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="008d4-169">Int32</span><span class="sxs-lookup"><span data-stu-id="008d4-169">Int32</span></span>|<span data-ttu-id="008d4-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="008d4-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="008d4-171">有効な値は[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="008d4-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="008d4-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="008d4-172">subjectNameFormat</span></span>|[<span data-ttu-id="008d4-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="008d4-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="008d4-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="008d4-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="008d4-175">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="008d4-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="008d4-176">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="008d4-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="008d4-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="008d4-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="008d4-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="008d4-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="008d4-179">証明書のサブジェクトの別名の種類です。</span><span class="sxs-lookup"><span data-stu-id="008d4-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="008d4-180">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="008d4-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="008d4-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="008d4-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="008d4-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="008d4-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="008d4-183">Int32</span><span class="sxs-lookup"><span data-stu-id="008d4-183">Int32</span></span>|<span data-ttu-id="008d4-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="008d4-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="008d4-185">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="008d4-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="008d4-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="008d4-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="008d4-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="008d4-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="008d4-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="008d4-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="008d4-189">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="008d4-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="008d4-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="008d4-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="008d4-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="008d4-191">certificationAuthority</span></span>|<span data-ttu-id="008d4-192">String</span><span class="sxs-lookup"><span data-stu-id="008d4-192">String</span></span>|<span data-ttu-id="008d4-193">PKCS 証明機関。</span><span class="sxs-lookup"><span data-stu-id="008d4-193">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="008d4-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="008d4-194">certificationAuthorityName</span></span>|<span data-ttu-id="008d4-195">String</span><span class="sxs-lookup"><span data-stu-id="008d4-195">String</span></span>|<span data-ttu-id="008d4-196">PKCS 証明機関の名前です。</span><span class="sxs-lookup"><span data-stu-id="008d4-196">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="008d4-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="008d4-197">certificateTemplateName</span></span>|<span data-ttu-id="008d4-198">String</span><span class="sxs-lookup"><span data-stu-id="008d4-198">String</span></span>|<span data-ttu-id="008d4-199">PKCS の証明書テンプレートの名前です。</span><span class="sxs-lookup"><span data-stu-id="008d4-199">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="008d4-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="008d4-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="008d4-201">String</span><span class="sxs-lookup"><span data-stu-id="008d4-201">String</span></span>|<span data-ttu-id="008d4-202">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="008d4-202">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="008d4-203">応答</span><span class="sxs-lookup"><span data-stu-id="008d4-203">Response</span></span>
<span data-ttu-id="008d4-204">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="008d4-204">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="008d4-205">例</span><span class="sxs-lookup"><span data-stu-id="008d4-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="008d4-206">要求</span><span class="sxs-lookup"><span data-stu-id="008d4-206">Request</span></span>
<span data-ttu-id="008d4-207">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="008d4-207">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 825

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="008d4-208">応答</span><span class="sxs-lookup"><span data-stu-id="008d4-208">Response</span></span>
<span data-ttu-id="008d4-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="008d4-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 933

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




