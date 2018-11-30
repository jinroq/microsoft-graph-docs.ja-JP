---
title: MacOSScepCertificateProfile を更新します。
description: MacOSScepCertificateProfile オブジェクトのプロパティを更新します。
ms.openlocfilehash: 459e3eaa90533320b5d6039802d9dca81958ef04
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073731"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="3248d-103">MacOSScepCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="3248d-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="3248d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3248d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3248d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3248d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3248d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3248d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3248d-107">[MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3248d-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3248d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3248d-108">Prerequisites</span></span>
<span data-ttu-id="3248d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3248d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3248d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3248d-111">Permission type</span></span>|<span data-ttu-id="3248d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3248d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3248d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3248d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3248d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3248d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3248d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3248d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3248d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3248d-116">Not supported.</span></span>|
|<span data-ttu-id="3248d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3248d-117">Application</span></span>|<span data-ttu-id="3248d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3248d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3248d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3248d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3248d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3248d-120">Request headers</span></span>
|<span data-ttu-id="3248d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3248d-121">Header</span></span>|<span data-ttu-id="3248d-122">値</span><span class="sxs-lookup"><span data-stu-id="3248d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3248d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3248d-123">Authorization</span></span>|<span data-ttu-id="3248d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3248d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3248d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3248d-125">Accept</span></span>|<span data-ttu-id="3248d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3248d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3248d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3248d-127">Request body</span></span>
<span data-ttu-id="3248d-128">要求の本文に[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3248d-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="3248d-129">[MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="3248d-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="3248d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3248d-130">Property</span></span>|<span data-ttu-id="3248d-131">型</span><span class="sxs-lookup"><span data-stu-id="3248d-131">Type</span></span>|<span data-ttu-id="3248d-132">説明</span><span class="sxs-lookup"><span data-stu-id="3248d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3248d-133">id</span><span class="sxs-lookup"><span data-stu-id="3248d-133">id</span></span>|<span data-ttu-id="3248d-134">String</span><span class="sxs-lookup"><span data-stu-id="3248d-134">String</span></span>|<span data-ttu-id="3248d-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3248d-135">Key of the entity.</span></span> <span data-ttu-id="3248d-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3248d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3248d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3248d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3248d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3248d-138">DateTimeOffset</span></span>|<span data-ttu-id="3248d-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3248d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3248d-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3248d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3248d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3248d-141">roleScopeTagIds</span></span>|<span data-ttu-id="3248d-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3248d-142">String collection</span></span>|<span data-ttu-id="3248d-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="3248d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3248d-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3248d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3248d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3248d-145">supportsScopeTags</span></span>|<span data-ttu-id="3248d-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="3248d-146">Boolean</span></span>|<span data-ttu-id="3248d-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3248d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3248d-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="3248d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3248d-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="3248d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3248d-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3248d-150">This property is read-only.</span></span> <span data-ttu-id="3248d-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3248d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3248d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3248d-152">createdDateTime</span></span>|<span data-ttu-id="3248d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3248d-153">DateTimeOffset</span></span>|<span data-ttu-id="3248d-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3248d-154">DateTime the object was created.</span></span> <span data-ttu-id="3248d-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3248d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3248d-156">説明</span><span class="sxs-lookup"><span data-stu-id="3248d-156">description</span></span>|<span data-ttu-id="3248d-157">String</span><span class="sxs-lookup"><span data-stu-id="3248d-157">String</span></span>|<span data-ttu-id="3248d-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="3248d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3248d-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3248d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3248d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3248d-160">displayName</span></span>|<span data-ttu-id="3248d-161">String</span><span class="sxs-lookup"><span data-stu-id="3248d-161">String</span></span>|<span data-ttu-id="3248d-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="3248d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3248d-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3248d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3248d-164">version</span><span class="sxs-lookup"><span data-stu-id="3248d-164">version</span></span>|<span data-ttu-id="3248d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3248d-165">Int32</span></span>|<span data-ttu-id="3248d-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3248d-166">Version of the device configuration.</span></span> <span data-ttu-id="3248d-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3248d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3248d-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3248d-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="3248d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3248d-169">Int32</span></span>|<span data-ttu-id="3248d-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="3248d-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3248d-171">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3248d-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3248d-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3248d-172">subjectNameFormat</span></span>|[<span data-ttu-id="3248d-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3248d-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="3248d-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="3248d-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="3248d-175">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3248d-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="3248d-176">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="3248d-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="3248d-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3248d-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3248d-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3248d-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3248d-179">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="3248d-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="3248d-180">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3248d-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="3248d-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="3248d-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3248d-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3248d-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3248d-183">Int32</span><span class="sxs-lookup"><span data-stu-id="3248d-183">Int32</span></span>|<span data-ttu-id="3248d-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="3248d-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3248d-185">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="3248d-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3248d-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3248d-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3248d-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3248d-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3248d-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="3248d-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3248d-189">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3248d-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="3248d-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="3248d-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3248d-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="3248d-191">scepServerUrls</span></span>|<span data-ttu-id="3248d-192">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3248d-192">String collection</span></span>|<span data-ttu-id="3248d-193">SCEP サーバー個の url。</span><span class="sxs-lookup"><span data-stu-id="3248d-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="3248d-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3248d-194">subjectNameFormatString</span></span>|<span data-ttu-id="3248d-195">String</span><span class="sxs-lookup"><span data-stu-id="3248d-195">String</span></span>|<span data-ttu-id="3248d-196">SubjectNameFormat で使用するカスタム書式指定 = カスタムです。</span><span class="sxs-lookup"><span data-stu-id="3248d-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="3248d-197">例: CN = EmailAddress {{}}、E = EmailAddress {{}}、OU = エンタープライズ ユーザーの場合は、O = コントソ株式会社、L = Redmond、ST = ワシントン州 C = u. s.</span><span class="sxs-lookup"><span data-stu-id="3248d-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="3248d-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="3248d-198">keyUsage</span></span>|[<span data-ttu-id="3248d-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="3248d-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="3248d-200">SCEP のキー使用法です。</span><span class="sxs-lookup"><span data-stu-id="3248d-200">SCEP Key Usage.</span></span> <span data-ttu-id="3248d-201">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="3248d-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="3248d-202">キー長</span><span class="sxs-lookup"><span data-stu-id="3248d-202">keySize</span></span>|[<span data-ttu-id="3248d-203">キー長</span><span class="sxs-lookup"><span data-stu-id="3248d-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="3248d-204">SCEP のキー サイズ。</span><span class="sxs-lookup"><span data-stu-id="3248d-204">SCEP Key Size.</span></span> <span data-ttu-id="3248d-205">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="3248d-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="3248d-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3248d-206">hashAlgorithm</span></span>|[<span data-ttu-id="3248d-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="3248d-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="3248d-208">SCEP ハッシュ アルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="3248d-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="3248d-209">使用可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="3248d-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="3248d-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="3248d-210">extendedKeyUsages</span></span>|<span data-ttu-id="3248d-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3248d-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="3248d-212">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="3248d-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="3248d-213">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3248d-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3248d-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3248d-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3248d-215">String</span><span class="sxs-lookup"><span data-stu-id="3248d-215">String</span></span>|<span data-ttu-id="3248d-216">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="3248d-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="3248d-217">応答</span><span class="sxs-lookup"><span data-stu-id="3248d-217">Response</span></span>
<span data-ttu-id="3248d-218">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3248d-218">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3248d-219">例</span><span class="sxs-lookup"><span data-stu-id="3248d-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="3248d-220">要求</span><span class="sxs-lookup"><span data-stu-id="3248d-220">Request</span></span>
<span data-ttu-id="3248d-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3248d-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 963

{
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="3248d-222">応答</span><span class="sxs-lookup"><span data-stu-id="3248d-222">Response</span></span>
<span data-ttu-id="3248d-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3248d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





