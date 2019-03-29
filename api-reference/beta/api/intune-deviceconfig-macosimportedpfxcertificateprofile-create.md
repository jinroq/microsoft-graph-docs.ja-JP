---
title: macOSImportedPFXCertificateProfile を作成する
description: 新しい macOSImportedPFXCertificateProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 646ab2bf10a296563b87692499f6f3b069da56a9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957767"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="5225f-103">macOSImportedPFXCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="5225f-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="5225f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5225f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5225f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5225f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5225f-106">新しい[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5225f-106">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5225f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5225f-107">Prerequisites</span></span>
<span data-ttu-id="5225f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5225f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5225f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5225f-110">Permission type</span></span>|<span data-ttu-id="5225f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5225f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5225f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5225f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5225f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5225f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5225f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5225f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5225f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5225f-115">Not supported.</span></span>|
|<span data-ttu-id="5225f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5225f-116">Application</span></span>|<span data-ttu-id="5225f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5225f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5225f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5225f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5225f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5225f-119">Request headers</span></span>
|<span data-ttu-id="5225f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5225f-120">Header</span></span>|<span data-ttu-id="5225f-121">値</span><span class="sxs-lookup"><span data-stu-id="5225f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5225f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5225f-122">Authorization</span></span>|<span data-ttu-id="5225f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5225f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5225f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5225f-124">Accept</span></span>|<span data-ttu-id="5225f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5225f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5225f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5225f-126">Request body</span></span>
<span data-ttu-id="5225f-127">要求本文で、macOSImportedPFXCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5225f-127">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="5225f-128">次の表に、macOSImportedPFXCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5225f-128">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="5225f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5225f-129">Property</span></span>|<span data-ttu-id="5225f-130">型</span><span class="sxs-lookup"><span data-stu-id="5225f-130">Type</span></span>|<span data-ttu-id="5225f-131">説明</span><span class="sxs-lookup"><span data-stu-id="5225f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5225f-132">id</span><span class="sxs-lookup"><span data-stu-id="5225f-132">id</span></span>|<span data-ttu-id="5225f-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5225f-133">String</span></span>|<span data-ttu-id="5225f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5225f-134">Key of the entity.</span></span> <span data-ttu-id="5225f-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5225f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5225f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5225f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5225f-137">DateTimeOffset</span></span>|<span data-ttu-id="5225f-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="5225f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5225f-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5225f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5225f-140">roleScopeTagIds</span></span>|<span data-ttu-id="5225f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5225f-141">String collection</span></span>|<span data-ttu-id="5225f-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="5225f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5225f-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5225f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5225f-144">supportsScopeTags</span></span>|<span data-ttu-id="5225f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5225f-145">Boolean</span></span>|<span data-ttu-id="5225f-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5225f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5225f-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="5225f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5225f-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="5225f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5225f-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="5225f-149">This property is read-only.</span></span> <span data-ttu-id="5225f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5225f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5225f-151">createdDateTime</span></span>|<span data-ttu-id="5225f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5225f-152">DateTimeOffset</span></span>|<span data-ttu-id="5225f-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5225f-153">DateTime the object was created.</span></span> <span data-ttu-id="5225f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5225f-155">description</span><span class="sxs-lookup"><span data-stu-id="5225f-155">description</span></span>|<span data-ttu-id="5225f-156">String</span><span class="sxs-lookup"><span data-stu-id="5225f-156">String</span></span>|<span data-ttu-id="5225f-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="5225f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5225f-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5225f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5225f-159">displayName</span></span>|<span data-ttu-id="5225f-160">String</span><span class="sxs-lookup"><span data-stu-id="5225f-160">String</span></span>|<span data-ttu-id="5225f-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="5225f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5225f-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5225f-163">version</span><span class="sxs-lookup"><span data-stu-id="5225f-163">version</span></span>|<span data-ttu-id="5225f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5225f-164">Int32</span></span>|<span data-ttu-id="5225f-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5225f-165">Version of the device configuration.</span></span> <span data-ttu-id="5225f-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5225f-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5225f-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="5225f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5225f-168">Int32</span></span>|<span data-ttu-id="5225f-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="5225f-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5225f-170">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5225f-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5225f-171">subjectNameFormat</span></span>|[<span data-ttu-id="5225f-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5225f-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="5225f-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="5225f-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="5225f-174">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5225f-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5225f-175">可能な値は `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="5225f-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="5225f-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5225f-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5225f-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5225f-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5225f-178">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="5225f-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="5225f-179">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5225f-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5225f-180">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="5225f-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5225f-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5225f-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5225f-182">Int32</span><span class="sxs-lookup"><span data-stu-id="5225f-182">Int32</span></span>|<span data-ttu-id="5225f-183">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="5225f-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5225f-184">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="5225f-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5225f-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5225f-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5225f-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5225f-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5225f-187">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="5225f-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5225f-188">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5225f-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5225f-189">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="5225f-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5225f-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="5225f-190">intendedPurpose</span></span>|[<span data-ttu-id="5225f-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="5225f-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="5225f-192">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="5225f-192">Not yet documented.</span></span> <span data-ttu-id="5225f-193">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="5225f-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="5225f-194">応答</span><span class="sxs-lookup"><span data-stu-id="5225f-194">Response</span></span>
<span data-ttu-id="5225f-195">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5225f-195">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5225f-196">例</span><span class="sxs-lookup"><span data-stu-id="5225f-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="5225f-197">要求</span><span class="sxs-lookup"><span data-stu-id="5225f-197">Request</span></span>
<span data-ttu-id="5225f-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5225f-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="5225f-199">応答</span><span class="sxs-lookup"><span data-stu-id="5225f-199">Response</span></span>
<span data-ttu-id="5225f-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5225f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 696

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "intendedPurpose": "smimeEncryption"
}
```




