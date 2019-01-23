---
title: AndroidPkcsCertificateProfile を作成します。
description: 新しい androidPkcsCertificateProfile オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9efcf4361d168cd44bbbe16da43941d3ed1215f5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395175"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="fab20-103">AndroidPkcsCertificateProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="fab20-103">Create androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="fab20-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fab20-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fab20-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fab20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fab20-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fab20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fab20-107">新しい[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fab20-107">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fab20-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fab20-108">Prerequisites</span></span>
<span data-ttu-id="fab20-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fab20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fab20-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fab20-111">Permission type</span></span>|<span data-ttu-id="fab20-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fab20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fab20-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fab20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fab20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fab20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fab20-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fab20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fab20-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fab20-116">Not supported.</span></span>|
|<span data-ttu-id="fab20-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fab20-117">Application</span></span>|<span data-ttu-id="fab20-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fab20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fab20-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fab20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fab20-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fab20-120">Request headers</span></span>
|<span data-ttu-id="fab20-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fab20-121">Header</span></span>|<span data-ttu-id="fab20-122">値</span><span class="sxs-lookup"><span data-stu-id="fab20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fab20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fab20-123">Authorization</span></span>|<span data-ttu-id="fab20-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fab20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fab20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fab20-125">Accept</span></span>|<span data-ttu-id="fab20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fab20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fab20-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fab20-127">Request body</span></span>
<span data-ttu-id="fab20-128">要求の本文に androidPkcsCertificateProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fab20-128">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="fab20-129">次の表は、androidPkcsCertificateProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fab20-129">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="fab20-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fab20-130">Property</span></span>|<span data-ttu-id="fab20-131">型</span><span class="sxs-lookup"><span data-stu-id="fab20-131">Type</span></span>|<span data-ttu-id="fab20-132">説明</span><span class="sxs-lookup"><span data-stu-id="fab20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fab20-133">id</span><span class="sxs-lookup"><span data-stu-id="fab20-133">id</span></span>|<span data-ttu-id="fab20-134">String</span><span class="sxs-lookup"><span data-stu-id="fab20-134">String</span></span>|<span data-ttu-id="fab20-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fab20-135">Key of the entity.</span></span> <span data-ttu-id="fab20-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab20-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab20-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fab20-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fab20-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fab20-138">DateTimeOffset</span></span>|<span data-ttu-id="fab20-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fab20-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fab20-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab20-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab20-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fab20-141">roleScopeTagIds</span></span>|<span data-ttu-id="fab20-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fab20-142">String collection</span></span>|<span data-ttu-id="fab20-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="fab20-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fab20-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab20-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab20-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fab20-145">supportsScopeTags</span></span>|<span data-ttu-id="fab20-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fab20-146">Boolean</span></span>|<span data-ttu-id="fab20-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fab20-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fab20-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="fab20-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fab20-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="fab20-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fab20-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fab20-150">This property is read-only.</span></span> <span data-ttu-id="fab20-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab20-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab20-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fab20-152">createdDateTime</span></span>|<span data-ttu-id="fab20-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fab20-153">DateTimeOffset</span></span>|<span data-ttu-id="fab20-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fab20-154">DateTime the object was created.</span></span> <span data-ttu-id="fab20-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab20-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab20-156">説明</span><span class="sxs-lookup"><span data-stu-id="fab20-156">description</span></span>|<span data-ttu-id="fab20-157">String</span><span class="sxs-lookup"><span data-stu-id="fab20-157">String</span></span>|<span data-ttu-id="fab20-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="fab20-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fab20-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab20-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab20-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fab20-160">displayName</span></span>|<span data-ttu-id="fab20-161">String</span><span class="sxs-lookup"><span data-stu-id="fab20-161">String</span></span>|<span data-ttu-id="fab20-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="fab20-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fab20-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab20-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab20-164">version</span><span class="sxs-lookup"><span data-stu-id="fab20-164">version</span></span>|<span data-ttu-id="fab20-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fab20-165">Int32</span></span>|<span data-ttu-id="fab20-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="fab20-166">Version of the device configuration.</span></span> <span data-ttu-id="fab20-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab20-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab20-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="fab20-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="fab20-169">Int32</span><span class="sxs-lookup"><span data-stu-id="fab20-169">Int32</span></span>|<span data-ttu-id="fab20-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="fab20-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="fab20-171">有効な値は[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="fab20-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fab20-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fab20-172">subjectNameFormat</span></span>|[<span data-ttu-id="fab20-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fab20-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="fab20-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="fab20-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="fab20-175">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="fab20-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="fab20-176">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="fab20-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="fab20-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fab20-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="fab20-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fab20-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="fab20-179">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="fab20-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="fab20-180">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="fab20-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="fab20-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="fab20-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="fab20-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="fab20-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="fab20-183">Int32</span><span class="sxs-lookup"><span data-stu-id="fab20-183">Int32</span></span>|<span data-ttu-id="fab20-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="fab20-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="fab20-185">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="fab20-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fab20-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fab20-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="fab20-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fab20-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="fab20-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="fab20-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="fab20-189">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="fab20-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="fab20-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="fab20-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="fab20-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="fab20-191">extendedKeyUsages</span></span>|<span data-ttu-id="fab20-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fab20-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="fab20-193">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="fab20-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="fab20-194">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="fab20-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="fab20-195">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="fab20-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fab20-196">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="fab20-196">certificationAuthority</span></span>|<span data-ttu-id="fab20-197">String</span><span class="sxs-lookup"><span data-stu-id="fab20-197">String</span></span>|<span data-ttu-id="fab20-198">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="fab20-198">PKCS Certification Authority</span></span>|
|<span data-ttu-id="fab20-199">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="fab20-199">certificationAuthorityName</span></span>|<span data-ttu-id="fab20-200">String</span><span class="sxs-lookup"><span data-stu-id="fab20-200">String</span></span>|<span data-ttu-id="fab20-201">PKCS 証明機関の名前</span><span class="sxs-lookup"><span data-stu-id="fab20-201">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="fab20-202">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="fab20-202">certificateTemplateName</span></span>|<span data-ttu-id="fab20-203">String</span><span class="sxs-lookup"><span data-stu-id="fab20-203">String</span></span>|<span data-ttu-id="fab20-204">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="fab20-204">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="fab20-205">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fab20-205">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="fab20-206">String</span><span class="sxs-lookup"><span data-stu-id="fab20-206">String</span></span>|<span data-ttu-id="fab20-207">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="fab20-207">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="fab20-208">応答</span><span class="sxs-lookup"><span data-stu-id="fab20-208">Response</span></span>
<span data-ttu-id="fab20-209">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fab20-209">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fab20-210">例</span><span class="sxs-lookup"><span data-stu-id="fab20-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="fab20-211">要求</span><span class="sxs-lookup"><span data-stu-id="fab20-211">Request</span></span>
<span data-ttu-id="fab20-212">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fab20-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 958

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="fab20-213">応答</span><span class="sxs-lookup"><span data-stu-id="fab20-213">Response</span></span>
<span data-ttu-id="fab20-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fab20-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




