---
title: IosScepCertificateProfile を作成します。
description: 新しい iosScepCertificateProfile オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: b81cec3750739fc5e1534af2c8c86d2e05301830
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357646"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="9f588-103">IosScepCertificateProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="9f588-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="9f588-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f588-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f588-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f588-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f588-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f588-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f588-107">新しい[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f588-107">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f588-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9f588-108">Prerequisites</span></span>
<span data-ttu-id="9f588-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f588-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f588-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f588-111">Permission type</span></span>|<span data-ttu-id="9f588-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f588-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f588-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f588-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f588-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f588-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f588-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f588-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f588-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f588-116">Not supported.</span></span>|
|<span data-ttu-id="9f588-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f588-117">Application</span></span>|<span data-ttu-id="9f588-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f588-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f588-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f588-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9f588-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f588-120">Request headers</span></span>
|<span data-ttu-id="9f588-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f588-121">Header</span></span>|<span data-ttu-id="9f588-122">値</span><span class="sxs-lookup"><span data-stu-id="9f588-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f588-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f588-123">Authorization</span></span>|<span data-ttu-id="9f588-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9f588-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f588-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f588-125">Accept</span></span>|<span data-ttu-id="9f588-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f588-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f588-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f588-127">Request body</span></span>
<span data-ttu-id="9f588-128">要求の本文に iosScepCertificateProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f588-128">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="9f588-129">次の表は、iosScepCertificateProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9f588-129">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="9f588-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f588-130">Property</span></span>|<span data-ttu-id="9f588-131">種類</span><span class="sxs-lookup"><span data-stu-id="9f588-131">Type</span></span>|<span data-ttu-id="9f588-132">説明</span><span class="sxs-lookup"><span data-stu-id="9f588-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f588-133">ID</span><span class="sxs-lookup"><span data-stu-id="9f588-133">id</span></span>|<span data-ttu-id="9f588-134">String</span><span class="sxs-lookup"><span data-stu-id="9f588-134">String</span></span>|<span data-ttu-id="9f588-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9f588-135">Key of the entity.</span></span> <span data-ttu-id="9f588-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f588-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f588-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f588-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9f588-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f588-138">DateTimeOffset</span></span>|<span data-ttu-id="9f588-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9f588-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9f588-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f588-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f588-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f588-141">roleScopeTagIds</span></span>|<span data-ttu-id="9f588-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9f588-142">String collection</span></span>|<span data-ttu-id="9f588-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="9f588-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9f588-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f588-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f588-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9f588-145">supportsScopeTags</span></span>|<span data-ttu-id="9f588-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="9f588-146">Boolean</span></span>|<span data-ttu-id="9f588-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9f588-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9f588-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="9f588-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9f588-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="9f588-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9f588-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9f588-150">This property is read-only.</span></span> <span data-ttu-id="9f588-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f588-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f588-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f588-152">createdDateTime</span></span>|<span data-ttu-id="9f588-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f588-153">DateTimeOffset</span></span>|<span data-ttu-id="9f588-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9f588-154">DateTime the object was created.</span></span> <span data-ttu-id="9f588-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f588-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f588-156">説明</span><span class="sxs-lookup"><span data-stu-id="9f588-156">description</span></span>|<span data-ttu-id="9f588-157">String</span><span class="sxs-lookup"><span data-stu-id="9f588-157">String</span></span>|<span data-ttu-id="9f588-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9f588-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f588-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f588-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f588-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9f588-160">displayName</span></span>|<span data-ttu-id="9f588-161">String</span><span class="sxs-lookup"><span data-stu-id="9f588-161">String</span></span>|<span data-ttu-id="9f588-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9f588-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f588-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f588-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f588-164">version</span><span class="sxs-lookup"><span data-stu-id="9f588-164">version</span></span>|<span data-ttu-id="9f588-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9f588-165">Int32</span></span>|<span data-ttu-id="9f588-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9f588-166">Version of the device configuration.</span></span> <span data-ttu-id="9f588-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f588-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f588-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9f588-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="9f588-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9f588-169">Int32</span></span>|<span data-ttu-id="9f588-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="9f588-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9f588-171">有効な値は[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="9f588-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9f588-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9f588-172">subjectNameFormat</span></span>|[<span data-ttu-id="9f588-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9f588-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="9f588-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="9f588-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="9f588-175">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9f588-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="9f588-176">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="9f588-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="9f588-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9f588-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9f588-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9f588-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9f588-179">証明書のサブジェクトの別名の種類です。</span><span class="sxs-lookup"><span data-stu-id="9f588-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="9f588-180">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9f588-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="9f588-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="9f588-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9f588-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9f588-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9f588-183">Int32</span><span class="sxs-lookup"><span data-stu-id="9f588-183">Int32</span></span>|<span data-ttu-id="9f588-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="9f588-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="9f588-185">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9f588-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9f588-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9f588-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9f588-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9f588-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9f588-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="9f588-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9f588-189">[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9f588-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="9f588-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="9f588-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9f588-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="9f588-191">scepServerUrls</span></span>|<span data-ttu-id="9f588-192">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9f588-192">String collection</span></span>|<span data-ttu-id="9f588-193">SCEP サーバー個の url。</span><span class="sxs-lookup"><span data-stu-id="9f588-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="9f588-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9f588-194">subjectNameFormatString</span></span>|<span data-ttu-id="9f588-195">String</span><span class="sxs-lookup"><span data-stu-id="9f588-195">String</span></span>|<span data-ttu-id="9f588-196">SubjectNameFormat で使用するカスタム書式指定 = カスタムです。</span><span class="sxs-lookup"><span data-stu-id="9f588-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="9f588-197">例: CN = EmailAddress {{}}、E = EmailAddress {{}}、OU = エンタープライズ ユーザーの場合は、O = コントソ株式会社、L = Redmond、ST = ワシントン州 C = u. s.</span><span class="sxs-lookup"><span data-stu-id="9f588-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="9f588-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="9f588-198">keyUsage</span></span>|[<span data-ttu-id="9f588-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="9f588-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="9f588-200">SCEP のキー使用法です。</span><span class="sxs-lookup"><span data-stu-id="9f588-200">SCEP Key Usage.</span></span> <span data-ttu-id="9f588-201">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="9f588-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="9f588-202">キー長</span><span class="sxs-lookup"><span data-stu-id="9f588-202">keySize</span></span>|[<span data-ttu-id="9f588-203">キー長</span><span class="sxs-lookup"><span data-stu-id="9f588-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="9f588-204">SCEP のキー サイズ。</span><span class="sxs-lookup"><span data-stu-id="9f588-204">SCEP Key Size.</span></span> <span data-ttu-id="9f588-205">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="9f588-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="9f588-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9f588-206">extendedKeyUsages</span></span>|<span data-ttu-id="9f588-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9f588-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="9f588-208">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="9f588-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="9f588-209">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9f588-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9f588-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9f588-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="9f588-211">String</span><span class="sxs-lookup"><span data-stu-id="9f588-211">String</span></span>|<span data-ttu-id="9f588-212">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="9f588-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="9f588-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9f588-213">certificateStore</span></span>|[<span data-ttu-id="9f588-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9f588-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="9f588-215">ターゲット ストアの証明書です。</span><span class="sxs-lookup"><span data-stu-id="9f588-215">Target store certificate.</span></span> <span data-ttu-id="9f588-216">使用可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="9f588-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="9f588-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="9f588-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="9f588-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9f588-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="9f588-219">Alterantive 名の設定をカスタムの件名です。</span><span class="sxs-lookup"><span data-stu-id="9f588-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="9f588-220">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9f588-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="9f588-221">応答</span><span class="sxs-lookup"><span data-stu-id="9f588-221">Response</span></span>
<span data-ttu-id="9f588-222">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9f588-222">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f588-223">例</span><span class="sxs-lookup"><span data-stu-id="9f588-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f588-224">要求</span><span class="sxs-lookup"><span data-stu-id="9f588-224">Request</span></span>
<span data-ttu-id="9f588-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f588-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="9f588-226">応答</span><span class="sxs-lookup"><span data-stu-id="9f588-226">Response</span></span>
<span data-ttu-id="9f588-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9f588-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




