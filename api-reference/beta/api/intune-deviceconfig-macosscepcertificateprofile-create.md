---
title: macosscepcertificateprofile の作成
description: 新しい macosscepcertificateprofile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c40bd6835f562c52fa03720472802a569e8a5c23
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972894"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="f88f5-103">macosscepcertificateprofile の作成</span><span class="sxs-lookup"><span data-stu-id="f88f5-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="f88f5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f88f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f88f5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f88f5-106">新しい[macosscepcertificateprofile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-106">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f88f5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f88f5-107">Prerequisites</span></span>
<span data-ttu-id="f88f5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f88f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f88f5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f88f5-110">Permission type</span></span>|<span data-ttu-id="f88f5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f88f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f88f5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f88f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f88f5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f88f5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f88f5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f88f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f88f5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f88f5-115">Not supported.</span></span>|
|<span data-ttu-id="f88f5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f88f5-116">Application</span></span>|<span data-ttu-id="f88f5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f88f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f88f5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f88f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f88f5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f88f5-119">Request headers</span></span>
|<span data-ttu-id="f88f5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f88f5-120">Header</span></span>|<span data-ttu-id="f88f5-121">値</span><span class="sxs-lookup"><span data-stu-id="f88f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f88f5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f88f5-122">Authorization</span></span>|<span data-ttu-id="f88f5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f88f5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f88f5-124">Accept</span></span>|<span data-ttu-id="f88f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f88f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f88f5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f88f5-126">Request body</span></span>
<span data-ttu-id="f88f5-127">要求本文で、macosscepcertificateprofile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-127">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="f88f5-128">次の表に、macosscepcertificateprofile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-128">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="f88f5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f88f5-129">Property</span></span>|<span data-ttu-id="f88f5-130">型</span><span class="sxs-lookup"><span data-stu-id="f88f5-130">Type</span></span>|<span data-ttu-id="f88f5-131">説明</span><span class="sxs-lookup"><span data-stu-id="f88f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f88f5-132">id</span><span class="sxs-lookup"><span data-stu-id="f88f5-132">id</span></span>|<span data-ttu-id="f88f5-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f88f5-133">String</span></span>|<span data-ttu-id="f88f5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f88f5-134">Key of the entity.</span></span> <span data-ttu-id="f88f5-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f88f5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f88f5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f88f5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f88f5-137">DateTimeOffset</span></span>|<span data-ttu-id="f88f5-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f88f5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f88f5-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f88f5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f88f5-140">roleScopeTagIds</span></span>|<span data-ttu-id="f88f5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f88f5-141">String collection</span></span>|<span data-ttu-id="f88f5-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f88f5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f88f5-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f88f5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f88f5-144">supportsScopeTags</span></span>|<span data-ttu-id="f88f5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f88f5-145">Boolean</span></span>|<span data-ttu-id="f88f5-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f88f5-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f88f5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f88f5-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f88f5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f88f5-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-149">This property is read-only.</span></span> <span data-ttu-id="f88f5-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f88f5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f88f5-151">createdDateTime</span></span>|<span data-ttu-id="f88f5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f88f5-152">DateTimeOffset</span></span>|<span data-ttu-id="f88f5-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f88f5-153">DateTime the object was created.</span></span> <span data-ttu-id="f88f5-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f88f5-155">description</span><span class="sxs-lookup"><span data-stu-id="f88f5-155">description</span></span>|<span data-ttu-id="f88f5-156">String</span><span class="sxs-lookup"><span data-stu-id="f88f5-156">String</span></span>|<span data-ttu-id="f88f5-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f88f5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f88f5-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f88f5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f88f5-159">displayName</span></span>|<span data-ttu-id="f88f5-160">String</span><span class="sxs-lookup"><span data-stu-id="f88f5-160">String</span></span>|<span data-ttu-id="f88f5-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f88f5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f88f5-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f88f5-163">version</span><span class="sxs-lookup"><span data-stu-id="f88f5-163">version</span></span>|<span data-ttu-id="f88f5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f88f5-164">Int32</span></span>|<span data-ttu-id="f88f5-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f88f5-165">Version of the device configuration.</span></span> <span data-ttu-id="f88f5-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f88f5-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f88f5-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="f88f5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f88f5-168">Int32</span></span>|<span data-ttu-id="f88f5-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="f88f5-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f88f5-170">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f88f5-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f88f5-171">subjectNameFormat</span></span>|[<span data-ttu-id="f88f5-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f88f5-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="f88f5-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="f88f5-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="f88f5-174">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f88f5-175">可能な値は `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="f88f5-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f88f5-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f88f5-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f88f5-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f88f5-178">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="f88f5-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f88f5-179">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f88f5-180">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f88f5-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f88f5-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f88f5-182">Int32</span><span class="sxs-lookup"><span data-stu-id="f88f5-182">Int32</span></span>|<span data-ttu-id="f88f5-183">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="f88f5-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f88f5-184">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f88f5-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f88f5-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f88f5-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f88f5-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f88f5-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f88f5-187">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="f88f5-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f88f5-188">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f88f5-189">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f88f5-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f88f5-190">scepServerUrls</span></span>|<span data-ttu-id="f88f5-191">String collection</span><span class="sxs-lookup"><span data-stu-id="f88f5-191">String collection</span></span>|<span data-ttu-id="f88f5-192">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="f88f5-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f88f5-193">subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="f88f5-193">subjectNameFormatString</span></span>|<span data-ttu-id="f88f5-194">String</span><span class="sxs-lookup"><span data-stu-id="f88f5-194">String</span></span>|<span data-ttu-id="f88f5-195">SubjectNameFormat = custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="f88f5-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f88f5-196">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="f88f5-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f88f5-197">keyusage</span><span class="sxs-lookup"><span data-stu-id="f88f5-197">keyUsage</span></span>|[<span data-ttu-id="f88f5-198">keyusages</span><span class="sxs-lookup"><span data-stu-id="f88f5-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f88f5-199">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="f88f5-199">SCEP Key Usage.</span></span> <span data-ttu-id="f88f5-200">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f88f5-201">keySize</span><span class="sxs-lookup"><span data-stu-id="f88f5-201">keySize</span></span>|[<span data-ttu-id="f88f5-202">keySize</span><span class="sxs-lookup"><span data-stu-id="f88f5-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f88f5-203">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="f88f5-203">SCEP Key Size.</span></span> <span data-ttu-id="f88f5-204">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f88f5-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f88f5-205">hashAlgorithm</span></span>|[<span data-ttu-id="f88f5-206">hashalgorithms</span><span class="sxs-lookup"><span data-stu-id="f88f5-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f88f5-207">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="f88f5-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f88f5-208">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f88f5-209">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="f88f5-209">extendedKeyUsages</span></span>|<span data-ttu-id="f88f5-210">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f88f5-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f88f5-211">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="f88f5-211">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f88f5-212">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f88f5-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f88f5-213">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f88f5-213">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f88f5-214">String</span><span class="sxs-lookup"><span data-stu-id="f88f5-214">String</span></span>|<span data-ttu-id="f88f5-215">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="f88f5-215">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f88f5-216">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f88f5-216">certificateStore</span></span>|[<span data-ttu-id="f88f5-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f88f5-217">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f88f5-218">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="f88f5-218">Target store certificate.</span></span> <span data-ttu-id="f88f5-219">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-219">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f88f5-220">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f88f5-220">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f88f5-221">[customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="f88f5-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f88f5-222">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="f88f5-222">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f88f5-223">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f88f5-223">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f88f5-224">応答</span><span class="sxs-lookup"><span data-stu-id="f88f5-224">Response</span></span>
<span data-ttu-id="f88f5-225">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macosscepcertificateprofile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f88f5-225">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f88f5-226">例</span><span class="sxs-lookup"><span data-stu-id="f88f5-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="f88f5-227">要求</span><span class="sxs-lookup"><span data-stu-id="f88f5-227">Request</span></span>
<span data-ttu-id="f88f5-228">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f88f5-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="f88f5-229">応答</span><span class="sxs-lookup"><span data-stu-id="f88f5-229">Response</span></span>
<span data-ttu-id="f88f5-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f88f5-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

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




