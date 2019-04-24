---
title: windows10PkcsCertificateProfile の更新
description: windows10PkcsCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c9689c811619de4ad514e32e7411c9711a33aa6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32515807"
---
# <a name="update-windows10pkcscertificateprofile"></a><span data-ttu-id="4d6c6-103">windows10PkcsCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="4d6c6-103">Update windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="4d6c6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d6c6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d6c6-106">[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-106">Update the properties of a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d6c6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4d6c6-107">Prerequisites</span></span>
<span data-ttu-id="4d6c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d6c6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d6c6-110">Permission type</span></span>|<span data-ttu-id="4d6c6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d6c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d6c6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d6c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d6c6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d6c6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d6c6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d6c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d6c6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-115">Not supported.</span></span>|
|<span data-ttu-id="4d6c6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d6c6-116">Application</span></span>|<span data-ttu-id="4d6c6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d6c6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d6c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4d6c6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d6c6-119">Request headers</span></span>
|<span data-ttu-id="4d6c6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d6c6-120">Header</span></span>|<span data-ttu-id="4d6c6-121">値</span><span class="sxs-lookup"><span data-stu-id="4d6c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d6c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d6c6-122">Authorization</span></span>|<span data-ttu-id="4d6c6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d6c6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4d6c6-124">Accept</span></span>|<span data-ttu-id="4d6c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d6c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d6c6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d6c6-126">Request body</span></span>
<span data-ttu-id="4d6c6-127">要求本文で、 [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-127">In the request body, supply a JSON representation for the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="4d6c6-128">次の表に、 [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-128">The following table shows the properties that are required when you create the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span></span>

|<span data-ttu-id="4d6c6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d6c6-129">Property</span></span>|<span data-ttu-id="4d6c6-130">型</span><span class="sxs-lookup"><span data-stu-id="4d6c6-130">Type</span></span>|<span data-ttu-id="4d6c6-131">説明</span><span class="sxs-lookup"><span data-stu-id="4d6c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d6c6-132">id</span><span class="sxs-lookup"><span data-stu-id="4d6c6-132">id</span></span>|<span data-ttu-id="4d6c6-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4d6c6-133">String</span></span>|<span data-ttu-id="4d6c6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-134">Key of the entity.</span></span> <span data-ttu-id="4d6c6-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4d6c6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d6c6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d6c6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4d6c6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d6c6-137">DateTimeOffset</span></span>|<span data-ttu-id="4d6c6-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4d6c6-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4d6c6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d6c6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4d6c6-140">roleScopeTagIds</span></span>|<span data-ttu-id="4d6c6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4d6c6-141">String collection</span></span>|<span data-ttu-id="4d6c6-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4d6c6-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4d6c6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d6c6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4d6c6-144">supportsScopeTags</span></span>|<span data-ttu-id="4d6c6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d6c6-145">Boolean</span></span>|<span data-ttu-id="4d6c6-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4d6c6-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4d6c6-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4d6c6-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-149">This property is read-only.</span></span> <span data-ttu-id="4d6c6-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4d6c6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d6c6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d6c6-151">createdDateTime</span></span>|<span data-ttu-id="4d6c6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d6c6-152">DateTimeOffset</span></span>|<span data-ttu-id="4d6c6-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-153">DateTime the object was created.</span></span> <span data-ttu-id="4d6c6-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4d6c6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d6c6-155">説明</span><span class="sxs-lookup"><span data-stu-id="4d6c6-155">description</span></span>|<span data-ttu-id="4d6c6-156">String</span><span class="sxs-lookup"><span data-stu-id="4d6c6-156">String</span></span>|<span data-ttu-id="4d6c6-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4d6c6-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4d6c6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d6c6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4d6c6-159">displayName</span></span>|<span data-ttu-id="4d6c6-160">String</span><span class="sxs-lookup"><span data-stu-id="4d6c6-160">String</span></span>|<span data-ttu-id="4d6c6-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4d6c6-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4d6c6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d6c6-163">version</span><span class="sxs-lookup"><span data-stu-id="4d6c6-163">version</span></span>|<span data-ttu-id="4d6c6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6c6-164">Int32</span></span>|<span data-ttu-id="4d6c6-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-165">Version of the device configuration.</span></span> <span data-ttu-id="4d6c6-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4d6c6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d6c6-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="4d6c6-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="4d6c6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6c6-168">Int32</span></span>|<span data-ttu-id="4d6c6-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="4d6c6-170">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4d6c6-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="4d6c6-171">keyStorageProvider</span></span>|[<span data-ttu-id="4d6c6-172">keystorageprovideroption</span><span class="sxs-lookup"><span data-stu-id="4d6c6-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="4d6c6-173">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承したキー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="4d6c6-174">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="4d6c6-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4d6c6-175">subjectNameFormat</span></span>|[<span data-ttu-id="4d6c6-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4d6c6-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="4d6c6-177">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される証明書のサブジェクト名形式。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="4d6c6-178">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="4d6c6-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4d6c6-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="4d6c6-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4d6c6-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="4d6c6-181">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書のサブジェクトの別名型。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="4d6c6-182">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="4d6c6-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="4d6c6-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="4d6c6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6c6-184">Int32</span></span>|<span data-ttu-id="4d6c6-185">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間の値</span><span class="sxs-lookup"><span data-stu-id="4d6c6-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4d6c6-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4d6c6-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="4d6c6-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4d6c6-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="4d6c6-188">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="4d6c6-189">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="4d6c6-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="4d6c6-190">certificationAuthority</span></span>|<span data-ttu-id="4d6c6-191">String</span><span class="sxs-lookup"><span data-stu-id="4d6c6-191">String</span></span>|<span data-ttu-id="4d6c6-192">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="4d6c6-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="4d6c6-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="4d6c6-193">certificationAuthorityName</span></span>|<span data-ttu-id="4d6c6-194">String</span><span class="sxs-lookup"><span data-stu-id="4d6c6-194">String</span></span>|<span data-ttu-id="4d6c6-195">PKCS 証明機関名</span><span class="sxs-lookup"><span data-stu-id="4d6c6-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="4d6c6-196">certificatetemplatename</span><span class="sxs-lookup"><span data-stu-id="4d6c6-196">certificateTemplateName</span></span>|<span data-ttu-id="4d6c6-197">String</span><span class="sxs-lookup"><span data-stu-id="4d6c6-197">String</span></span>|<span data-ttu-id="4d6c6-198">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="4d6c6-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="4d6c6-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4d6c6-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="4d6c6-200">String</span><span class="sxs-lookup"><span data-stu-id="4d6c6-200">String</span></span>|<span data-ttu-id="4d6c6-201">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="4d6c6-202">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="4d6c6-202">extendedKeyUsages</span></span>|<span data-ttu-id="4d6c6-203">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4d6c6-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="4d6c6-204">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="4d6c6-205">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4d6c6-206">応答</span><span class="sxs-lookup"><span data-stu-id="4d6c6-206">Response</span></span>
<span data-ttu-id="4d6c6-207">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-207">If successful, this method returns a `200 OK` response code and an updated [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d6c6-208">例</span><span class="sxs-lookup"><span data-stu-id="4d6c6-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d6c6-209">要求</span><span class="sxs-lookup"><span data-stu-id="4d6c6-209">Request</span></span>
<span data-ttu-id="4d6c6-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1011

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4d6c6-211">応答</span><span class="sxs-lookup"><span data-stu-id="4d6c6-211">Response</span></span>
<span data-ttu-id="4d6c6-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d6c6-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1183

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```





