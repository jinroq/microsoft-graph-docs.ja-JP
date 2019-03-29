---
title: androidForWorkScepCertificateProfile の更新
description: androidForWorkScepCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 073991efa53e39ac05bf1f40d87af7bad0d5d27e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974875"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="309ce-103">androidForWorkScepCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="309ce-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="309ce-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="309ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="309ce-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="309ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="309ce-106">[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="309ce-106">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="309ce-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="309ce-107">Prerequisites</span></span>
<span data-ttu-id="309ce-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="309ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="309ce-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="309ce-110">Permission type</span></span>|<span data-ttu-id="309ce-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="309ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="309ce-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="309ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="309ce-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="309ce-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="309ce-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="309ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="309ce-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="309ce-115">Not supported.</span></span>|
|<span data-ttu-id="309ce-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="309ce-116">Application</span></span>|<span data-ttu-id="309ce-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="309ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="309ce-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="309ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="309ce-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="309ce-119">Request headers</span></span>
|<span data-ttu-id="309ce-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="309ce-120">Header</span></span>|<span data-ttu-id="309ce-121">値</span><span class="sxs-lookup"><span data-stu-id="309ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="309ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="309ce-122">Authorization</span></span>|<span data-ttu-id="309ce-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="309ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="309ce-124">承諾</span><span class="sxs-lookup"><span data-stu-id="309ce-124">Accept</span></span>|<span data-ttu-id="309ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="309ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="309ce-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="309ce-126">Request body</span></span>
<span data-ttu-id="309ce-127">要求本文で、 [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="309ce-127">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="309ce-128">次の表に、 [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="309ce-128">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="309ce-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="309ce-129">Property</span></span>|<span data-ttu-id="309ce-130">型</span><span class="sxs-lookup"><span data-stu-id="309ce-130">Type</span></span>|<span data-ttu-id="309ce-131">説明</span><span class="sxs-lookup"><span data-stu-id="309ce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="309ce-132">id</span><span class="sxs-lookup"><span data-stu-id="309ce-132">id</span></span>|<span data-ttu-id="309ce-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="309ce-133">String</span></span>|<span data-ttu-id="309ce-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="309ce-134">Key of the entity.</span></span> <span data-ttu-id="309ce-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="309ce-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="309ce-136">lastModifiedDateTime</span></span>|<span data-ttu-id="309ce-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="309ce-137">DateTimeOffset</span></span>|<span data-ttu-id="309ce-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="309ce-138">DateTime the object was last modified.</span></span> <span data-ttu-id="309ce-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="309ce-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="309ce-140">roleScopeTagIds</span></span>|<span data-ttu-id="309ce-141">String collection</span><span class="sxs-lookup"><span data-stu-id="309ce-141">String collection</span></span>|<span data-ttu-id="309ce-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="309ce-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="309ce-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="309ce-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="309ce-144">supportsScopeTags</span></span>|<span data-ttu-id="309ce-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="309ce-145">Boolean</span></span>|<span data-ttu-id="309ce-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="309ce-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="309ce-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="309ce-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="309ce-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="309ce-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="309ce-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="309ce-149">This property is read-only.</span></span> <span data-ttu-id="309ce-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="309ce-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="309ce-151">createdDateTime</span></span>|<span data-ttu-id="309ce-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="309ce-152">DateTimeOffset</span></span>|<span data-ttu-id="309ce-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="309ce-153">DateTime the object was created.</span></span> <span data-ttu-id="309ce-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="309ce-155">description</span><span class="sxs-lookup"><span data-stu-id="309ce-155">description</span></span>|<span data-ttu-id="309ce-156">String</span><span class="sxs-lookup"><span data-stu-id="309ce-156">String</span></span>|<span data-ttu-id="309ce-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="309ce-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="309ce-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="309ce-159">displayName</span><span class="sxs-lookup"><span data-stu-id="309ce-159">displayName</span></span>|<span data-ttu-id="309ce-160">String</span><span class="sxs-lookup"><span data-stu-id="309ce-160">String</span></span>|<span data-ttu-id="309ce-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="309ce-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="309ce-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="309ce-163">version</span><span class="sxs-lookup"><span data-stu-id="309ce-163">version</span></span>|<span data-ttu-id="309ce-164">Int32</span><span class="sxs-lookup"><span data-stu-id="309ce-164">Int32</span></span>|<span data-ttu-id="309ce-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="309ce-165">Version of the device configuration.</span></span> <span data-ttu-id="309ce-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="309ce-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="309ce-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="309ce-168">Int32</span><span class="sxs-lookup"><span data-stu-id="309ce-168">Int32</span></span>|<span data-ttu-id="309ce-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="309ce-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="309ce-170">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承された有効な値 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="309ce-170">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="309ce-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="309ce-171">subjectNameFormat</span></span>|[<span data-ttu-id="309ce-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="309ce-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="309ce-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="309ce-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="309ce-174">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="309ce-174">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="309ce-175">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="309ce-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="309ce-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="309ce-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="309ce-177">Int32</span><span class="sxs-lookup"><span data-stu-id="309ce-177">Int32</span></span>|<span data-ttu-id="309ce-178">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="309ce-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="309ce-179">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-179">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="309ce-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="309ce-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="309ce-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="309ce-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="309ce-182">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="309ce-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="309ce-183">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="309ce-183">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="309ce-184">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="309ce-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="309ce-185">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="309ce-185">extendedKeyUsages</span></span>|<span data-ttu-id="309ce-186">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="309ce-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="309ce-187">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="309ce-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="309ce-188">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="309ce-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="309ce-189">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="309ce-189">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="309ce-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="309ce-190">scepServerUrls</span></span>|<span data-ttu-id="309ce-191">String collection</span><span class="sxs-lookup"><span data-stu-id="309ce-191">String collection</span></span>|<span data-ttu-id="309ce-192">SCEP サーバーの Url</span><span class="sxs-lookup"><span data-stu-id="309ce-192">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="309ce-193">subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="309ce-193">subjectNameFormatString</span></span>|<span data-ttu-id="309ce-194">String</span><span class="sxs-lookup"><span data-stu-id="309ce-194">String</span></span>|<span data-ttu-id="309ce-195">SubjectNameFormat = custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="309ce-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="309ce-196">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="309ce-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="309ce-197">keyusage</span><span class="sxs-lookup"><span data-stu-id="309ce-197">keyUsage</span></span>|[<span data-ttu-id="309ce-198">keyusages</span><span class="sxs-lookup"><span data-stu-id="309ce-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="309ce-199">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="309ce-199">SCEP Key Usage.</span></span> <span data-ttu-id="309ce-200">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="309ce-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="309ce-201">keySize</span><span class="sxs-lookup"><span data-stu-id="309ce-201">keySize</span></span>|[<span data-ttu-id="309ce-202">keySize</span><span class="sxs-lookup"><span data-stu-id="309ce-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="309ce-203">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="309ce-203">SCEP Key Size.</span></span> <span data-ttu-id="309ce-204">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="309ce-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="309ce-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="309ce-205">hashAlgorithm</span></span>|[<span data-ttu-id="309ce-206">hashalgorithms</span><span class="sxs-lookup"><span data-stu-id="309ce-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="309ce-207">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="309ce-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="309ce-208">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="309ce-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="309ce-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="309ce-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="309ce-210">String</span><span class="sxs-lookup"><span data-stu-id="309ce-210">String</span></span>|<span data-ttu-id="309ce-211">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="309ce-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="309ce-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="309ce-212">certificateStore</span></span>|[<span data-ttu-id="309ce-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="309ce-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="309ce-214">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="309ce-214">Target store certificate.</span></span> <span data-ttu-id="309ce-215">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="309ce-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="309ce-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="309ce-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="309ce-217">[customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="309ce-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="309ce-218">カスタムの Subject Alterantive Name 設定。</span><span class="sxs-lookup"><span data-stu-id="309ce-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="309ce-219">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="309ce-219">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="309ce-220">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="309ce-220">subjectAlternativeNameType</span></span>|[<span data-ttu-id="309ce-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="309ce-221">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="309ce-222">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="309ce-222">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="309ce-223">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="309ce-223">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="309ce-224">応答</span><span class="sxs-lookup"><span data-stu-id="309ce-224">Response</span></span>
<span data-ttu-id="309ce-225">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="309ce-225">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="309ce-226">例</span><span class="sxs-lookup"><span data-stu-id="309ce-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="309ce-227">要求</span><span class="sxs-lookup"><span data-stu-id="309ce-227">Request</span></span>
<span data-ttu-id="309ce-228">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="309ce-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1205

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="309ce-229">応答</span><span class="sxs-lookup"><span data-stu-id="309ce-229">Response</span></span>
<span data-ttu-id="309ce-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="309ce-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```




