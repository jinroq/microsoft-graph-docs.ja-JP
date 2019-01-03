---
title: MacOSImportedPFXCertificateProfile を作成します。
description: 新しい macOSImportedPFXCertificateProfile オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 065817d209dd6c2b34fac23ca516d59250eb8cdf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338683"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="d5d97-103">MacOSImportedPFXCertificateProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5d97-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="d5d97-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5d97-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5d97-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5d97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5d97-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5d97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5d97-107">新しい[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d5d97-107">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5d97-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d5d97-108">Prerequisites</span></span>
<span data-ttu-id="d5d97-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5d97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5d97-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5d97-111">Permission type</span></span>|<span data-ttu-id="d5d97-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5d97-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5d97-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5d97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5d97-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d97-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5d97-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5d97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5d97-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5d97-116">Not supported.</span></span>|
|<span data-ttu-id="d5d97-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5d97-117">Application</span></span>|<span data-ttu-id="d5d97-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5d97-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5d97-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5d97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d5d97-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5d97-120">Request headers</span></span>
|<span data-ttu-id="d5d97-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5d97-121">Header</span></span>|<span data-ttu-id="d5d97-122">値</span><span class="sxs-lookup"><span data-stu-id="d5d97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5d97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5d97-123">Authorization</span></span>|<span data-ttu-id="d5d97-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d5d97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5d97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5d97-125">Accept</span></span>|<span data-ttu-id="d5d97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5d97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5d97-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5d97-127">Request body</span></span>
<span data-ttu-id="d5d97-128">要求の本文に macOSImportedPFXCertificateProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5d97-128">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="d5d97-129">次の表は、macOSImportedPFXCertificateProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d5d97-129">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="d5d97-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5d97-130">Property</span></span>|<span data-ttu-id="d5d97-131">種類</span><span class="sxs-lookup"><span data-stu-id="d5d97-131">Type</span></span>|<span data-ttu-id="d5d97-132">説明</span><span class="sxs-lookup"><span data-stu-id="d5d97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5d97-133">ID</span><span class="sxs-lookup"><span data-stu-id="d5d97-133">id</span></span>|<span data-ttu-id="d5d97-134">String</span><span class="sxs-lookup"><span data-stu-id="d5d97-134">String</span></span>|<span data-ttu-id="d5d97-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d5d97-135">Key of the entity.</span></span> <span data-ttu-id="d5d97-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5d97-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d97-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5d97-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d5d97-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5d97-138">DateTimeOffset</span></span>|<span data-ttu-id="d5d97-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d5d97-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d5d97-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5d97-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d97-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5d97-141">roleScopeTagIds</span></span>|<span data-ttu-id="d5d97-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d5d97-142">String collection</span></span>|<span data-ttu-id="d5d97-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="d5d97-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d5d97-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5d97-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d97-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d5d97-145">supportsScopeTags</span></span>|<span data-ttu-id="d5d97-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="d5d97-146">Boolean</span></span>|<span data-ttu-id="d5d97-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d5d97-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d5d97-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="d5d97-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d5d97-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="d5d97-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d5d97-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-150">This property is read-only.</span></span> <span data-ttu-id="d5d97-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5d97-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d97-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5d97-152">createdDateTime</span></span>|<span data-ttu-id="d5d97-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5d97-153">DateTimeOffset</span></span>|<span data-ttu-id="d5d97-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d5d97-154">DateTime the object was created.</span></span> <span data-ttu-id="d5d97-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5d97-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d97-156">説明</span><span class="sxs-lookup"><span data-stu-id="d5d97-156">description</span></span>|<span data-ttu-id="d5d97-157">String</span><span class="sxs-lookup"><span data-stu-id="d5d97-157">String</span></span>|<span data-ttu-id="d5d97-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d5d97-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5d97-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5d97-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d97-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d5d97-160">displayName</span></span>|<span data-ttu-id="d5d97-161">String</span><span class="sxs-lookup"><span data-stu-id="d5d97-161">String</span></span>|<span data-ttu-id="d5d97-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d5d97-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5d97-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5d97-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d97-164">version</span><span class="sxs-lookup"><span data-stu-id="d5d97-164">version</span></span>|<span data-ttu-id="d5d97-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d5d97-165">Int32</span></span>|<span data-ttu-id="d5d97-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d5d97-166">Version of the device configuration.</span></span> <span data-ttu-id="d5d97-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5d97-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d97-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d5d97-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="d5d97-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d5d97-169">Int32</span></span>|<span data-ttu-id="d5d97-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d5d97-171">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d5d97-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d5d97-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d5d97-172">subjectNameFormat</span></span>|[<span data-ttu-id="d5d97-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d5d97-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="d5d97-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="d5d97-175">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d5d97-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d5d97-176">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="d5d97-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="d5d97-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d5d97-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d5d97-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d5d97-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d5d97-179">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d5d97-180">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d5d97-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d5d97-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d5d97-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d5d97-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d5d97-183">Int32</span><span class="sxs-lookup"><span data-stu-id="d5d97-183">Int32</span></span>|<span data-ttu-id="d5d97-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d5d97-185">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d5d97-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d5d97-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d5d97-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d5d97-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d5d97-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d5d97-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="d5d97-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d5d97-189">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d5d97-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d5d97-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d5d97-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d5d97-191">intendedPurpose</span></span>|[<span data-ttu-id="d5d97-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d5d97-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d5d97-193">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="d5d97-193">Not yet documented.</span></span> <span data-ttu-id="d5d97-194">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d5d97-195">応答</span><span class="sxs-lookup"><span data-stu-id="d5d97-195">Response</span></span>
<span data-ttu-id="d5d97-196">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d5d97-196">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5d97-197">例</span><span class="sxs-lookup"><span data-stu-id="d5d97-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5d97-198">要求</span><span class="sxs-lookup"><span data-stu-id="d5d97-198">Request</span></span>
<span data-ttu-id="d5d97-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5d97-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="d5d97-200">応答</span><span class="sxs-lookup"><span data-stu-id="d5d97-200">Response</span></span>
<span data-ttu-id="d5d97-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5d97-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




