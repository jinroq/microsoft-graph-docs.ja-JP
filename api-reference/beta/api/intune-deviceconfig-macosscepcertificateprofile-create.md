---
title: macosscepcertificateprofile の作成
description: 新しい macosscepcertificateprofile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc2f24a37c3c4cda0efbff722b771aa097975963
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776487"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="90aaa-103">macosscepcertificateprofile の作成</span><span class="sxs-lookup"><span data-stu-id="90aaa-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="90aaa-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90aaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90aaa-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90aaa-106">新しい[macosscepcertificateprofile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-106">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90aaa-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="90aaa-107">Prerequisites</span></span>
<span data-ttu-id="90aaa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90aaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90aaa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90aaa-110">Permission type</span></span>|<span data-ttu-id="90aaa-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="90aaa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90aaa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90aaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90aaa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90aaa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90aaa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90aaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90aaa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90aaa-115">Not supported.</span></span>|
|<span data-ttu-id="90aaa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90aaa-116">Application</span></span>|<span data-ttu-id="90aaa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90aaa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90aaa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90aaa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90aaa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90aaa-119">Request headers</span></span>
|<span data-ttu-id="90aaa-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90aaa-120">Header</span></span>|<span data-ttu-id="90aaa-121">値</span><span class="sxs-lookup"><span data-stu-id="90aaa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90aaa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90aaa-122">Authorization</span></span>|<span data-ttu-id="90aaa-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90aaa-124">承諾</span><span class="sxs-lookup"><span data-stu-id="90aaa-124">Accept</span></span>|<span data-ttu-id="90aaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90aaa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90aaa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="90aaa-126">Request body</span></span>
<span data-ttu-id="90aaa-127">要求本文で、macosscepcertificateprofile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-127">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="90aaa-128">次の表に、macosscepcertificateprofile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-128">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="90aaa-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90aaa-129">Property</span></span>|<span data-ttu-id="90aaa-130">型</span><span class="sxs-lookup"><span data-stu-id="90aaa-130">Type</span></span>|<span data-ttu-id="90aaa-131">説明</span><span class="sxs-lookup"><span data-stu-id="90aaa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90aaa-132">id</span><span class="sxs-lookup"><span data-stu-id="90aaa-132">id</span></span>|<span data-ttu-id="90aaa-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="90aaa-133">String</span></span>|<span data-ttu-id="90aaa-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="90aaa-134">Key of the entity.</span></span> <span data-ttu-id="90aaa-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90aaa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90aaa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="90aaa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90aaa-137">DateTimeOffset</span></span>|<span data-ttu-id="90aaa-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="90aaa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="90aaa-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90aaa-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90aaa-140">roleScopeTagIds</span></span>|<span data-ttu-id="90aaa-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="90aaa-141">String collection</span></span>|<span data-ttu-id="90aaa-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="90aaa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="90aaa-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90aaa-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="90aaa-144">supportsScopeTags</span></span>|<span data-ttu-id="90aaa-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="90aaa-145">Boolean</span></span>|<span data-ttu-id="90aaa-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="90aaa-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="90aaa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="90aaa-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="90aaa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="90aaa-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-149">This property is read-only.</span></span> <span data-ttu-id="90aaa-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90aaa-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90aaa-151">createdDateTime</span></span>|<span data-ttu-id="90aaa-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90aaa-152">DateTimeOffset</span></span>|<span data-ttu-id="90aaa-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="90aaa-153">DateTime the object was created.</span></span> <span data-ttu-id="90aaa-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90aaa-155">説明</span><span class="sxs-lookup"><span data-stu-id="90aaa-155">description</span></span>|<span data-ttu-id="90aaa-156">String</span><span class="sxs-lookup"><span data-stu-id="90aaa-156">String</span></span>|<span data-ttu-id="90aaa-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="90aaa-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90aaa-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90aaa-159">displayName</span><span class="sxs-lookup"><span data-stu-id="90aaa-159">displayName</span></span>|<span data-ttu-id="90aaa-160">String</span><span class="sxs-lookup"><span data-stu-id="90aaa-160">String</span></span>|<span data-ttu-id="90aaa-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="90aaa-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90aaa-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90aaa-163">version</span><span class="sxs-lookup"><span data-stu-id="90aaa-163">version</span></span>|<span data-ttu-id="90aaa-164">Int32</span><span class="sxs-lookup"><span data-stu-id="90aaa-164">Int32</span></span>|<span data-ttu-id="90aaa-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="90aaa-165">Version of the device configuration.</span></span> <span data-ttu-id="90aaa-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90aaa-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="90aaa-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="90aaa-168">Int32</span><span class="sxs-lookup"><span data-stu-id="90aaa-168">Int32</span></span>|<span data-ttu-id="90aaa-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="90aaa-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="90aaa-170">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="90aaa-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="90aaa-171">subjectNameFormat</span></span>|[<span data-ttu-id="90aaa-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="90aaa-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="90aaa-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="90aaa-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="90aaa-174">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="90aaa-175">可能な値は `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="90aaa-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="90aaa-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="90aaa-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="90aaa-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="90aaa-178">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="90aaa-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="90aaa-179">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="90aaa-180">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="90aaa-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="90aaa-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="90aaa-182">Int32</span><span class="sxs-lookup"><span data-stu-id="90aaa-182">Int32</span></span>|<span data-ttu-id="90aaa-183">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="90aaa-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="90aaa-184">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="90aaa-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="90aaa-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="90aaa-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="90aaa-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="90aaa-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="90aaa-187">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="90aaa-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="90aaa-188">[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="90aaa-189">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="90aaa-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="90aaa-190">scepServerUrls</span></span>|<span data-ttu-id="90aaa-191">String コレクション</span><span class="sxs-lookup"><span data-stu-id="90aaa-191">String collection</span></span>|<span data-ttu-id="90aaa-192">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="90aaa-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="90aaa-193">subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="90aaa-193">subjectNameFormatString</span></span>|<span data-ttu-id="90aaa-194">文字列</span><span class="sxs-lookup"><span data-stu-id="90aaa-194">String</span></span>|<span data-ttu-id="90aaa-195">SubjectNameFormat = custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="90aaa-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="90aaa-196">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="90aaa-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="90aaa-197">keyusage</span><span class="sxs-lookup"><span data-stu-id="90aaa-197">keyUsage</span></span>|[<span data-ttu-id="90aaa-198">keyusages</span><span class="sxs-lookup"><span data-stu-id="90aaa-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="90aaa-199">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="90aaa-199">SCEP Key Usage.</span></span> <span data-ttu-id="90aaa-200">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="90aaa-201">keySize</span><span class="sxs-lookup"><span data-stu-id="90aaa-201">keySize</span></span>|[<span data-ttu-id="90aaa-202">keySize</span><span class="sxs-lookup"><span data-stu-id="90aaa-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="90aaa-203">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="90aaa-203">SCEP Key Size.</span></span> <span data-ttu-id="90aaa-204">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="90aaa-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="90aaa-205">hashAlgorithm</span></span>|[<span data-ttu-id="90aaa-206">hashalgorithms</span><span class="sxs-lookup"><span data-stu-id="90aaa-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="90aaa-207">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="90aaa-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="90aaa-208">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="90aaa-209">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="90aaa-209">extendedKeyUsages</span></span>|<span data-ttu-id="90aaa-210">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="90aaa-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="90aaa-211">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="90aaa-211">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="90aaa-212">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="90aaa-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="90aaa-213">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="90aaa-213">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="90aaa-214">文字列</span><span class="sxs-lookup"><span data-stu-id="90aaa-214">String</span></span>|<span data-ttu-id="90aaa-215">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="90aaa-215">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="90aaa-216">certificateStore</span><span class="sxs-lookup"><span data-stu-id="90aaa-216">certificateStore</span></span>|[<span data-ttu-id="90aaa-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="90aaa-217">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="90aaa-218">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="90aaa-218">Target store certificate.</span></span> <span data-ttu-id="90aaa-219">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-219">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="90aaa-220">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="90aaa-220">customSubjectAlternativeNames</span></span>|<span data-ttu-id="90aaa-221">[customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="90aaa-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="90aaa-222">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="90aaa-222">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="90aaa-223">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="90aaa-223">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="90aaa-224">応答</span><span class="sxs-lookup"><span data-stu-id="90aaa-224">Response</span></span>
<span data-ttu-id="90aaa-225">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macosscepcertificateprofile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="90aaa-225">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90aaa-226">例</span><span class="sxs-lookup"><span data-stu-id="90aaa-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="90aaa-227">要求</span><span class="sxs-lookup"><span data-stu-id="90aaa-227">Request</span></span>
<span data-ttu-id="90aaa-228">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90aaa-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="90aaa-229">応答</span><span class="sxs-lookup"><span data-stu-id="90aaa-229">Response</span></span>
<span data-ttu-id="90aaa-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90aaa-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





