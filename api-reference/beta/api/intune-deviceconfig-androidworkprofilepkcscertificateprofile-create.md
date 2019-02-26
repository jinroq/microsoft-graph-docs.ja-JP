---
title: androidWorkProfilePkcsCertificateProfile を作成する
description: 新しい androidWorkProfilePkcsCertificateProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2ddd365e594ecd25a840125f34845b15662280b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142372"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="7a3d9-103">androidWorkProfilePkcsCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="7a3d9-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="7a3d9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a3d9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a3d9-106">新しい[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-106">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a3d9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7a3d9-107">Prerequisites</span></span>
<span data-ttu-id="7a3d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7a3d9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7a3d9-110">Permission type</span></span>|<span data-ttu-id="7a3d9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7a3d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a3d9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7a3d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a3d9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a3d9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a3d9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7a3d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a3d9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-115">Not supported.</span></span>|
|<span data-ttu-id="7a3d9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7a3d9-116">Application</span></span>|<span data-ttu-id="7a3d9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a3d9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7a3d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7a3d9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a3d9-119">Request headers</span></span>
|<span data-ttu-id="7a3d9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a3d9-120">Header</span></span>|<span data-ttu-id="7a3d9-121">値</span><span class="sxs-lookup"><span data-stu-id="7a3d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a3d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a3d9-122">Authorization</span></span>|<span data-ttu-id="7a3d9-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a3d9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7a3d9-124">Accept</span></span>|<span data-ttu-id="7a3d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a3d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a3d9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7a3d9-126">Request body</span></span>
<span data-ttu-id="7a3d9-127">要求本文で、androidWorkProfilePkcsCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-127">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="7a3d9-128">次の表に、androidWorkProfilePkcsCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-128">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="7a3d9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a3d9-129">Property</span></span>|<span data-ttu-id="7a3d9-130">型</span><span class="sxs-lookup"><span data-stu-id="7a3d9-130">Type</span></span>|<span data-ttu-id="7a3d9-131">説明</span><span class="sxs-lookup"><span data-stu-id="7a3d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a3d9-132">id</span><span class="sxs-lookup"><span data-stu-id="7a3d9-132">id</span></span>|<span data-ttu-id="7a3d9-133">文字列</span><span class="sxs-lookup"><span data-stu-id="7a3d9-133">String</span></span>|<span data-ttu-id="7a3d9-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-134">Key of the entity.</span></span> <span data-ttu-id="7a3d9-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a3d9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3d9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a3d9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7a3d9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a3d9-137">DateTimeOffset</span></span>|<span data-ttu-id="7a3d9-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7a3d9-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a3d9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3d9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7a3d9-140">roleScopeTagIds</span></span>|<span data-ttu-id="7a3d9-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7a3d9-141">String collection</span></span>|<span data-ttu-id="7a3d9-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7a3d9-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a3d9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3d9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7a3d9-144">supportsScopeTags</span></span>|<span data-ttu-id="7a3d9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a3d9-145">Boolean</span></span>|<span data-ttu-id="7a3d9-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7a3d9-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7a3d9-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7a3d9-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-149">This property is read-only.</span></span> <span data-ttu-id="7a3d9-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a3d9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3d9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a3d9-151">createdDateTime</span></span>|<span data-ttu-id="7a3d9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a3d9-152">DateTimeOffset</span></span>|<span data-ttu-id="7a3d9-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-153">DateTime the object was created.</span></span> <span data-ttu-id="7a3d9-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a3d9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3d9-155">説明</span><span class="sxs-lookup"><span data-stu-id="7a3d9-155">description</span></span>|<span data-ttu-id="7a3d9-156">String</span><span class="sxs-lookup"><span data-stu-id="7a3d9-156">String</span></span>|<span data-ttu-id="7a3d9-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7a3d9-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a3d9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3d9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7a3d9-159">displayName</span></span>|<span data-ttu-id="7a3d9-160">String</span><span class="sxs-lookup"><span data-stu-id="7a3d9-160">String</span></span>|<span data-ttu-id="7a3d9-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7a3d9-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a3d9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3d9-163">version</span><span class="sxs-lookup"><span data-stu-id="7a3d9-163">version</span></span>|<span data-ttu-id="7a3d9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7a3d9-164">Int32</span></span>|<span data-ttu-id="7a3d9-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-165">Version of the device configuration.</span></span> <span data-ttu-id="7a3d9-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a3d9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3d9-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="7a3d9-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="7a3d9-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7a3d9-168">Int32</span></span>|<span data-ttu-id="7a3d9-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7a3d9-170">[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承された有効な値 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="7a3d9-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7a3d9-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7a3d9-171">subjectNameFormat</span></span>|[<span data-ttu-id="7a3d9-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7a3d9-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="7a3d9-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="7a3d9-174">[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="7a3d9-175">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="7a3d9-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7a3d9-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7a3d9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7a3d9-177">Int32</span></span>|<span data-ttu-id="7a3d9-178">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7a3d9-179">[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7a3d9-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7a3d9-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7a3d9-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7a3d9-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7a3d9-182">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7a3d9-183">[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="7a3d9-184">可能な値は `days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7a3d9-185">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="7a3d9-185">extendedKeyUsages</span></span>|<span data-ttu-id="7a3d9-186">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7a3d9-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="7a3d9-187">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="7a3d9-188">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7a3d9-189">[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7a3d9-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="7a3d9-190">certificationAuthority</span></span>|<span data-ttu-id="7a3d9-191">String</span><span class="sxs-lookup"><span data-stu-id="7a3d9-191">String</span></span>|<span data-ttu-id="7a3d9-192">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="7a3d9-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="7a3d9-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="7a3d9-193">certificationAuthorityName</span></span>|<span data-ttu-id="7a3d9-194">String</span><span class="sxs-lookup"><span data-stu-id="7a3d9-194">String</span></span>|<span data-ttu-id="7a3d9-195">PKCS 証明機関名</span><span class="sxs-lookup"><span data-stu-id="7a3d9-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="7a3d9-196">certificatetemplatename</span><span class="sxs-lookup"><span data-stu-id="7a3d9-196">certificateTemplateName</span></span>|<span data-ttu-id="7a3d9-197">String</span><span class="sxs-lookup"><span data-stu-id="7a3d9-197">String</span></span>|<span data-ttu-id="7a3d9-198">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="7a3d9-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="7a3d9-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7a3d9-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7a3d9-200">String</span><span class="sxs-lookup"><span data-stu-id="7a3d9-200">String</span></span>|<span data-ttu-id="7a3d9-201">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="7a3d9-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7a3d9-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7a3d9-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7a3d9-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7a3d9-204">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="7a3d9-205">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-205">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="7a3d9-206">応答</span><span class="sxs-lookup"><span data-stu-id="7a3d9-206">Response</span></span>
<span data-ttu-id="7a3d9-207">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-207">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a3d9-208">例</span><span class="sxs-lookup"><span data-stu-id="7a3d9-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a3d9-209">要求</span><span class="sxs-lookup"><span data-stu-id="7a3d9-209">Request</span></span>
<span data-ttu-id="7a3d9-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 969

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="7a3d9-211">応答</span><span class="sxs-lookup"><span data-stu-id="7a3d9-211">Response</span></span>
<span data-ttu-id="7a3d9-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7a3d9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1141

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```




