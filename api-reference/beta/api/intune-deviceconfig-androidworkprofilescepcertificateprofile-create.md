---
title: Androidwork プロファイル Cepcertificateprofile の作成
description: 新しい Androidwork プロファイル Cepcertificateprofile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5ecd1806cd1797c6d5a79c34270c7b8db9a8893
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928324"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="869e6-103">Androidwork プロファイル Cepcertificateprofile の作成</span><span class="sxs-lookup"><span data-stu-id="869e6-103">Create androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="869e6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="869e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="869e6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="869e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="869e6-106">新しい[Androidwork プロファイル Cepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="869e6-106">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="869e6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="869e6-107">Prerequisites</span></span>
<span data-ttu-id="869e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="869e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="869e6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="869e6-110">Permission type</span></span>|<span data-ttu-id="869e6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="869e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="869e6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="869e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="869e6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="869e6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="869e6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="869e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="869e6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="869e6-115">Not supported.</span></span>|
|<span data-ttu-id="869e6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="869e6-116">Application</span></span>|<span data-ttu-id="869e6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="869e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="869e6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="869e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="869e6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="869e6-119">Request headers</span></span>
|<span data-ttu-id="869e6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="869e6-120">Header</span></span>|<span data-ttu-id="869e6-121">値</span><span class="sxs-lookup"><span data-stu-id="869e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="869e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="869e6-122">Authorization</span></span>|<span data-ttu-id="869e6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="869e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="869e6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="869e6-124">Accept</span></span>|<span data-ttu-id="869e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="869e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="869e6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="869e6-126">Request body</span></span>
<span data-ttu-id="869e6-127">要求本文で、Androidwork プロファイル Cepcertificateprofile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="869e6-127">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="869e6-128">次の表に、Androidwork プロファイル Cepcertificateprofile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="869e6-128">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="869e6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="869e6-129">Property</span></span>|<span data-ttu-id="869e6-130">型</span><span class="sxs-lookup"><span data-stu-id="869e6-130">Type</span></span>|<span data-ttu-id="869e6-131">説明</span><span class="sxs-lookup"><span data-stu-id="869e6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="869e6-132">id</span><span class="sxs-lookup"><span data-stu-id="869e6-132">id</span></span>|<span data-ttu-id="869e6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="869e6-133">String</span></span>|<span data-ttu-id="869e6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="869e6-134">Key of the entity.</span></span> <span data-ttu-id="869e6-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869e6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="869e6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="869e6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="869e6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869e6-137">DateTimeOffset</span></span>|<span data-ttu-id="869e6-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="869e6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="869e6-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869e6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="869e6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="869e6-140">roleScopeTagIds</span></span>|<span data-ttu-id="869e6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="869e6-141">String collection</span></span>|<span data-ttu-id="869e6-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="869e6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="869e6-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869e6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="869e6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="869e6-144">supportsScopeTags</span></span>|<span data-ttu-id="869e6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="869e6-145">Boolean</span></span>|<span data-ttu-id="869e6-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="869e6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="869e6-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="869e6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="869e6-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="869e6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="869e6-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="869e6-149">This property is read-only.</span></span> <span data-ttu-id="869e6-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869e6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="869e6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="869e6-151">createdDateTime</span></span>|<span data-ttu-id="869e6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869e6-152">DateTimeOffset</span></span>|<span data-ttu-id="869e6-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="869e6-153">DateTime the object was created.</span></span> <span data-ttu-id="869e6-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869e6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="869e6-155">description</span><span class="sxs-lookup"><span data-stu-id="869e6-155">description</span></span>|<span data-ttu-id="869e6-156">String</span><span class="sxs-lookup"><span data-stu-id="869e6-156">String</span></span>|<span data-ttu-id="869e6-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="869e6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="869e6-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869e6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="869e6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="869e6-159">displayName</span></span>|<span data-ttu-id="869e6-160">String</span><span class="sxs-lookup"><span data-stu-id="869e6-160">String</span></span>|<span data-ttu-id="869e6-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="869e6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="869e6-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869e6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="869e6-163">version</span><span class="sxs-lookup"><span data-stu-id="869e6-163">version</span></span>|<span data-ttu-id="869e6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="869e6-164">Int32</span></span>|<span data-ttu-id="869e6-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="869e6-165">Version of the device configuration.</span></span> <span data-ttu-id="869e6-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869e6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="869e6-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="869e6-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="869e6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="869e6-168">Int32</span></span>|<span data-ttu-id="869e6-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="869e6-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="869e6-170">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承された有効な値 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="869e6-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="869e6-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="869e6-171">subjectNameFormat</span></span>|[<span data-ttu-id="869e6-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="869e6-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="869e6-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="869e6-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="869e6-174">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="869e6-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="869e6-175">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="869e6-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="869e6-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="869e6-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="869e6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="869e6-177">Int32</span></span>|<span data-ttu-id="869e6-178">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="869e6-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="869e6-179">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="869e6-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="869e6-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="869e6-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="869e6-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="869e6-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="869e6-182">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="869e6-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="869e6-183">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="869e6-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="869e6-184">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="869e6-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="869e6-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="869e6-185">extendedKeyUsages</span></span>|<span data-ttu-id="869e6-186">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="869e6-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="869e6-187">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="869e6-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="869e6-188">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="869e6-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="869e6-189">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="869e6-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="869e6-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="869e6-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="869e6-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="869e6-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="869e6-192">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="869e6-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="869e6-193">[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="869e6-193">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="869e6-194">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="869e6-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="869e6-195">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="869e6-195">scepServerUrls</span></span>|<span data-ttu-id="869e6-196">String collection</span><span class="sxs-lookup"><span data-stu-id="869e6-196">String collection</span></span>|<span data-ttu-id="869e6-197">SCEP サーバーの Url</span><span class="sxs-lookup"><span data-stu-id="869e6-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="869e6-198">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="869e6-198">subjectNameFormatString</span></span>|<span data-ttu-id="869e6-199">String</span><span class="sxs-lookup"><span data-stu-id="869e6-199">String</span></span>|<span data-ttu-id="869e6-200">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="869e6-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="869e6-201">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="869e6-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="869e6-202">keyUsage</span><span class="sxs-lookup"><span data-stu-id="869e6-202">keyUsage</span></span>|[<span data-ttu-id="869e6-203">keyUsages</span><span class="sxs-lookup"><span data-stu-id="869e6-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="869e6-204">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="869e6-204">SCEP Key Usage.</span></span> <span data-ttu-id="869e6-205">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="869e6-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="869e6-206">keySize</span><span class="sxs-lookup"><span data-stu-id="869e6-206">keySize</span></span>|[<span data-ttu-id="869e6-207">keySize</span><span class="sxs-lookup"><span data-stu-id="869e6-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="869e6-208">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="869e6-208">SCEP Key Size.</span></span> <span data-ttu-id="869e6-209">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="869e6-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="869e6-210">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="869e6-210">hashAlgorithm</span></span>|[<span data-ttu-id="869e6-211">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="869e6-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="869e6-212">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="869e6-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="869e6-213">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="869e6-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="869e6-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="869e6-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="869e6-215">String</span><span class="sxs-lookup"><span data-stu-id="869e6-215">String</span></span>|<span data-ttu-id="869e6-216">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="869e6-216">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="869e6-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="869e6-217">certificateStore</span></span>|[<span data-ttu-id="869e6-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="869e6-218">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="869e6-219">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="869e6-219">Target store certificate.</span></span> <span data-ttu-id="869e6-220">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="869e6-220">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="869e6-221">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="869e6-221">customSubjectAlternativeNames</span></span>|<span data-ttu-id="869e6-222">[Customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="869e6-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="869e6-223">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="869e6-223">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="869e6-224">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="869e6-224">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="869e6-225">応答</span><span class="sxs-lookup"><span data-stu-id="869e6-225">Response</span></span>
<span data-ttu-id="869e6-226">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androidwork プロファイル cepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="869e6-226">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="869e6-227">例</span><span class="sxs-lookup"><span data-stu-id="869e6-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="869e6-228">要求</span><span class="sxs-lookup"><span data-stu-id="869e6-228">Request</span></span>
<span data-ttu-id="869e6-229">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="869e6-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
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
  "subjectAlternativeNameType": "emailAddress",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="869e6-230">応答</span><span class="sxs-lookup"><span data-stu-id="869e6-230">Response</span></span>
<span data-ttu-id="869e6-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="869e6-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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
  "subjectAlternativeNameType": "emailAddress",
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
  ]
}
```




