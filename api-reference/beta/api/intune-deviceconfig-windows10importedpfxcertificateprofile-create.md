---
title: windows10ImportedPFXCertificateProfile を作成する
description: 新しい windows10ImportedPFXCertificateProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a986e258e0d0b61bf178c27a3a14e30743d8d312
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145340"
---
# <a name="create-windows10importedpfxcertificateprofile"></a><span data-ttu-id="535d3-103">windows10ImportedPFXCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="535d3-103">Create windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="535d3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="535d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="535d3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="535d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="535d3-106">新しい[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="535d3-106">Create a new [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="535d3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="535d3-107">Prerequisites</span></span>
<span data-ttu-id="535d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="535d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="535d3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="535d3-110">Permission type</span></span>|<span data-ttu-id="535d3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="535d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="535d3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="535d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="535d3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535d3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="535d3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="535d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="535d3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="535d3-115">Not supported.</span></span>|
|<span data-ttu-id="535d3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="535d3-116">Application</span></span>|<span data-ttu-id="535d3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="535d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="535d3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="535d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="535d3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="535d3-119">Request headers</span></span>
|<span data-ttu-id="535d3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="535d3-120">Header</span></span>|<span data-ttu-id="535d3-121">値</span><span class="sxs-lookup"><span data-stu-id="535d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="535d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="535d3-122">Authorization</span></span>|<span data-ttu-id="535d3-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="535d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="535d3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="535d3-124">Accept</span></span>|<span data-ttu-id="535d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="535d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="535d3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="535d3-126">Request body</span></span>
<span data-ttu-id="535d3-127">要求本文で、windows10ImportedPFXCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="535d3-127">In the request body, supply a JSON representation for the windows10ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="535d3-128">次の表に、windows10ImportedPFXCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="535d3-128">The following table shows the properties that are required when you create the windows10ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="535d3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="535d3-129">Property</span></span>|<span data-ttu-id="535d3-130">型</span><span class="sxs-lookup"><span data-stu-id="535d3-130">Type</span></span>|<span data-ttu-id="535d3-131">説明</span><span class="sxs-lookup"><span data-stu-id="535d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="535d3-132">id</span><span class="sxs-lookup"><span data-stu-id="535d3-132">id</span></span>|<span data-ttu-id="535d3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="535d3-133">String</span></span>|<span data-ttu-id="535d3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="535d3-134">Key of the entity.</span></span> <span data-ttu-id="535d3-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="535d3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="535d3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="535d3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="535d3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="535d3-137">DateTimeOffset</span></span>|<span data-ttu-id="535d3-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="535d3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="535d3-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="535d3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="535d3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="535d3-140">roleScopeTagIds</span></span>|<span data-ttu-id="535d3-141">String collection</span><span class="sxs-lookup"><span data-stu-id="535d3-141">String collection</span></span>|<span data-ttu-id="535d3-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="535d3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="535d3-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="535d3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="535d3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="535d3-144">supportsScopeTags</span></span>|<span data-ttu-id="535d3-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="535d3-145">Boolean</span></span>|<span data-ttu-id="535d3-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="535d3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="535d3-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="535d3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="535d3-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="535d3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="535d3-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="535d3-149">This property is read-only.</span></span> <span data-ttu-id="535d3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="535d3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="535d3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="535d3-151">createdDateTime</span></span>|<span data-ttu-id="535d3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="535d3-152">DateTimeOffset</span></span>|<span data-ttu-id="535d3-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="535d3-153">DateTime the object was created.</span></span> <span data-ttu-id="535d3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="535d3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="535d3-155">説明</span><span class="sxs-lookup"><span data-stu-id="535d3-155">description</span></span>|<span data-ttu-id="535d3-156">String</span><span class="sxs-lookup"><span data-stu-id="535d3-156">String</span></span>|<span data-ttu-id="535d3-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="535d3-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="535d3-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="535d3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="535d3-159">displayName</span><span class="sxs-lookup"><span data-stu-id="535d3-159">displayName</span></span>|<span data-ttu-id="535d3-160">String</span><span class="sxs-lookup"><span data-stu-id="535d3-160">String</span></span>|<span data-ttu-id="535d3-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="535d3-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="535d3-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="535d3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="535d3-163">version</span><span class="sxs-lookup"><span data-stu-id="535d3-163">version</span></span>|<span data-ttu-id="535d3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="535d3-164">Int32</span></span>|<span data-ttu-id="535d3-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="535d3-165">Version of the device configuration.</span></span> <span data-ttu-id="535d3-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="535d3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="535d3-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="535d3-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="535d3-168">Int32</span><span class="sxs-lookup"><span data-stu-id="535d3-168">Int32</span></span>|<span data-ttu-id="535d3-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="535d3-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="535d3-170">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="535d3-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="535d3-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="535d3-171">keyStorageProvider</span></span>|[<span data-ttu-id="535d3-172">keystorageprovideroption</span><span class="sxs-lookup"><span data-stu-id="535d3-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="535d3-173">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承したキー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="535d3-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="535d3-174">使用可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="535d3-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="535d3-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="535d3-175">subjectNameFormat</span></span>|[<span data-ttu-id="535d3-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="535d3-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="535d3-177">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される証明書のサブジェクト名形式。</span><span class="sxs-lookup"><span data-stu-id="535d3-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="535d3-178">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="535d3-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="535d3-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="535d3-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="535d3-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="535d3-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="535d3-181">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書のサブジェクトの別名型。</span><span class="sxs-lookup"><span data-stu-id="535d3-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="535d3-182">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="535d3-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="535d3-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="535d3-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="535d3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="535d3-184">Int32</span></span>|<span data-ttu-id="535d3-185">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間の値</span><span class="sxs-lookup"><span data-stu-id="535d3-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="535d3-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="535d3-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="535d3-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="535d3-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="535d3-188">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="535d3-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="535d3-189">可能な値は `days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="535d3-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="535d3-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="535d3-190">intendedPurpose</span></span>|[<span data-ttu-id="535d3-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="535d3-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="535d3-192">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="535d3-192">Not yet documented.</span></span> <span data-ttu-id="535d3-193">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="535d3-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="535d3-194">応答</span><span class="sxs-lookup"><span data-stu-id="535d3-194">Response</span></span>
<span data-ttu-id="535d3-195">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="535d3-195">If successful, this method returns a `201 Created` response code and a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="535d3-196">例</span><span class="sxs-lookup"><span data-stu-id="535d3-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="535d3-197">要求</span><span class="sxs-lookup"><span data-stu-id="535d3-197">Request</span></span>
<span data-ttu-id="535d3-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="535d3-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 586

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="535d3-199">応答</span><span class="sxs-lookup"><span data-stu-id="535d3-199">Response</span></span>
<span data-ttu-id="535d3-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="535d3-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 758

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```




