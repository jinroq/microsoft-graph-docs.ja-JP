---
title: androidForWorkPkcsCertificateProfile の更新
description: androidForWorkPkcsCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2b0c108915c9af848aed5040cc39f14cd654e0e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806805"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="49878-103">androidForWorkPkcsCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="49878-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="49878-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49878-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49878-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49878-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49878-106">[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="49878-106">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49878-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="49878-107">Prerequisites</span></span>
<span data-ttu-id="49878-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49878-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49878-110">Permission type</span></span>|<span data-ttu-id="49878-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="49878-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49878-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49878-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49878-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49878-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49878-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49878-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49878-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49878-115">Not supported.</span></span>|
|<span data-ttu-id="49878-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49878-116">Application</span></span>|<span data-ttu-id="49878-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49878-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49878-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49878-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="49878-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49878-119">Request headers</span></span>
|<span data-ttu-id="49878-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49878-120">Header</span></span>|<span data-ttu-id="49878-121">値</span><span class="sxs-lookup"><span data-stu-id="49878-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49878-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49878-122">Authorization</span></span>|<span data-ttu-id="49878-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="49878-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49878-124">承諾</span><span class="sxs-lookup"><span data-stu-id="49878-124">Accept</span></span>|<span data-ttu-id="49878-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49878-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49878-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="49878-126">Request body</span></span>
<span data-ttu-id="49878-127">要求本文で、 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="49878-127">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="49878-128">次の表に、 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="49878-128">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="49878-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49878-129">Property</span></span>|<span data-ttu-id="49878-130">型</span><span class="sxs-lookup"><span data-stu-id="49878-130">Type</span></span>|<span data-ttu-id="49878-131">説明</span><span class="sxs-lookup"><span data-stu-id="49878-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49878-132">id</span><span class="sxs-lookup"><span data-stu-id="49878-132">id</span></span>|<span data-ttu-id="49878-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="49878-133">String</span></span>|<span data-ttu-id="49878-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="49878-134">Key of the entity.</span></span> <span data-ttu-id="49878-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49878-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49878-136">lastModifiedDateTime</span></span>|<span data-ttu-id="49878-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49878-137">DateTimeOffset</span></span>|<span data-ttu-id="49878-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="49878-138">DateTime the object was last modified.</span></span> <span data-ttu-id="49878-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49878-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49878-140">roleScopeTagIds</span></span>|<span data-ttu-id="49878-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="49878-141">String collection</span></span>|<span data-ttu-id="49878-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="49878-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="49878-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49878-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="49878-144">supportsScopeTags</span></span>|<span data-ttu-id="49878-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="49878-145">Boolean</span></span>|<span data-ttu-id="49878-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="49878-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="49878-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="49878-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="49878-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="49878-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="49878-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="49878-149">This property is read-only.</span></span> <span data-ttu-id="49878-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49878-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49878-151">createdDateTime</span></span>|<span data-ttu-id="49878-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49878-152">DateTimeOffset</span></span>|<span data-ttu-id="49878-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="49878-153">DateTime the object was created.</span></span> <span data-ttu-id="49878-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49878-155">説明</span><span class="sxs-lookup"><span data-stu-id="49878-155">description</span></span>|<span data-ttu-id="49878-156">String</span><span class="sxs-lookup"><span data-stu-id="49878-156">String</span></span>|<span data-ttu-id="49878-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="49878-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49878-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49878-159">displayName</span><span class="sxs-lookup"><span data-stu-id="49878-159">displayName</span></span>|<span data-ttu-id="49878-160">String</span><span class="sxs-lookup"><span data-stu-id="49878-160">String</span></span>|<span data-ttu-id="49878-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="49878-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49878-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49878-163">version</span><span class="sxs-lookup"><span data-stu-id="49878-163">version</span></span>|<span data-ttu-id="49878-164">Int32</span><span class="sxs-lookup"><span data-stu-id="49878-164">Int32</span></span>|<span data-ttu-id="49878-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="49878-165">Version of the device configuration.</span></span> <span data-ttu-id="49878-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49878-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="49878-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="49878-168">Int32</span><span class="sxs-lookup"><span data-stu-id="49878-168">Int32</span></span>|<span data-ttu-id="49878-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="49878-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="49878-170">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承された有効な値 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="49878-170">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="49878-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="49878-171">subjectNameFormat</span></span>|[<span data-ttu-id="49878-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="49878-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="49878-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="49878-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="49878-174">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="49878-174">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="49878-175">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="49878-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="49878-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="49878-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="49878-177">Int32</span><span class="sxs-lookup"><span data-stu-id="49878-177">Int32</span></span>|<span data-ttu-id="49878-178">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="49878-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="49878-179">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-179">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="49878-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="49878-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="49878-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="49878-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="49878-182">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="49878-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="49878-183">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="49878-183">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="49878-184">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="49878-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="49878-185">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="49878-185">extendedKeyUsages</span></span>|<span data-ttu-id="49878-186">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="49878-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="49878-187">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="49878-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="49878-188">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="49878-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="49878-189">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="49878-189">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="49878-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="49878-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="49878-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="49878-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="49878-192">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="49878-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="49878-193">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="49878-193">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="49878-194">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="49878-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="49878-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="49878-195">certificationAuthority</span></span>|<span data-ttu-id="49878-196">文字列</span><span class="sxs-lookup"><span data-stu-id="49878-196">String</span></span>|<span data-ttu-id="49878-197">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="49878-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="49878-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="49878-198">certificationAuthorityName</span></span>|<span data-ttu-id="49878-199">文字列</span><span class="sxs-lookup"><span data-stu-id="49878-199">String</span></span>|<span data-ttu-id="49878-200">PKCS 証明機関名</span><span class="sxs-lookup"><span data-stu-id="49878-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="49878-201">certificatetemplatename</span><span class="sxs-lookup"><span data-stu-id="49878-201">certificateTemplateName</span></span>|<span data-ttu-id="49878-202">文字列</span><span class="sxs-lookup"><span data-stu-id="49878-202">String</span></span>|<span data-ttu-id="49878-203">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="49878-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="49878-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="49878-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="49878-205">文字列</span><span class="sxs-lookup"><span data-stu-id="49878-205">String</span></span>|<span data-ttu-id="49878-206">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="49878-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="49878-207">応答</span><span class="sxs-lookup"><span data-stu-id="49878-207">Response</span></span>
<span data-ttu-id="49878-208">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="49878-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49878-209">例</span><span class="sxs-lookup"><span data-stu-id="49878-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="49878-210">要求</span><span class="sxs-lookup"><span data-stu-id="49878-210">Request</span></span>
<span data-ttu-id="49878-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="49878-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 965

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="49878-212">応答</span><span class="sxs-lookup"><span data-stu-id="49878-212">Response</span></span>
<span data-ttu-id="49878-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="49878-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





