---
title: AndroidForWorkPkcsCertificateProfile を更新します。
description: AndroidForWorkPkcsCertificateProfile オブジェクトのプロパティを更新します。
ms.openlocfilehash: aa66069317ea2be9d13b21e8f909edc2a36ddc99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072245"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="f4ccf-103">AndroidForWorkPkcsCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="f4ccf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4ccf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4ccf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4ccf-107">[AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-107">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4ccf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f4ccf-108">Prerequisites</span></span>
<span data-ttu-id="f4ccf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4ccf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4ccf-111">Permission type</span></span>|<span data-ttu-id="f4ccf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4ccf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4ccf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4ccf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4ccf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4ccf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4ccf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4ccf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4ccf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-116">Not supported.</span></span>|
|<span data-ttu-id="f4ccf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4ccf-117">Application</span></span>|<span data-ttu-id="f4ccf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4ccf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4ccf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4ccf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4ccf-120">Request headers</span></span>
|<span data-ttu-id="f4ccf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4ccf-121">Header</span></span>|<span data-ttu-id="f4ccf-122">値</span><span class="sxs-lookup"><span data-stu-id="f4ccf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4ccf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4ccf-123">Authorization</span></span>|<span data-ttu-id="f4ccf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4ccf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4ccf-125">Accept</span></span>|<span data-ttu-id="f4ccf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4ccf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4ccf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4ccf-127">Request body</span></span>
<span data-ttu-id="f4ccf-128">要求の本文に[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-128">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="f4ccf-129">[AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-129">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="f4ccf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4ccf-130">Property</span></span>|<span data-ttu-id="f4ccf-131">型</span><span class="sxs-lookup"><span data-stu-id="f4ccf-131">Type</span></span>|<span data-ttu-id="f4ccf-132">説明</span><span class="sxs-lookup"><span data-stu-id="f4ccf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4ccf-133">id</span><span class="sxs-lookup"><span data-stu-id="f4ccf-133">id</span></span>|<span data-ttu-id="f4ccf-134">String</span><span class="sxs-lookup"><span data-stu-id="f4ccf-134">String</span></span>|<span data-ttu-id="f4ccf-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-135">Key of the entity.</span></span> <span data-ttu-id="f4ccf-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4ccf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4ccf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ccf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f4ccf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ccf-138">DateTimeOffset</span></span>|<span data-ttu-id="f4ccf-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f4ccf-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4ccf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4ccf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4ccf-141">roleScopeTagIds</span></span>|<span data-ttu-id="f4ccf-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f4ccf-142">String collection</span></span>|<span data-ttu-id="f4ccf-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4ccf-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4ccf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4ccf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4ccf-145">supportsScopeTags</span></span>|<span data-ttu-id="f4ccf-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="f4ccf-146">Boolean</span></span>|<span data-ttu-id="f4ccf-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4ccf-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4ccf-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4ccf-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-150">This property is read-only.</span></span> <span data-ttu-id="f4ccf-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4ccf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4ccf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ccf-152">createdDateTime</span></span>|<span data-ttu-id="f4ccf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ccf-153">DateTimeOffset</span></span>|<span data-ttu-id="f4ccf-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-154">DateTime the object was created.</span></span> <span data-ttu-id="f4ccf-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4ccf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4ccf-156">説明</span><span class="sxs-lookup"><span data-stu-id="f4ccf-156">description</span></span>|<span data-ttu-id="f4ccf-157">String</span><span class="sxs-lookup"><span data-stu-id="f4ccf-157">String</span></span>|<span data-ttu-id="f4ccf-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4ccf-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4ccf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4ccf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f4ccf-160">displayName</span></span>|<span data-ttu-id="f4ccf-161">String</span><span class="sxs-lookup"><span data-stu-id="f4ccf-161">String</span></span>|<span data-ttu-id="f4ccf-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4ccf-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4ccf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4ccf-164">version</span><span class="sxs-lookup"><span data-stu-id="f4ccf-164">version</span></span>|<span data-ttu-id="f4ccf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f4ccf-165">Int32</span></span>|<span data-ttu-id="f4ccf-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-166">Version of the device configuration.</span></span> <span data-ttu-id="f4ccf-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4ccf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4ccf-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f4ccf-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="f4ccf-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f4ccf-169">Int32</span></span>|<span data-ttu-id="f4ccf-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f4ccf-171">有効な値は[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="f4ccf-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f4ccf-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f4ccf-172">subjectNameFormat</span></span>|[<span data-ttu-id="f4ccf-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f4ccf-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f4ccf-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="f4ccf-175">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="f4ccf-176">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f4ccf-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f4ccf-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f4ccf-178">Int32</span><span class="sxs-lookup"><span data-stu-id="f4ccf-178">Int32</span></span>|<span data-ttu-id="f4ccf-179">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f4ccf-180">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f4ccf-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f4ccf-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f4ccf-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f4ccf-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f4ccf-183">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f4ccf-184">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="f4ccf-185">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f4ccf-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f4ccf-186">extendedKeyUsages</span></span>|<span data-ttu-id="f4ccf-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f4ccf-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f4ccf-188">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f4ccf-189">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f4ccf-190">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f4ccf-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="f4ccf-191">certificationAuthority</span></span>|<span data-ttu-id="f4ccf-192">String</span><span class="sxs-lookup"><span data-stu-id="f4ccf-192">String</span></span>|<span data-ttu-id="f4ccf-193">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="f4ccf-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="f4ccf-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="f4ccf-194">certificationAuthorityName</span></span>|<span data-ttu-id="f4ccf-195">String</span><span class="sxs-lookup"><span data-stu-id="f4ccf-195">String</span></span>|<span data-ttu-id="f4ccf-196">PKCS 証明機関の名前</span><span class="sxs-lookup"><span data-stu-id="f4ccf-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="f4ccf-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="f4ccf-197">certificateTemplateName</span></span>|<span data-ttu-id="f4ccf-198">String</span><span class="sxs-lookup"><span data-stu-id="f4ccf-198">String</span></span>|<span data-ttu-id="f4ccf-199">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="f4ccf-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="f4ccf-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f4ccf-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f4ccf-201">String</span><span class="sxs-lookup"><span data-stu-id="f4ccf-201">String</span></span>|<span data-ttu-id="f4ccf-202">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f4ccf-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f4ccf-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f4ccf-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f4ccf-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f4ccf-205">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f4ccf-206">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="f4ccf-207">応答</span><span class="sxs-lookup"><span data-stu-id="f4ccf-207">Response</span></span>
<span data-ttu-id="f4ccf-208">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4ccf-209">例</span><span class="sxs-lookup"><span data-stu-id="f4ccf-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4ccf-210">要求</span><span class="sxs-lookup"><span data-stu-id="f4ccf-210">Request</span></span>
<span data-ttu-id="f4ccf-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 954

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="f4ccf-212">応答</span><span class="sxs-lookup"><span data-stu-id="f4ccf-212">Response</span></span>
<span data-ttu-id="f4ccf-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4ccf-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```





