---
title: macOSImportedPFXCertificateProfile を作成する
description: 新しい macOSImportedPFXCertificateProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 78a7a35d1632edd9e9c7576ef5707100b5017224
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147538"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="da2b8-103">macOSImportedPFXCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="da2b8-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="da2b8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da2b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da2b8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da2b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da2b8-106">新しい[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="da2b8-106">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da2b8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="da2b8-107">Prerequisites</span></span>
<span data-ttu-id="da2b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="da2b8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da2b8-110">Permission type</span></span>|<span data-ttu-id="da2b8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="da2b8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da2b8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da2b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da2b8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2b8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da2b8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da2b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da2b8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da2b8-115">Not supported.</span></span>|
|<span data-ttu-id="da2b8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da2b8-116">Application</span></span>|<span data-ttu-id="da2b8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da2b8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da2b8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da2b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="da2b8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da2b8-119">Request headers</span></span>
|<span data-ttu-id="da2b8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da2b8-120">Header</span></span>|<span data-ttu-id="da2b8-121">値</span><span class="sxs-lookup"><span data-stu-id="da2b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da2b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da2b8-122">Authorization</span></span>|<span data-ttu-id="da2b8-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="da2b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da2b8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="da2b8-124">Accept</span></span>|<span data-ttu-id="da2b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da2b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da2b8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="da2b8-126">Request body</span></span>
<span data-ttu-id="da2b8-127">要求本文で、macOSImportedPFXCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="da2b8-127">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="da2b8-128">次の表に、macOSImportedPFXCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="da2b8-128">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="da2b8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da2b8-129">Property</span></span>|<span data-ttu-id="da2b8-130">型</span><span class="sxs-lookup"><span data-stu-id="da2b8-130">Type</span></span>|<span data-ttu-id="da2b8-131">説明</span><span class="sxs-lookup"><span data-stu-id="da2b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da2b8-132">id</span><span class="sxs-lookup"><span data-stu-id="da2b8-132">id</span></span>|<span data-ttu-id="da2b8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="da2b8-133">String</span></span>|<span data-ttu-id="da2b8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="da2b8-134">Key of the entity.</span></span> <span data-ttu-id="da2b8-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da2b8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da2b8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="da2b8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da2b8-137">DateTimeOffset</span></span>|<span data-ttu-id="da2b8-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="da2b8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="da2b8-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da2b8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da2b8-140">roleScopeTagIds</span></span>|<span data-ttu-id="da2b8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="da2b8-141">String collection</span></span>|<span data-ttu-id="da2b8-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="da2b8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da2b8-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da2b8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da2b8-144">supportsScopeTags</span></span>|<span data-ttu-id="da2b8-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="da2b8-145">Boolean</span></span>|<span data-ttu-id="da2b8-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da2b8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da2b8-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="da2b8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da2b8-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="da2b8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da2b8-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="da2b8-149">This property is read-only.</span></span> <span data-ttu-id="da2b8-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da2b8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da2b8-151">createdDateTime</span></span>|<span data-ttu-id="da2b8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da2b8-152">DateTimeOffset</span></span>|<span data-ttu-id="da2b8-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="da2b8-153">DateTime the object was created.</span></span> <span data-ttu-id="da2b8-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da2b8-155">説明</span><span class="sxs-lookup"><span data-stu-id="da2b8-155">description</span></span>|<span data-ttu-id="da2b8-156">String</span><span class="sxs-lookup"><span data-stu-id="da2b8-156">String</span></span>|<span data-ttu-id="da2b8-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="da2b8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da2b8-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da2b8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="da2b8-159">displayName</span></span>|<span data-ttu-id="da2b8-160">String</span><span class="sxs-lookup"><span data-stu-id="da2b8-160">String</span></span>|<span data-ttu-id="da2b8-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="da2b8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da2b8-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da2b8-163">version</span><span class="sxs-lookup"><span data-stu-id="da2b8-163">version</span></span>|<span data-ttu-id="da2b8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="da2b8-164">Int32</span></span>|<span data-ttu-id="da2b8-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="da2b8-165">Version of the device configuration.</span></span> <span data-ttu-id="da2b8-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da2b8-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="da2b8-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="da2b8-168">Int32</span><span class="sxs-lookup"><span data-stu-id="da2b8-168">Int32</span></span>|<span data-ttu-id="da2b8-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="da2b8-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="da2b8-170">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="da2b8-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="da2b8-171">subjectNameFormat</span></span>|[<span data-ttu-id="da2b8-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="da2b8-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="da2b8-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="da2b8-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="da2b8-174">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="da2b8-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="da2b8-175">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="da2b8-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="da2b8-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="da2b8-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="da2b8-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="da2b8-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="da2b8-178">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="da2b8-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="da2b8-179">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="da2b8-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="da2b8-180">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="da2b8-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="da2b8-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="da2b8-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="da2b8-182">Int32</span><span class="sxs-lookup"><span data-stu-id="da2b8-182">Int32</span></span>|<span data-ttu-id="da2b8-183">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="da2b8-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="da2b8-184">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="da2b8-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="da2b8-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="da2b8-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="da2b8-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="da2b8-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="da2b8-187">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="da2b8-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="da2b8-188">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="da2b8-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="da2b8-189">可能な値は `days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="da2b8-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="da2b8-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="da2b8-190">intendedPurpose</span></span>|[<span data-ttu-id="da2b8-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="da2b8-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="da2b8-192">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="da2b8-192">Not yet documented.</span></span> <span data-ttu-id="da2b8-193">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="da2b8-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="da2b8-194">応答</span><span class="sxs-lookup"><span data-stu-id="da2b8-194">Response</span></span>
<span data-ttu-id="da2b8-195">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="da2b8-195">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da2b8-196">例</span><span class="sxs-lookup"><span data-stu-id="da2b8-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="da2b8-197">要求</span><span class="sxs-lookup"><span data-stu-id="da2b8-197">Request</span></span>
<span data-ttu-id="da2b8-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da2b8-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="da2b8-199">応答</span><span class="sxs-lookup"><span data-stu-id="da2b8-199">Response</span></span>
<span data-ttu-id="da2b8-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="da2b8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




