---
title: AndroidScepCertificateProfile を更新します。
description: AndroidScepCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 437a1ab0e8d257b0e9216782abf118f5af50671a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836933"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="5b37c-103">AndroidScepCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="5b37c-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="5b37c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b37c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b37c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b37c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b37c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b37c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b37c-107">[AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5b37c-107">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b37c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5b37c-108">Prerequisites</span></span>
<span data-ttu-id="5b37c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b37c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b37c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b37c-111">Permission type</span></span>|<span data-ttu-id="5b37c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b37c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b37c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b37c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b37c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b37c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b37c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b37c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b37c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b37c-116">Not supported.</span></span>|
|<span data-ttu-id="5b37c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b37c-117">Application</span></span>|<span data-ttu-id="5b37c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b37c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b37c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b37c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5b37c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b37c-120">Request headers</span></span>
|<span data-ttu-id="5b37c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b37c-121">Header</span></span>|<span data-ttu-id="5b37c-122">値</span><span class="sxs-lookup"><span data-stu-id="5b37c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b37c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b37c-123">Authorization</span></span>|<span data-ttu-id="5b37c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5b37c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b37c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b37c-125">Accept</span></span>|<span data-ttu-id="5b37c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b37c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b37c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b37c-127">Request body</span></span>
<span data-ttu-id="5b37c-128">要求の本文に[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b37c-128">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="5b37c-129">[AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="5b37c-129">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="5b37c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b37c-130">Property</span></span>|<span data-ttu-id="5b37c-131">種類</span><span class="sxs-lookup"><span data-stu-id="5b37c-131">Type</span></span>|<span data-ttu-id="5b37c-132">説明</span><span class="sxs-lookup"><span data-stu-id="5b37c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b37c-133">ID</span><span class="sxs-lookup"><span data-stu-id="5b37c-133">id</span></span>|<span data-ttu-id="5b37c-134">String</span><span class="sxs-lookup"><span data-stu-id="5b37c-134">String</span></span>|<span data-ttu-id="5b37c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5b37c-135">Key of the entity.</span></span> <span data-ttu-id="5b37c-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b37c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b37c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b37c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5b37c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b37c-138">DateTimeOffset</span></span>|<span data-ttu-id="5b37c-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5b37c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5b37c-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b37c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b37c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b37c-141">roleScopeTagIds</span></span>|<span data-ttu-id="5b37c-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5b37c-142">String collection</span></span>|<span data-ttu-id="5b37c-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="5b37c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5b37c-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b37c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b37c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5b37c-145">supportsScopeTags</span></span>|<span data-ttu-id="5b37c-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="5b37c-146">Boolean</span></span>|<span data-ttu-id="5b37c-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b37c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5b37c-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="5b37c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5b37c-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="5b37c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5b37c-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-150">This property is read-only.</span></span> <span data-ttu-id="5b37c-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b37c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b37c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b37c-152">createdDateTime</span></span>|<span data-ttu-id="5b37c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b37c-153">DateTimeOffset</span></span>|<span data-ttu-id="5b37c-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5b37c-154">DateTime the object was created.</span></span> <span data-ttu-id="5b37c-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b37c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b37c-156">説明</span><span class="sxs-lookup"><span data-stu-id="5b37c-156">description</span></span>|<span data-ttu-id="5b37c-157">String</span><span class="sxs-lookup"><span data-stu-id="5b37c-157">String</span></span>|<span data-ttu-id="5b37c-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="5b37c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b37c-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b37c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b37c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5b37c-160">displayName</span></span>|<span data-ttu-id="5b37c-161">String</span><span class="sxs-lookup"><span data-stu-id="5b37c-161">String</span></span>|<span data-ttu-id="5b37c-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="5b37c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b37c-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b37c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b37c-164">version</span><span class="sxs-lookup"><span data-stu-id="5b37c-164">version</span></span>|<span data-ttu-id="5b37c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5b37c-165">Int32</span></span>|<span data-ttu-id="5b37c-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5b37c-166">Version of the device configuration.</span></span> <span data-ttu-id="5b37c-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b37c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b37c-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5b37c-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="5b37c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="5b37c-169">Int32</span></span>|<span data-ttu-id="5b37c-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5b37c-171">有効な値は[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="5b37c-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5b37c-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5b37c-172">subjectNameFormat</span></span>|[<span data-ttu-id="5b37c-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5b37c-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="5b37c-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="5b37c-175">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="5b37c-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="5b37c-176">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="5b37c-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5b37c-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5b37c-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5b37c-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5b37c-179">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="5b37c-180">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="5b37c-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="5b37c-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5b37c-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5b37c-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5b37c-183">Int32</span><span class="sxs-lookup"><span data-stu-id="5b37c-183">Int32</span></span>|<span data-ttu-id="5b37c-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5b37c-185">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5b37c-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5b37c-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5b37c-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5b37c-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5b37c-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5b37c-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="5b37c-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5b37c-189">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="5b37c-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="5b37c-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5b37c-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="5b37c-191">extendedKeyUsages</span></span>|<span data-ttu-id="5b37c-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5b37c-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="5b37c-193">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="5b37c-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="5b37c-194">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5b37c-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5b37c-195">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5b37c-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5b37c-196">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="5b37c-196">scepServerUrls</span></span>|<span data-ttu-id="5b37c-197">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5b37c-197">String collection</span></span>|<span data-ttu-id="5b37c-198">SCEP サーバー個の url</span><span class="sxs-lookup"><span data-stu-id="5b37c-198">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="5b37c-199">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5b37c-199">subjectNameFormatString</span></span>|<span data-ttu-id="5b37c-200">String</span><span class="sxs-lookup"><span data-stu-id="5b37c-200">String</span></span>|<span data-ttu-id="5b37c-201">SubjectNameFormat で使用するカスタム書式指定 = カスタムです。</span><span class="sxs-lookup"><span data-stu-id="5b37c-201">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="5b37c-202">例: CN = EmailAddress {{}}、E = EmailAddress {{}}、OU = エンタープライズ ユーザーの場合は、O = コントソ株式会社、L = Redmond、ST = ワシントン州 C = u. s.</span><span class="sxs-lookup"><span data-stu-id="5b37c-202">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="5b37c-203">keyUsage</span><span class="sxs-lookup"><span data-stu-id="5b37c-203">keyUsage</span></span>|[<span data-ttu-id="5b37c-204">keyUsages</span><span class="sxs-lookup"><span data-stu-id="5b37c-204">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="5b37c-205">SCEP のキー使用法です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-205">SCEP Key Usage.</span></span> <span data-ttu-id="5b37c-206">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-206">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="5b37c-207">キー長</span><span class="sxs-lookup"><span data-stu-id="5b37c-207">keySize</span></span>|[<span data-ttu-id="5b37c-208">キー長</span><span class="sxs-lookup"><span data-stu-id="5b37c-208">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="5b37c-209">SCEP のキー サイズ。</span><span class="sxs-lookup"><span data-stu-id="5b37c-209">SCEP Key Size.</span></span> <span data-ttu-id="5b37c-210">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-210">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="5b37c-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="5b37c-211">hashAlgorithm</span></span>|[<span data-ttu-id="5b37c-212">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="5b37c-212">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="5b37c-213">SCEP ハッシュ アルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="5b37c-213">SCEP Hash Algorithm.</span></span> <span data-ttu-id="5b37c-214">使用可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-214">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="5b37c-215">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5b37c-215">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5b37c-216">String</span><span class="sxs-lookup"><span data-stu-id="5b37c-216">String</span></span>|<span data-ttu-id="5b37c-217">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="5b37c-217">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="5b37c-218">応答</span><span class="sxs-lookup"><span data-stu-id="5b37c-218">Response</span></span>
<span data-ttu-id="5b37c-219">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5b37c-219">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b37c-220">例</span><span class="sxs-lookup"><span data-stu-id="5b37c-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b37c-221">要求</span><span class="sxs-lookup"><span data-stu-id="5b37c-221">Request</span></span>
<span data-ttu-id="5b37c-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b37c-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 970

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
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="5b37c-223">応答</span><span class="sxs-lookup"><span data-stu-id="5b37c-223">Response</span></span>
<span data-ttu-id="5b37c-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b37c-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1146

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





