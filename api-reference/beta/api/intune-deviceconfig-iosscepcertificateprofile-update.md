---
title: IosScepCertificateProfile を更新します。
description: IosScepCertificateProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c7ac67a81dab6faca9724c9cf7eec17d4920414d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396498"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="f23be-103">IosScepCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="f23be-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="f23be-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f23be-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f23be-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f23be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f23be-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f23be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f23be-107">[IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f23be-107">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f23be-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f23be-108">Prerequisites</span></span>
<span data-ttu-id="f23be-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f23be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f23be-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f23be-111">Permission type</span></span>|<span data-ttu-id="f23be-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f23be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f23be-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f23be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f23be-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23be-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f23be-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f23be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f23be-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f23be-116">Not supported.</span></span>|
|<span data-ttu-id="f23be-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f23be-117">Application</span></span>|<span data-ttu-id="f23be-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f23be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f23be-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f23be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f23be-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f23be-120">Request headers</span></span>
|<span data-ttu-id="f23be-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f23be-121">Header</span></span>|<span data-ttu-id="f23be-122">値</span><span class="sxs-lookup"><span data-stu-id="f23be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f23be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f23be-123">Authorization</span></span>|<span data-ttu-id="f23be-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f23be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f23be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f23be-125">Accept</span></span>|<span data-ttu-id="f23be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f23be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f23be-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f23be-127">Request body</span></span>
<span data-ttu-id="f23be-128">要求の本文に[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f23be-128">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="f23be-129">[IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f23be-129">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="f23be-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f23be-130">Property</span></span>|<span data-ttu-id="f23be-131">型</span><span class="sxs-lookup"><span data-stu-id="f23be-131">Type</span></span>|<span data-ttu-id="f23be-132">説明</span><span class="sxs-lookup"><span data-stu-id="f23be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23be-133">id</span><span class="sxs-lookup"><span data-stu-id="f23be-133">id</span></span>|<span data-ttu-id="f23be-134">String</span><span class="sxs-lookup"><span data-stu-id="f23be-134">String</span></span>|<span data-ttu-id="f23be-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f23be-135">Key of the entity.</span></span> <span data-ttu-id="f23be-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23be-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23be-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f23be-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f23be-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23be-138">DateTimeOffset</span></span>|<span data-ttu-id="f23be-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f23be-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f23be-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23be-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23be-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f23be-141">roleScopeTagIds</span></span>|<span data-ttu-id="f23be-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f23be-142">String collection</span></span>|<span data-ttu-id="f23be-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="f23be-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f23be-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23be-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23be-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f23be-145">supportsScopeTags</span></span>|<span data-ttu-id="f23be-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f23be-146">Boolean</span></span>|<span data-ttu-id="f23be-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f23be-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f23be-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="f23be-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f23be-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="f23be-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f23be-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f23be-150">This property is read-only.</span></span> <span data-ttu-id="f23be-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23be-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23be-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f23be-152">createdDateTime</span></span>|<span data-ttu-id="f23be-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23be-153">DateTimeOffset</span></span>|<span data-ttu-id="f23be-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f23be-154">DateTime the object was created.</span></span> <span data-ttu-id="f23be-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23be-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23be-156">説明</span><span class="sxs-lookup"><span data-stu-id="f23be-156">description</span></span>|<span data-ttu-id="f23be-157">String</span><span class="sxs-lookup"><span data-stu-id="f23be-157">String</span></span>|<span data-ttu-id="f23be-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f23be-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f23be-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23be-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23be-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f23be-160">displayName</span></span>|<span data-ttu-id="f23be-161">String</span><span class="sxs-lookup"><span data-stu-id="f23be-161">String</span></span>|<span data-ttu-id="f23be-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f23be-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f23be-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23be-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23be-164">version</span><span class="sxs-lookup"><span data-stu-id="f23be-164">version</span></span>|<span data-ttu-id="f23be-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f23be-165">Int32</span></span>|<span data-ttu-id="f23be-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f23be-166">Version of the device configuration.</span></span> <span data-ttu-id="f23be-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23be-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23be-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f23be-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="f23be-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f23be-169">Int32</span></span>|<span data-ttu-id="f23be-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="f23be-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f23be-171">有効な値は[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="f23be-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f23be-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f23be-172">subjectNameFormat</span></span>|[<span data-ttu-id="f23be-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f23be-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="f23be-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="f23be-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="f23be-175">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f23be-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f23be-176">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="f23be-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="f23be-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f23be-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f23be-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f23be-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f23be-179">証明書のサブジェクトの別名の種類です。</span><span class="sxs-lookup"><span data-stu-id="f23be-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="f23be-180">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f23be-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f23be-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="f23be-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f23be-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f23be-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f23be-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f23be-183">Int32</span></span>|<span data-ttu-id="f23be-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="f23be-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f23be-185">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="f23be-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f23be-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f23be-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f23be-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f23be-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f23be-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="f23be-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f23be-189">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f23be-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f23be-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="f23be-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f23be-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f23be-191">scepServerUrls</span></span>|<span data-ttu-id="f23be-192">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f23be-192">String collection</span></span>|<span data-ttu-id="f23be-193">SCEP サーバー個の url。</span><span class="sxs-lookup"><span data-stu-id="f23be-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f23be-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f23be-194">subjectNameFormatString</span></span>|<span data-ttu-id="f23be-195">String</span><span class="sxs-lookup"><span data-stu-id="f23be-195">String</span></span>|<span data-ttu-id="f23be-196">SubjectNameFormat で使用するカスタム書式指定 = カスタムです。</span><span class="sxs-lookup"><span data-stu-id="f23be-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f23be-197">例: CN = EmailAddress {{}}、E = EmailAddress {{}}、OU = エンタープライズ ユーザーの場合は、O = コントソ株式会社、L = Redmond、ST = ワシントン州 C = u. s.</span><span class="sxs-lookup"><span data-stu-id="f23be-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f23be-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="f23be-198">keyUsage</span></span>|[<span data-ttu-id="f23be-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="f23be-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f23be-200">SCEP のキー使用法です。</span><span class="sxs-lookup"><span data-stu-id="f23be-200">SCEP Key Usage.</span></span> <span data-ttu-id="f23be-201">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="f23be-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f23be-202">キー長</span><span class="sxs-lookup"><span data-stu-id="f23be-202">keySize</span></span>|[<span data-ttu-id="f23be-203">キー長</span><span class="sxs-lookup"><span data-stu-id="f23be-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f23be-204">SCEP のキー サイズ。</span><span class="sxs-lookup"><span data-stu-id="f23be-204">SCEP Key Size.</span></span> <span data-ttu-id="f23be-205">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="f23be-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f23be-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f23be-206">extendedKeyUsages</span></span>|<span data-ttu-id="f23be-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f23be-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f23be-208">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="f23be-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f23be-209">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f23be-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f23be-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f23be-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f23be-211">String</span><span class="sxs-lookup"><span data-stu-id="f23be-211">String</span></span>|<span data-ttu-id="f23be-212">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="f23be-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f23be-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f23be-213">certificateStore</span></span>|[<span data-ttu-id="f23be-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f23be-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f23be-215">ターゲット ストアの証明書です。</span><span class="sxs-lookup"><span data-stu-id="f23be-215">Target store certificate.</span></span> <span data-ttu-id="f23be-216">使用可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="f23be-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f23be-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f23be-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f23be-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f23be-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f23be-219">Alterantive 名の設定をカスタムの件名です。</span><span class="sxs-lookup"><span data-stu-id="f23be-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="f23be-220">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f23be-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f23be-221">応答</span><span class="sxs-lookup"><span data-stu-id="f23be-221">Response</span></span>
<span data-ttu-id="f23be-222">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f23be-222">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23be-223">例</span><span class="sxs-lookup"><span data-stu-id="f23be-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="f23be-224">要求</span><span class="sxs-lookup"><span data-stu-id="f23be-224">Request</span></span>
<span data-ttu-id="f23be-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f23be-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f23be-226">応答</span><span class="sxs-lookup"><span data-stu-id="f23be-226">Response</span></span>
<span data-ttu-id="f23be-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f23be-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```




