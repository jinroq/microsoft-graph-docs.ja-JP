---
title: androidForWorkPkcsCertificateProfile の更新
description: androidForWorkPkcsCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2b0c108915c9af848aed5040cc39f14cd654e0e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32478386"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="5bdc0-103">androidForWorkPkcsCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="5bdc0-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="5bdc0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bdc0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bdc0-106">[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-106">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bdc0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5bdc0-107">Prerequisites</span></span>
<span data-ttu-id="5bdc0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bdc0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5bdc0-110">Permission type</span></span>|<span data-ttu-id="5bdc0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5bdc0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bdc0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5bdc0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5bdc0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bdc0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5bdc0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bdc0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bdc0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-115">Not supported.</span></span>|
|<span data-ttu-id="5bdc0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5bdc0-116">Application</span></span>|<span data-ttu-id="5bdc0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bdc0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bdc0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5bdc0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bdc0-119">Request headers</span></span>
|<span data-ttu-id="5bdc0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bdc0-120">Header</span></span>|<span data-ttu-id="5bdc0-121">値</span><span class="sxs-lookup"><span data-stu-id="5bdc0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bdc0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bdc0-122">Authorization</span></span>|<span data-ttu-id="5bdc0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bdc0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5bdc0-124">Accept</span></span>|<span data-ttu-id="5bdc0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5bdc0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bdc0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bdc0-126">Request body</span></span>
<span data-ttu-id="5bdc0-127">要求本文で、 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-127">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="5bdc0-128">次の表に、 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-128">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="5bdc0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bdc0-129">Property</span></span>|<span data-ttu-id="5bdc0-130">型</span><span class="sxs-lookup"><span data-stu-id="5bdc0-130">Type</span></span>|<span data-ttu-id="5bdc0-131">説明</span><span class="sxs-lookup"><span data-stu-id="5bdc0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bdc0-132">id</span><span class="sxs-lookup"><span data-stu-id="5bdc0-132">id</span></span>|<span data-ttu-id="5bdc0-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5bdc0-133">String</span></span>|<span data-ttu-id="5bdc0-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-134">Key of the entity.</span></span> <span data-ttu-id="5bdc0-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5bdc0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bdc0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5bdc0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bdc0-137">DateTimeOffset</span></span>|<span data-ttu-id="5bdc0-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5bdc0-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5bdc0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5bdc0-140">roleScopeTagIds</span></span>|<span data-ttu-id="5bdc0-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5bdc0-141">String collection</span></span>|<span data-ttu-id="5bdc0-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5bdc0-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5bdc0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5bdc0-144">supportsScopeTags</span></span>|<span data-ttu-id="5bdc0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bdc0-145">Boolean</span></span>|<span data-ttu-id="5bdc0-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5bdc0-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5bdc0-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5bdc0-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-149">This property is read-only.</span></span> <span data-ttu-id="5bdc0-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5bdc0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bdc0-151">createdDateTime</span></span>|<span data-ttu-id="5bdc0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bdc0-152">DateTimeOffset</span></span>|<span data-ttu-id="5bdc0-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-153">DateTime the object was created.</span></span> <span data-ttu-id="5bdc0-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5bdc0-155">説明</span><span class="sxs-lookup"><span data-stu-id="5bdc0-155">description</span></span>|<span data-ttu-id="5bdc0-156">String</span><span class="sxs-lookup"><span data-stu-id="5bdc0-156">String</span></span>|<span data-ttu-id="5bdc0-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5bdc0-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5bdc0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5bdc0-159">displayName</span></span>|<span data-ttu-id="5bdc0-160">String</span><span class="sxs-lookup"><span data-stu-id="5bdc0-160">String</span></span>|<span data-ttu-id="5bdc0-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5bdc0-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5bdc0-163">version</span><span class="sxs-lookup"><span data-stu-id="5bdc0-163">version</span></span>|<span data-ttu-id="5bdc0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5bdc0-164">Int32</span></span>|<span data-ttu-id="5bdc0-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-165">Version of the device configuration.</span></span> <span data-ttu-id="5bdc0-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5bdc0-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5bdc0-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="5bdc0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5bdc0-168">Int32</span></span>|<span data-ttu-id="5bdc0-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5bdc0-170">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承された有効な値 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="5bdc0-170">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5bdc0-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5bdc0-171">subjectNameFormat</span></span>|[<span data-ttu-id="5bdc0-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5bdc0-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="5bdc0-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="5bdc0-174">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-174">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="5bdc0-175">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="5bdc0-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5bdc0-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5bdc0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5bdc0-177">Int32</span></span>|<span data-ttu-id="5bdc0-178">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5bdc0-179">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-179">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5bdc0-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5bdc0-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5bdc0-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5bdc0-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5bdc0-182">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5bdc0-183">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-183">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="5bdc0-184">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5bdc0-185">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="5bdc0-185">extendedKeyUsages</span></span>|<span data-ttu-id="5bdc0-186">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5bdc0-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="5bdc0-187">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="5bdc0-188">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5bdc0-189">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="5bdc0-189">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5bdc0-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5bdc0-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5bdc0-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5bdc0-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5bdc0-192">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="5bdc0-193">[androidforwork certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-193">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="5bdc0-194">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5bdc0-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="5bdc0-195">certificationAuthority</span></span>|<span data-ttu-id="5bdc0-196">String</span><span class="sxs-lookup"><span data-stu-id="5bdc0-196">String</span></span>|<span data-ttu-id="5bdc0-197">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="5bdc0-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="5bdc0-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="5bdc0-198">certificationAuthorityName</span></span>|<span data-ttu-id="5bdc0-199">String</span><span class="sxs-lookup"><span data-stu-id="5bdc0-199">String</span></span>|<span data-ttu-id="5bdc0-200">PKCS 証明機関名</span><span class="sxs-lookup"><span data-stu-id="5bdc0-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="5bdc0-201">certificatetemplatename</span><span class="sxs-lookup"><span data-stu-id="5bdc0-201">certificateTemplateName</span></span>|<span data-ttu-id="5bdc0-202">String</span><span class="sxs-lookup"><span data-stu-id="5bdc0-202">String</span></span>|<span data-ttu-id="5bdc0-203">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="5bdc0-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="5bdc0-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5bdc0-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5bdc0-205">String</span><span class="sxs-lookup"><span data-stu-id="5bdc0-205">String</span></span>|<span data-ttu-id="5bdc0-206">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="5bdc0-207">応答</span><span class="sxs-lookup"><span data-stu-id="5bdc0-207">Response</span></span>
<span data-ttu-id="5bdc0-208">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bdc0-209">例</span><span class="sxs-lookup"><span data-stu-id="5bdc0-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bdc0-210">要求</span><span class="sxs-lookup"><span data-stu-id="5bdc0-210">Request</span></span>
<span data-ttu-id="5bdc0-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5bdc0-212">応答</span><span class="sxs-lookup"><span data-stu-id="5bdc0-212">Response</span></span>
<span data-ttu-id="5bdc0-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5bdc0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





