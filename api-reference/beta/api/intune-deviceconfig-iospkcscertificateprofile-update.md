---
title: iospkcscertificateprofile の更新
description: iospkcscertificateprofile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c33d5beb2220ae9c60027ebb5cd0ecbc1b19a6ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174665"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="9cb05-103">iospkcscertificateprofile の更新</span><span class="sxs-lookup"><span data-stu-id="9cb05-103">Update iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="9cb05-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cb05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cb05-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9cb05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cb05-106">[iospkcscertificateprofile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9cb05-106">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cb05-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9cb05-107">Prerequisites</span></span>
<span data-ttu-id="9cb05-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cb05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9cb05-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9cb05-110">Permission type</span></span>|<span data-ttu-id="9cb05-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9cb05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cb05-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9cb05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9cb05-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cb05-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cb05-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9cb05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cb05-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cb05-115">Not supported.</span></span>|
|<span data-ttu-id="9cb05-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9cb05-116">Application</span></span>|<span data-ttu-id="9cb05-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cb05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cb05-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9cb05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9cb05-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9cb05-119">Request headers</span></span>
|<span data-ttu-id="9cb05-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9cb05-120">Header</span></span>|<span data-ttu-id="9cb05-121">値</span><span class="sxs-lookup"><span data-stu-id="9cb05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cb05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb05-122">Authorization</span></span>|<span data-ttu-id="9cb05-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9cb05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cb05-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9cb05-124">Accept</span></span>|<span data-ttu-id="9cb05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9cb05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cb05-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9cb05-126">Request body</span></span>
<span data-ttu-id="9cb05-127">要求本文で、 [iospkcscertificateprofile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9cb05-127">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="9cb05-128">次の表に、 [iospkcscertificateprofile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9cb05-128">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="9cb05-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cb05-129">Property</span></span>|<span data-ttu-id="9cb05-130">型</span><span class="sxs-lookup"><span data-stu-id="9cb05-130">Type</span></span>|<span data-ttu-id="9cb05-131">説明</span><span class="sxs-lookup"><span data-stu-id="9cb05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cb05-132">id</span><span class="sxs-lookup"><span data-stu-id="9cb05-132">id</span></span>|<span data-ttu-id="9cb05-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9cb05-133">String</span></span>|<span data-ttu-id="9cb05-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9cb05-134">Key of the entity.</span></span> <span data-ttu-id="9cb05-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cb05-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cb05-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9cb05-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cb05-137">DateTimeOffset</span></span>|<span data-ttu-id="9cb05-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9cb05-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9cb05-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cb05-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9cb05-140">roleScopeTagIds</span></span>|<span data-ttu-id="9cb05-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9cb05-141">String collection</span></span>|<span data-ttu-id="9cb05-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9cb05-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9cb05-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cb05-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9cb05-144">supportsScopeTags</span></span>|<span data-ttu-id="9cb05-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="9cb05-145">Boolean</span></span>|<span data-ttu-id="9cb05-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9cb05-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9cb05-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9cb05-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9cb05-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9cb05-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9cb05-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9cb05-149">This property is read-only.</span></span> <span data-ttu-id="9cb05-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cb05-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9cb05-151">createdDateTime</span></span>|<span data-ttu-id="9cb05-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cb05-152">DateTimeOffset</span></span>|<span data-ttu-id="9cb05-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9cb05-153">DateTime the object was created.</span></span> <span data-ttu-id="9cb05-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cb05-155">説明</span><span class="sxs-lookup"><span data-stu-id="9cb05-155">description</span></span>|<span data-ttu-id="9cb05-156">String</span><span class="sxs-lookup"><span data-stu-id="9cb05-156">String</span></span>|<span data-ttu-id="9cb05-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9cb05-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9cb05-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cb05-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9cb05-159">displayName</span></span>|<span data-ttu-id="9cb05-160">String</span><span class="sxs-lookup"><span data-stu-id="9cb05-160">String</span></span>|<span data-ttu-id="9cb05-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9cb05-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9cb05-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cb05-163">version</span><span class="sxs-lookup"><span data-stu-id="9cb05-163">version</span></span>|<span data-ttu-id="9cb05-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9cb05-164">Int32</span></span>|<span data-ttu-id="9cb05-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9cb05-165">Version of the device configuration.</span></span> <span data-ttu-id="9cb05-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cb05-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9cb05-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="9cb05-168">Int32</span><span class="sxs-lookup"><span data-stu-id="9cb05-168">Int32</span></span>|<span data-ttu-id="9cb05-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="9cb05-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9cb05-170">有効な値は、 [ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承された値 1 ~ 99 です。</span><span class="sxs-lookup"><span data-stu-id="9cb05-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9cb05-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9cb05-171">subjectNameFormat</span></span>|[<span data-ttu-id="9cb05-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9cb05-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="9cb05-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="9cb05-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="9cb05-174">[ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9cb05-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="9cb05-175">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="9cb05-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="9cb05-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9cb05-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9cb05-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9cb05-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9cb05-178">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="9cb05-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="9cb05-179">[ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9cb05-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="9cb05-180">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="9cb05-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9cb05-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9cb05-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9cb05-182">Int32</span><span class="sxs-lookup"><span data-stu-id="9cb05-182">Int32</span></span>|<span data-ttu-id="9cb05-183">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="9cb05-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="9cb05-184">[ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="9cb05-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9cb05-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9cb05-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9cb05-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9cb05-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9cb05-187">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="9cb05-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9cb05-188">[ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9cb05-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="9cb05-189">可能な値は `days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="9cb05-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9cb05-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="9cb05-190">certificationAuthority</span></span>|<span data-ttu-id="9cb05-191">String</span><span class="sxs-lookup"><span data-stu-id="9cb05-191">String</span></span>|<span data-ttu-id="9cb05-192">PKCS 証明機関。</span><span class="sxs-lookup"><span data-stu-id="9cb05-192">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="9cb05-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="9cb05-193">certificationAuthorityName</span></span>|<span data-ttu-id="9cb05-194">String</span><span class="sxs-lookup"><span data-stu-id="9cb05-194">String</span></span>|<span data-ttu-id="9cb05-195">PKCS 証明機関名。</span><span class="sxs-lookup"><span data-stu-id="9cb05-195">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="9cb05-196">certificatetemplatename</span><span class="sxs-lookup"><span data-stu-id="9cb05-196">certificateTemplateName</span></span>|<span data-ttu-id="9cb05-197">String</span><span class="sxs-lookup"><span data-stu-id="9cb05-197">String</span></span>|<span data-ttu-id="9cb05-198">PKCS 証明書テンプレート名。</span><span class="sxs-lookup"><span data-stu-id="9cb05-198">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="9cb05-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9cb05-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="9cb05-200">String</span><span class="sxs-lookup"><span data-stu-id="9cb05-200">String</span></span>|<span data-ttu-id="9cb05-201">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="9cb05-201">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="9cb05-202">応答</span><span class="sxs-lookup"><span data-stu-id="9cb05-202">Response</span></span>
<span data-ttu-id="9cb05-203">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[iospkcscertificateprofile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9cb05-203">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cb05-204">例</span><span class="sxs-lookup"><span data-stu-id="9cb05-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cb05-205">要求</span><span class="sxs-lookup"><span data-stu-id="9cb05-205">Request</span></span>
<span data-ttu-id="9cb05-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9cb05-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 761

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="9cb05-207">応答</span><span class="sxs-lookup"><span data-stu-id="9cb05-207">Response</span></span>
<span data-ttu-id="9cb05-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9cb05-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




