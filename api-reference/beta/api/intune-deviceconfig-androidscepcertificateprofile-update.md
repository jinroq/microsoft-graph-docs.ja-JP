---
title: androidScepCertificateProfile の更新
description: androidScepCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55ab824a44f567946f4f7f7ee1dedcedada2e76a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799686"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="629ca-103">androidScepCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="629ca-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="629ca-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="629ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="629ca-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="629ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="629ca-106">[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="629ca-106">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="629ca-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="629ca-107">Prerequisites</span></span>
<span data-ttu-id="629ca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="629ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="629ca-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="629ca-110">Permission type</span></span>|<span data-ttu-id="629ca-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="629ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="629ca-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="629ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="629ca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629ca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="629ca-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="629ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="629ca-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="629ca-115">Not supported.</span></span>|
|<span data-ttu-id="629ca-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="629ca-116">Application</span></span>|<span data-ttu-id="629ca-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="629ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="629ca-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="629ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="629ca-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="629ca-119">Request headers</span></span>
|<span data-ttu-id="629ca-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="629ca-120">Header</span></span>|<span data-ttu-id="629ca-121">値</span><span class="sxs-lookup"><span data-stu-id="629ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="629ca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="629ca-122">Authorization</span></span>|<span data-ttu-id="629ca-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="629ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="629ca-124">承諾</span><span class="sxs-lookup"><span data-stu-id="629ca-124">Accept</span></span>|<span data-ttu-id="629ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="629ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="629ca-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="629ca-126">Request body</span></span>
<span data-ttu-id="629ca-127">要求本文で、 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="629ca-127">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="629ca-128">次の表に、 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="629ca-128">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="629ca-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="629ca-129">Property</span></span>|<span data-ttu-id="629ca-130">型</span><span class="sxs-lookup"><span data-stu-id="629ca-130">Type</span></span>|<span data-ttu-id="629ca-131">説明</span><span class="sxs-lookup"><span data-stu-id="629ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="629ca-132">id</span><span class="sxs-lookup"><span data-stu-id="629ca-132">id</span></span>|<span data-ttu-id="629ca-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="629ca-133">String</span></span>|<span data-ttu-id="629ca-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="629ca-134">Key of the entity.</span></span> <span data-ttu-id="629ca-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="629ca-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="629ca-136">lastModifiedDateTime</span></span>|<span data-ttu-id="629ca-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="629ca-137">DateTimeOffset</span></span>|<span data-ttu-id="629ca-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="629ca-138">DateTime the object was last modified.</span></span> <span data-ttu-id="629ca-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="629ca-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="629ca-140">roleScopeTagIds</span></span>|<span data-ttu-id="629ca-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="629ca-141">String collection</span></span>|<span data-ttu-id="629ca-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="629ca-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="629ca-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="629ca-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="629ca-144">supportsScopeTags</span></span>|<span data-ttu-id="629ca-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="629ca-145">Boolean</span></span>|<span data-ttu-id="629ca-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="629ca-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="629ca-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="629ca-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="629ca-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="629ca-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="629ca-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="629ca-149">This property is read-only.</span></span> <span data-ttu-id="629ca-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="629ca-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="629ca-151">createdDateTime</span></span>|<span data-ttu-id="629ca-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="629ca-152">DateTimeOffset</span></span>|<span data-ttu-id="629ca-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="629ca-153">DateTime the object was created.</span></span> <span data-ttu-id="629ca-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="629ca-155">説明</span><span class="sxs-lookup"><span data-stu-id="629ca-155">description</span></span>|<span data-ttu-id="629ca-156">String</span><span class="sxs-lookup"><span data-stu-id="629ca-156">String</span></span>|<span data-ttu-id="629ca-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="629ca-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="629ca-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="629ca-159">displayName</span><span class="sxs-lookup"><span data-stu-id="629ca-159">displayName</span></span>|<span data-ttu-id="629ca-160">String</span><span class="sxs-lookup"><span data-stu-id="629ca-160">String</span></span>|<span data-ttu-id="629ca-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="629ca-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="629ca-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="629ca-163">version</span><span class="sxs-lookup"><span data-stu-id="629ca-163">version</span></span>|<span data-ttu-id="629ca-164">Int32</span><span class="sxs-lookup"><span data-stu-id="629ca-164">Int32</span></span>|<span data-ttu-id="629ca-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="629ca-165">Version of the device configuration.</span></span> <span data-ttu-id="629ca-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="629ca-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="629ca-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="629ca-168">Int32</span><span class="sxs-lookup"><span data-stu-id="629ca-168">Int32</span></span>|<span data-ttu-id="629ca-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="629ca-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="629ca-170">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="629ca-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="629ca-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="629ca-171">subjectNameFormat</span></span>|[<span data-ttu-id="629ca-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="629ca-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="629ca-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="629ca-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="629ca-174">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="629ca-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="629ca-175">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="629ca-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="629ca-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="629ca-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="629ca-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="629ca-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="629ca-178">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="629ca-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="629ca-179">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="629ca-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="629ca-180">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="629ca-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="629ca-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="629ca-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="629ca-182">Int32</span><span class="sxs-lookup"><span data-stu-id="629ca-182">Int32</span></span>|<span data-ttu-id="629ca-183">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="629ca-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="629ca-184">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="629ca-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="629ca-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="629ca-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="629ca-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="629ca-187">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="629ca-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="629ca-188">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="629ca-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="629ca-189">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="629ca-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="629ca-190">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="629ca-190">extendedKeyUsages</span></span>|<span data-ttu-id="629ca-191">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="629ca-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="629ca-192">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="629ca-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="629ca-193">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="629ca-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="629ca-194">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="629ca-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="629ca-195">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="629ca-195">scepServerUrls</span></span>|<span data-ttu-id="629ca-196">String コレクション</span><span class="sxs-lookup"><span data-stu-id="629ca-196">String collection</span></span>|<span data-ttu-id="629ca-197">SCEP サーバーの Url</span><span class="sxs-lookup"><span data-stu-id="629ca-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="629ca-198">subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="629ca-198">subjectNameFormatString</span></span>|<span data-ttu-id="629ca-199">文字列</span><span class="sxs-lookup"><span data-stu-id="629ca-199">String</span></span>|<span data-ttu-id="629ca-200">SubjectNameFormat = custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="629ca-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="629ca-201">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="629ca-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="629ca-202">keyusage</span><span class="sxs-lookup"><span data-stu-id="629ca-202">keyUsage</span></span>|[<span data-ttu-id="629ca-203">keyusages</span><span class="sxs-lookup"><span data-stu-id="629ca-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="629ca-204">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="629ca-204">SCEP Key Usage.</span></span> <span data-ttu-id="629ca-205">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="629ca-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="629ca-206">keySize</span><span class="sxs-lookup"><span data-stu-id="629ca-206">keySize</span></span>|[<span data-ttu-id="629ca-207">keySize</span><span class="sxs-lookup"><span data-stu-id="629ca-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="629ca-208">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="629ca-208">SCEP Key Size.</span></span> <span data-ttu-id="629ca-209">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="629ca-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="629ca-210">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="629ca-210">hashAlgorithm</span></span>|[<span data-ttu-id="629ca-211">hashalgorithms</span><span class="sxs-lookup"><span data-stu-id="629ca-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="629ca-212">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="629ca-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="629ca-213">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="629ca-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="629ca-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="629ca-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="629ca-215">文字列</span><span class="sxs-lookup"><span data-stu-id="629ca-215">String</span></span>|<span data-ttu-id="629ca-216">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="629ca-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="629ca-217">応答</span><span class="sxs-lookup"><span data-stu-id="629ca-217">Response</span></span>
<span data-ttu-id="629ca-218">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="629ca-218">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="629ca-219">例</span><span class="sxs-lookup"><span data-stu-id="629ca-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="629ca-220">要求</span><span class="sxs-lookup"><span data-stu-id="629ca-220">Request</span></span>
<span data-ttu-id="629ca-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="629ca-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="629ca-222">応答</span><span class="sxs-lookup"><span data-stu-id="629ca-222">Response</span></span>
<span data-ttu-id="629ca-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="629ca-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





