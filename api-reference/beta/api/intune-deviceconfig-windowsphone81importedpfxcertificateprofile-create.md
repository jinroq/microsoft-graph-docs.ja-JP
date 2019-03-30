---
title: windowsPhone81ImportedPFXCertificateProfile を作成する
description: 新しい windowsPhone81ImportedPFXCertificateProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75e083e531b5647146b09f49d0bcafe8a5802817
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966048"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="1a567-103">windowsPhone81ImportedPFXCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="1a567-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="1a567-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a567-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a567-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a567-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a567-106">新しい[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1a567-106">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a567-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a567-107">Prerequisites</span></span>
<span data-ttu-id="1a567-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a567-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a567-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a567-110">Permission type</span></span>|<span data-ttu-id="1a567-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a567-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a567-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a567-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a567-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a567-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a567-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a567-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a567-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a567-115">Not supported.</span></span>|
|<span data-ttu-id="1a567-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a567-116">Application</span></span>|<span data-ttu-id="1a567-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a567-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a567-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a567-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1a567-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a567-119">Request headers</span></span>
|<span data-ttu-id="1a567-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a567-120">Header</span></span>|<span data-ttu-id="1a567-121">値</span><span class="sxs-lookup"><span data-stu-id="1a567-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a567-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a567-122">Authorization</span></span>|<span data-ttu-id="1a567-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a567-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a567-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1a567-124">Accept</span></span>|<span data-ttu-id="1a567-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a567-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a567-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a567-126">Request body</span></span>
<span data-ttu-id="1a567-127">要求本文で、windowsPhone81ImportedPFXCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a567-127">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="1a567-128">次の表に、windowsPhone81ImportedPFXCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1a567-128">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="1a567-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a567-129">Property</span></span>|<span data-ttu-id="1a567-130">型</span><span class="sxs-lookup"><span data-stu-id="1a567-130">Type</span></span>|<span data-ttu-id="1a567-131">説明</span><span class="sxs-lookup"><span data-stu-id="1a567-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a567-132">id</span><span class="sxs-lookup"><span data-stu-id="1a567-132">id</span></span>|<span data-ttu-id="1a567-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1a567-133">String</span></span>|<span data-ttu-id="1a567-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1a567-134">Key of the entity.</span></span> <span data-ttu-id="1a567-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a567-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a567-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a567-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1a567-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a567-137">DateTimeOffset</span></span>|<span data-ttu-id="1a567-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a567-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1a567-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a567-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a567-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a567-140">roleScopeTagIds</span></span>|<span data-ttu-id="1a567-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1a567-141">String collection</span></span>|<span data-ttu-id="1a567-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="1a567-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a567-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a567-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a567-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a567-144">supportsScopeTags</span></span>|<span data-ttu-id="1a567-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a567-145">Boolean</span></span>|<span data-ttu-id="1a567-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1a567-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a567-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="1a567-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a567-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="1a567-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a567-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="1a567-149">This property is read-only.</span></span> <span data-ttu-id="1a567-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a567-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a567-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a567-151">createdDateTime</span></span>|<span data-ttu-id="1a567-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a567-152">DateTimeOffset</span></span>|<span data-ttu-id="1a567-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a567-153">DateTime the object was created.</span></span> <span data-ttu-id="1a567-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a567-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a567-155">description</span><span class="sxs-lookup"><span data-stu-id="1a567-155">description</span></span>|<span data-ttu-id="1a567-156">String</span><span class="sxs-lookup"><span data-stu-id="1a567-156">String</span></span>|<span data-ttu-id="1a567-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="1a567-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a567-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a567-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a567-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1a567-159">displayName</span></span>|<span data-ttu-id="1a567-160">String</span><span class="sxs-lookup"><span data-stu-id="1a567-160">String</span></span>|<span data-ttu-id="1a567-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="1a567-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a567-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a567-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a567-163">version</span><span class="sxs-lookup"><span data-stu-id="1a567-163">version</span></span>|<span data-ttu-id="1a567-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1a567-164">Int32</span></span>|<span data-ttu-id="1a567-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1a567-165">Version of the device configuration.</span></span> <span data-ttu-id="1a567-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a567-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a567-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1a567-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="1a567-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1a567-168">Int32</span></span>|<span data-ttu-id="1a567-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="1a567-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1a567-170">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="1a567-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1a567-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="1a567-171">keyStorageProvider</span></span>|[<span data-ttu-id="1a567-172">keystorageprovideroption</span><span class="sxs-lookup"><span data-stu-id="1a567-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="1a567-173">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承したキー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="1a567-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="1a567-174">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="1a567-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="1a567-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1a567-175">subjectNameFormat</span></span>|[<span data-ttu-id="1a567-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1a567-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="1a567-177">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される証明書のサブジェクト名形式。</span><span class="sxs-lookup"><span data-stu-id="1a567-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="1a567-178">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="1a567-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="1a567-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1a567-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1a567-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1a567-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="1a567-181">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書のサブジェクトの別名型。</span><span class="sxs-lookup"><span data-stu-id="1a567-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="1a567-182">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="1a567-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="1a567-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1a567-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1a567-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1a567-184">Int32</span></span>|<span data-ttu-id="1a567-185">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間の値</span><span class="sxs-lookup"><span data-stu-id="1a567-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1a567-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1a567-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1a567-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1a567-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1a567-188">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="1a567-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="1a567-189">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="1a567-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="1a567-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1a567-190">intendedPurpose</span></span>|[<span data-ttu-id="1a567-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1a567-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="1a567-192">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="1a567-192">Not yet documented.</span></span> <span data-ttu-id="1a567-193">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="1a567-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="1a567-194">応答</span><span class="sxs-lookup"><span data-stu-id="1a567-194">Response</span></span>
<span data-ttu-id="1a567-195">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1a567-195">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a567-196">例</span><span class="sxs-lookup"><span data-stu-id="1a567-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a567-197">要求</span><span class="sxs-lookup"><span data-stu-id="1a567-197">Request</span></span>
<span data-ttu-id="1a567-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a567-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="1a567-199">応答</span><span class="sxs-lookup"><span data-stu-id="1a567-199">Response</span></span>
<span data-ttu-id="1a567-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a567-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 763

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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




