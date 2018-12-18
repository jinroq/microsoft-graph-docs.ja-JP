---
title: AndroidWorkProfilePkcsCertificateProfile を更新します。
description: AndroidWorkProfilePkcsCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: dbd3adbcc15b7b46e51ff3a2874e340c78339ac2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355896"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="c1751-103">AndroidWorkProfilePkcsCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="c1751-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="c1751-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1751-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1751-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1751-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1751-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1751-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1751-107">[AndroidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c1751-107">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1751-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c1751-108">Prerequisites</span></span>
<span data-ttu-id="c1751-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1751-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1751-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1751-111">Permission type</span></span>|<span data-ttu-id="c1751-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1751-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1751-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1751-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1751-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1751-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1751-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1751-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1751-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1751-116">Not supported.</span></span>|
|<span data-ttu-id="c1751-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1751-117">Application</span></span>|<span data-ttu-id="c1751-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1751-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1751-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1751-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1751-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1751-120">Request headers</span></span>
|<span data-ttu-id="c1751-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1751-121">Header</span></span>|<span data-ttu-id="c1751-122">値</span><span class="sxs-lookup"><span data-stu-id="c1751-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1751-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1751-123">Authorization</span></span>|<span data-ttu-id="c1751-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c1751-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1751-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1751-125">Accept</span></span>|<span data-ttu-id="c1751-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1751-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1751-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1751-127">Request body</span></span>
<span data-ttu-id="c1751-128">要求の本文に[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c1751-128">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="c1751-129">[AndroidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c1751-129">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="c1751-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1751-130">Property</span></span>|<span data-ttu-id="c1751-131">種類</span><span class="sxs-lookup"><span data-stu-id="c1751-131">Type</span></span>|<span data-ttu-id="c1751-132">説明</span><span class="sxs-lookup"><span data-stu-id="c1751-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1751-133">ID</span><span class="sxs-lookup"><span data-stu-id="c1751-133">id</span></span>|<span data-ttu-id="c1751-134">String</span><span class="sxs-lookup"><span data-stu-id="c1751-134">String</span></span>|<span data-ttu-id="c1751-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c1751-135">Key of the entity.</span></span> <span data-ttu-id="c1751-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1751-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1751-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1751-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c1751-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1751-138">DateTimeOffset</span></span>|<span data-ttu-id="c1751-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c1751-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c1751-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1751-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1751-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1751-141">roleScopeTagIds</span></span>|<span data-ttu-id="c1751-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1751-142">String collection</span></span>|<span data-ttu-id="c1751-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="c1751-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1751-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1751-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1751-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1751-145">supportsScopeTags</span></span>|<span data-ttu-id="c1751-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="c1751-146">Boolean</span></span>|<span data-ttu-id="c1751-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c1751-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1751-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="c1751-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1751-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="c1751-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1751-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c1751-150">This property is read-only.</span></span> <span data-ttu-id="c1751-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1751-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1751-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1751-152">createdDateTime</span></span>|<span data-ttu-id="c1751-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1751-153">DateTimeOffset</span></span>|<span data-ttu-id="c1751-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c1751-154">DateTime the object was created.</span></span> <span data-ttu-id="c1751-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1751-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1751-156">説明</span><span class="sxs-lookup"><span data-stu-id="c1751-156">description</span></span>|<span data-ttu-id="c1751-157">String</span><span class="sxs-lookup"><span data-stu-id="c1751-157">String</span></span>|<span data-ttu-id="c1751-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c1751-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1751-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1751-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1751-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c1751-160">displayName</span></span>|<span data-ttu-id="c1751-161">String</span><span class="sxs-lookup"><span data-stu-id="c1751-161">String</span></span>|<span data-ttu-id="c1751-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c1751-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1751-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1751-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1751-164">version</span><span class="sxs-lookup"><span data-stu-id="c1751-164">version</span></span>|<span data-ttu-id="c1751-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c1751-165">Int32</span></span>|<span data-ttu-id="c1751-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c1751-166">Version of the device configuration.</span></span> <span data-ttu-id="c1751-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1751-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1751-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c1751-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="c1751-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c1751-169">Int32</span></span>|<span data-ttu-id="c1751-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="c1751-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c1751-171">有効な値は[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="c1751-171">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c1751-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c1751-172">subjectNameFormat</span></span>|[<span data-ttu-id="c1751-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c1751-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c1751-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="c1751-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="c1751-175">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c1751-175">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c1751-176">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="c1751-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c1751-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c1751-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c1751-178">Int32</span><span class="sxs-lookup"><span data-stu-id="c1751-178">Int32</span></span>|<span data-ttu-id="c1751-179">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="c1751-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c1751-180">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="c1751-180">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c1751-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c1751-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c1751-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c1751-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c1751-183">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="c1751-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c1751-184">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c1751-184">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c1751-185">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="c1751-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c1751-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c1751-186">extendedKeyUsages</span></span>|<span data-ttu-id="c1751-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c1751-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c1751-188">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="c1751-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c1751-189">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c1751-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c1751-190">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="c1751-190">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c1751-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="c1751-191">certificationAuthority</span></span>|<span data-ttu-id="c1751-192">String</span><span class="sxs-lookup"><span data-stu-id="c1751-192">String</span></span>|<span data-ttu-id="c1751-193">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="c1751-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="c1751-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="c1751-194">certificationAuthorityName</span></span>|<span data-ttu-id="c1751-195">String</span><span class="sxs-lookup"><span data-stu-id="c1751-195">String</span></span>|<span data-ttu-id="c1751-196">PKCS 証明機関の名前</span><span class="sxs-lookup"><span data-stu-id="c1751-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="c1751-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="c1751-197">certificateTemplateName</span></span>|<span data-ttu-id="c1751-198">String</span><span class="sxs-lookup"><span data-stu-id="c1751-198">String</span></span>|<span data-ttu-id="c1751-199">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="c1751-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="c1751-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c1751-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c1751-201">String</span><span class="sxs-lookup"><span data-stu-id="c1751-201">String</span></span>|<span data-ttu-id="c1751-202">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="c1751-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="c1751-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c1751-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c1751-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c1751-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c1751-205">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="c1751-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c1751-206">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="c1751-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="c1751-207">応答</span><span class="sxs-lookup"><span data-stu-id="c1751-207">Response</span></span>
<span data-ttu-id="c1751-208">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c1751-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1751-209">例</span><span class="sxs-lookup"><span data-stu-id="c1751-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1751-210">要求</span><span class="sxs-lookup"><span data-stu-id="c1751-210">Request</span></span>
<span data-ttu-id="c1751-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c1751-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 954

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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="c1751-212">応答</span><span class="sxs-lookup"><span data-stu-id="c1751-212">Response</span></span>
<span data-ttu-id="c1751-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c1751-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1141

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```





