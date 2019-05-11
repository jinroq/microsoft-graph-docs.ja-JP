---
title: IosScepCertificateProfile の作成
description: 新しい iosScepCertificateProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af3b0a05624b4950372669e027da41068d6fc4d5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923399"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="c8665-103">IosScepCertificateProfile の作成</span><span class="sxs-lookup"><span data-stu-id="c8665-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="c8665-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8665-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8665-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8665-106">新しい[Iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8665-106">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8665-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8665-107">Prerequisites</span></span>
<span data-ttu-id="c8665-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8665-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8665-110">Permission type</span></span>|<span data-ttu-id="c8665-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8665-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8665-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8665-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8665-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8665-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8665-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8665-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8665-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8665-115">Not supported.</span></span>|
|<span data-ttu-id="c8665-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8665-116">Application</span></span>|<span data-ttu-id="c8665-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8665-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8665-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8665-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c8665-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8665-119">Request headers</span></span>
|<span data-ttu-id="c8665-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8665-120">Header</span></span>|<span data-ttu-id="c8665-121">値</span><span class="sxs-lookup"><span data-stu-id="c8665-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8665-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8665-122">Authorization</span></span>|<span data-ttu-id="c8665-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8665-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8665-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c8665-124">Accept</span></span>|<span data-ttu-id="c8665-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8665-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8665-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8665-126">Request body</span></span>
<span data-ttu-id="c8665-127">要求本文で、iosScepCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8665-127">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="c8665-128">次の表に、iosScepCertificateProfile プロファイルの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c8665-128">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="c8665-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8665-129">Property</span></span>|<span data-ttu-id="c8665-130">型</span><span class="sxs-lookup"><span data-stu-id="c8665-130">Type</span></span>|<span data-ttu-id="c8665-131">説明</span><span class="sxs-lookup"><span data-stu-id="c8665-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8665-132">id</span><span class="sxs-lookup"><span data-stu-id="c8665-132">id</span></span>|<span data-ttu-id="c8665-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c8665-133">String</span></span>|<span data-ttu-id="c8665-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c8665-134">Key of the entity.</span></span> <span data-ttu-id="c8665-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8665-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8665-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c8665-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8665-137">DateTimeOffset</span></span>|<span data-ttu-id="c8665-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="c8665-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c8665-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8665-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c8665-140">roleScopeTagIds</span></span>|<span data-ttu-id="c8665-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c8665-141">String collection</span></span>|<span data-ttu-id="c8665-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c8665-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c8665-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8665-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c8665-144">supportsScopeTags</span></span>|<span data-ttu-id="c8665-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8665-145">Boolean</span></span>|<span data-ttu-id="c8665-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c8665-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c8665-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="c8665-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c8665-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="c8665-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c8665-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="c8665-149">This property is read-only.</span></span> <span data-ttu-id="c8665-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8665-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8665-151">createdDateTime</span></span>|<span data-ttu-id="c8665-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8665-152">DateTimeOffset</span></span>|<span data-ttu-id="c8665-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c8665-153">DateTime the object was created.</span></span> <span data-ttu-id="c8665-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8665-155">description</span><span class="sxs-lookup"><span data-stu-id="c8665-155">description</span></span>|<span data-ttu-id="c8665-156">String</span><span class="sxs-lookup"><span data-stu-id="c8665-156">String</span></span>|<span data-ttu-id="c8665-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="c8665-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c8665-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8665-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c8665-159">displayName</span></span>|<span data-ttu-id="c8665-160">String</span><span class="sxs-lookup"><span data-stu-id="c8665-160">String</span></span>|<span data-ttu-id="c8665-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="c8665-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c8665-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8665-163">version</span><span class="sxs-lookup"><span data-stu-id="c8665-163">version</span></span>|<span data-ttu-id="c8665-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c8665-164">Int32</span></span>|<span data-ttu-id="c8665-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c8665-165">Version of the device configuration.</span></span> <span data-ttu-id="c8665-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8665-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c8665-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="c8665-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c8665-168">Int32</span></span>|<span data-ttu-id="c8665-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="c8665-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c8665-170">有効な値は、 [Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承された値 1 ~ 99 です。</span><span class="sxs-lookup"><span data-stu-id="c8665-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c8665-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c8665-171">subjectNameFormat</span></span>|[<span data-ttu-id="c8665-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c8665-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="c8665-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="c8665-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="c8665-174">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c8665-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c8665-175">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="c8665-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="c8665-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c8665-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c8665-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c8665-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c8665-178">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="c8665-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="c8665-179">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c8665-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c8665-180">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="c8665-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c8665-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c8665-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c8665-182">Int32</span><span class="sxs-lookup"><span data-stu-id="c8665-182">Int32</span></span>|<span data-ttu-id="c8665-183">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="c8665-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c8665-184">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="c8665-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c8665-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c8665-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c8665-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c8665-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c8665-187">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="c8665-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c8665-188">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c8665-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c8665-189">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="c8665-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c8665-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="c8665-190">scepServerUrls</span></span>|<span data-ttu-id="c8665-191">String collection</span><span class="sxs-lookup"><span data-stu-id="c8665-191">String collection</span></span>|<span data-ttu-id="c8665-192">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="c8665-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="c8665-193">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8665-193">subjectNameFormatString</span></span>|<span data-ttu-id="c8665-194">String</span><span class="sxs-lookup"><span data-stu-id="c8665-194">String</span></span>|<span data-ttu-id="c8665-195">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="c8665-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c8665-196">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="c8665-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c8665-197">keyUsage</span><span class="sxs-lookup"><span data-stu-id="c8665-197">keyUsage</span></span>|[<span data-ttu-id="c8665-198">keyUsages</span><span class="sxs-lookup"><span data-stu-id="c8665-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c8665-199">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="c8665-199">SCEP Key Usage.</span></span> <span data-ttu-id="c8665-200">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="c8665-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c8665-201">keySize</span><span class="sxs-lookup"><span data-stu-id="c8665-201">keySize</span></span>|[<span data-ttu-id="c8665-202">keySize</span><span class="sxs-lookup"><span data-stu-id="c8665-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="c8665-203">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="c8665-203">SCEP Key Size.</span></span> <span data-ttu-id="c8665-204">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="c8665-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="c8665-205">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c8665-205">extendedKeyUsages</span></span>|<span data-ttu-id="c8665-206">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c8665-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c8665-207">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="c8665-207">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c8665-208">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c8665-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c8665-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c8665-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c8665-210">String</span><span class="sxs-lookup"><span data-stu-id="c8665-210">String</span></span>|<span data-ttu-id="c8665-211">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="c8665-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="c8665-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c8665-212">certificateStore</span></span>|[<span data-ttu-id="c8665-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c8665-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="c8665-214">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="c8665-214">Target store certificate.</span></span> <span data-ttu-id="c8665-215">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="c8665-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c8665-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="c8665-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="c8665-217">[Customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="c8665-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="c8665-218">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="c8665-218">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="c8665-219">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c8665-219">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c8665-220">応答</span><span class="sxs-lookup"><span data-stu-id="c8665-220">Response</span></span>
<span data-ttu-id="c8665-221">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8665-221">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8665-222">例</span><span class="sxs-lookup"><span data-stu-id="c8665-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8665-223">要求</span><span class="sxs-lookup"><span data-stu-id="c8665-223">Request</span></span>
<span data-ttu-id="c8665-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8665-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c8665-225">応答</span><span class="sxs-lookup"><span data-stu-id="c8665-225">Response</span></span>
<span data-ttu-id="c8665-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8665-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




