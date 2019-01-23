---
title: Windows10PkcsCertificateProfile を更新します。
description: Windows10PkcsCertificateProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c2eee04b80356bd4f49a0eb6281472e2b37ad591
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400355"
---
# <a name="update-windows10pkcscertificateprofile"></a><span data-ttu-id="18b53-103">Windows10PkcsCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="18b53-103">Update windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="18b53-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18b53-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18b53-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18b53-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18b53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18b53-107">[Windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="18b53-107">Update the properties of a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18b53-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="18b53-108">Prerequisites</span></span>
<span data-ttu-id="18b53-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18b53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18b53-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18b53-111">Permission type</span></span>|<span data-ttu-id="18b53-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18b53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18b53-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18b53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18b53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18b53-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18b53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18b53-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b53-116">Not supported.</span></span>|
|<span data-ttu-id="18b53-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18b53-117">Application</span></span>|<span data-ttu-id="18b53-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b53-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18b53-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18b53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="18b53-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18b53-120">Request headers</span></span>
|<span data-ttu-id="18b53-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18b53-121">Header</span></span>|<span data-ttu-id="18b53-122">値</span><span class="sxs-lookup"><span data-stu-id="18b53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18b53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b53-123">Authorization</span></span>|<span data-ttu-id="18b53-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="18b53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18b53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18b53-125">Accept</span></span>|<span data-ttu-id="18b53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18b53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18b53-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="18b53-127">Request body</span></span>
<span data-ttu-id="18b53-128">要求の本文に[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="18b53-128">In the request body, supply a JSON representation for the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="18b53-129">[Windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="18b53-129">The following table shows the properties that are required when you create the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span></span>

|<span data-ttu-id="18b53-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18b53-130">Property</span></span>|<span data-ttu-id="18b53-131">型</span><span class="sxs-lookup"><span data-stu-id="18b53-131">Type</span></span>|<span data-ttu-id="18b53-132">説明</span><span class="sxs-lookup"><span data-stu-id="18b53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b53-133">id</span><span class="sxs-lookup"><span data-stu-id="18b53-133">id</span></span>|<span data-ttu-id="18b53-134">String</span><span class="sxs-lookup"><span data-stu-id="18b53-134">String</span></span>|<span data-ttu-id="18b53-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="18b53-135">Key of the entity.</span></span> <span data-ttu-id="18b53-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18b53-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b53-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18b53-137">lastModifiedDateTime</span></span>|<span data-ttu-id="18b53-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18b53-138">DateTimeOffset</span></span>|<span data-ttu-id="18b53-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="18b53-139">DateTime the object was last modified.</span></span> <span data-ttu-id="18b53-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18b53-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b53-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18b53-141">roleScopeTagIds</span></span>|<span data-ttu-id="18b53-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="18b53-142">String collection</span></span>|<span data-ttu-id="18b53-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="18b53-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18b53-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18b53-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b53-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="18b53-145">supportsScopeTags</span></span>|<span data-ttu-id="18b53-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="18b53-146">Boolean</span></span>|<span data-ttu-id="18b53-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18b53-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="18b53-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="18b53-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="18b53-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="18b53-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="18b53-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="18b53-150">This property is read-only.</span></span> <span data-ttu-id="18b53-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18b53-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b53-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18b53-152">createdDateTime</span></span>|<span data-ttu-id="18b53-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18b53-153">DateTimeOffset</span></span>|<span data-ttu-id="18b53-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="18b53-154">DateTime the object was created.</span></span> <span data-ttu-id="18b53-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18b53-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b53-156">説明</span><span class="sxs-lookup"><span data-stu-id="18b53-156">description</span></span>|<span data-ttu-id="18b53-157">String</span><span class="sxs-lookup"><span data-stu-id="18b53-157">String</span></span>|<span data-ttu-id="18b53-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="18b53-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18b53-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18b53-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b53-160">displayName</span><span class="sxs-lookup"><span data-stu-id="18b53-160">displayName</span></span>|<span data-ttu-id="18b53-161">String</span><span class="sxs-lookup"><span data-stu-id="18b53-161">String</span></span>|<span data-ttu-id="18b53-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="18b53-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18b53-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18b53-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b53-164">version</span><span class="sxs-lookup"><span data-stu-id="18b53-164">version</span></span>|<span data-ttu-id="18b53-165">Int32</span><span class="sxs-lookup"><span data-stu-id="18b53-165">Int32</span></span>|<span data-ttu-id="18b53-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="18b53-166">Version of the device configuration.</span></span> <span data-ttu-id="18b53-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18b53-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b53-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="18b53-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="18b53-169">Int32</span><span class="sxs-lookup"><span data-stu-id="18b53-169">Int32</span></span>|<span data-ttu-id="18b53-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="18b53-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="18b53-171">有効な値は[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="18b53-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="18b53-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="18b53-172">keyStorageProvider</span></span>|[<span data-ttu-id="18b53-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="18b53-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="18b53-174">[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)からキー記憶域プロバイダー (KSP) 継承します。</span><span class="sxs-lookup"><span data-stu-id="18b53-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="18b53-175">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="18b53-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="18b53-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="18b53-176">subjectNameFormat</span></span>|[<span data-ttu-id="18b53-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="18b53-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="18b53-178">証明書サブジェクト名の形式から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)です。</span><span class="sxs-lookup"><span data-stu-id="18b53-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="18b53-179">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="18b53-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="18b53-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="18b53-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="18b53-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="18b53-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="18b53-182">証明書サブジェクト代替名タイプから継承[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="18b53-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="18b53-183">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="18b53-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="18b53-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="18b53-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="18b53-185">Int32</span><span class="sxs-lookup"><span data-stu-id="18b53-185">Int32</span></span>|<span data-ttu-id="18b53-186">証明書有効期間から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)の値</span><span class="sxs-lookup"><span data-stu-id="18b53-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="18b53-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="18b53-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="18b53-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="18b53-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="18b53-189">証明書有効期間から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)のスケールです。</span><span class="sxs-lookup"><span data-stu-id="18b53-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="18b53-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="18b53-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="18b53-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="18b53-191">certificationAuthority</span></span>|<span data-ttu-id="18b53-192">String</span><span class="sxs-lookup"><span data-stu-id="18b53-192">String</span></span>|<span data-ttu-id="18b53-193">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="18b53-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="18b53-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="18b53-194">certificationAuthorityName</span></span>|<span data-ttu-id="18b53-195">String</span><span class="sxs-lookup"><span data-stu-id="18b53-195">String</span></span>|<span data-ttu-id="18b53-196">PKCS 証明機関の名前</span><span class="sxs-lookup"><span data-stu-id="18b53-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="18b53-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="18b53-197">certificateTemplateName</span></span>|<span data-ttu-id="18b53-198">String</span><span class="sxs-lookup"><span data-stu-id="18b53-198">String</span></span>|<span data-ttu-id="18b53-199">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="18b53-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="18b53-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="18b53-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="18b53-201">String</span><span class="sxs-lookup"><span data-stu-id="18b53-201">String</span></span>|<span data-ttu-id="18b53-202">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="18b53-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="18b53-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="18b53-203">extendedKeyUsages</span></span>|<span data-ttu-id="18b53-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18b53-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="18b53-205">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="18b53-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="18b53-206">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="18b53-206">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="18b53-207">応答</span><span class="sxs-lookup"><span data-stu-id="18b53-207">Response</span></span>
<span data-ttu-id="18b53-208">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="18b53-208">If successful, this method returns a `200 OK` response code and an updated [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b53-209">例</span><span class="sxs-lookup"><span data-stu-id="18b53-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="18b53-210">要求</span><span class="sxs-lookup"><span data-stu-id="18b53-210">Request</span></span>
<span data-ttu-id="18b53-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18b53-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18b53-212">応答</span><span class="sxs-lookup"><span data-stu-id="18b53-212">Response</span></span>
<span data-ttu-id="18b53-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18b53-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




