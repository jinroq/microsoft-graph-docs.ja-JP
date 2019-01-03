---
title: AndroidImportedPFXCertificateProfile を更新します。
description: AndroidImportedPFXCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: f8f4f78dbefaa3ed2b9e945d2d5eece5046a5bba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352536"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="ce88f-103">AndroidImportedPFXCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="ce88f-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="ce88f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce88f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce88f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce88f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce88f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce88f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce88f-107">[AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ce88f-107">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce88f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce88f-108">Prerequisites</span></span>
<span data-ttu-id="ce88f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce88f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce88f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce88f-111">Permission type</span></span>|<span data-ttu-id="ce88f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce88f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce88f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce88f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce88f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce88f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce88f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce88f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce88f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce88f-116">Not supported.</span></span>|
|<span data-ttu-id="ce88f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce88f-117">Application</span></span>|<span data-ttu-id="ce88f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce88f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce88f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce88f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ce88f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce88f-120">Request headers</span></span>
|<span data-ttu-id="ce88f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce88f-121">Header</span></span>|<span data-ttu-id="ce88f-122">値</span><span class="sxs-lookup"><span data-stu-id="ce88f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce88f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce88f-123">Authorization</span></span>|<span data-ttu-id="ce88f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ce88f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce88f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce88f-125">Accept</span></span>|<span data-ttu-id="ce88f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce88f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce88f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce88f-127">Request body</span></span>
<span data-ttu-id="ce88f-128">要求の本文に[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce88f-128">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="ce88f-129">[AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="ce88f-129">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="ce88f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce88f-130">Property</span></span>|<span data-ttu-id="ce88f-131">種類</span><span class="sxs-lookup"><span data-stu-id="ce88f-131">Type</span></span>|<span data-ttu-id="ce88f-132">説明</span><span class="sxs-lookup"><span data-stu-id="ce88f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce88f-133">ID</span><span class="sxs-lookup"><span data-stu-id="ce88f-133">id</span></span>|<span data-ttu-id="ce88f-134">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-134">String</span></span>|<span data-ttu-id="ce88f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ce88f-135">Key of the entity.</span></span> <span data-ttu-id="ce88f-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce88f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce88f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ce88f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce88f-138">DateTimeOffset</span></span>|<span data-ttu-id="ce88f-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ce88f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ce88f-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce88f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce88f-141">roleScopeTagIds</span></span>|<span data-ttu-id="ce88f-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ce88f-142">String collection</span></span>|<span data-ttu-id="ce88f-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="ce88f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce88f-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce88f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ce88f-145">supportsScopeTags</span></span>|<span data-ttu-id="ce88f-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="ce88f-146">Boolean</span></span>|<span data-ttu-id="ce88f-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce88f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce88f-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="ce88f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce88f-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="ce88f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce88f-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-150">This property is read-only.</span></span> <span data-ttu-id="ce88f-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce88f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce88f-152">createdDateTime</span></span>|<span data-ttu-id="ce88f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce88f-153">DateTimeOffset</span></span>|<span data-ttu-id="ce88f-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ce88f-154">DateTime the object was created.</span></span> <span data-ttu-id="ce88f-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce88f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-156">説明</span><span class="sxs-lookup"><span data-stu-id="ce88f-156">description</span></span>|<span data-ttu-id="ce88f-157">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-157">String</span></span>|<span data-ttu-id="ce88f-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="ce88f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce88f-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce88f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ce88f-160">displayName</span></span>|<span data-ttu-id="ce88f-161">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-161">String</span></span>|<span data-ttu-id="ce88f-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="ce88f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce88f-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce88f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-164">version</span><span class="sxs-lookup"><span data-stu-id="ce88f-164">version</span></span>|<span data-ttu-id="ce88f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-165">Int32</span></span>|<span data-ttu-id="ce88f-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ce88f-166">Version of the device configuration.</span></span> <span data-ttu-id="ce88f-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce88f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ce88f-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="ce88f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-169">Int32</span></span>|<span data-ttu-id="ce88f-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ce88f-171">有効な値は[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="ce88f-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ce88f-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ce88f-172">subjectNameFormat</span></span>|[<span data-ttu-id="ce88f-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ce88f-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ce88f-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="ce88f-175">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ce88f-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="ce88f-176">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ce88f-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ce88f-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ce88f-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ce88f-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ce88f-179">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="ce88f-180">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ce88f-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="ce88f-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ce88f-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ce88f-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ce88f-183">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-183">Int32</span></span>|<span data-ttu-id="ce88f-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="ce88f-185">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ce88f-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ce88f-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ce88f-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ce88f-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ce88f-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ce88f-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="ce88f-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ce88f-189">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ce88f-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="ce88f-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ce88f-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ce88f-191">extendedKeyUsages</span></span>|<span data-ttu-id="ce88f-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ce88f-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ce88f-193">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="ce88f-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ce88f-194">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ce88f-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ce88f-195">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ce88f-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ce88f-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ce88f-196">intendedPurpose</span></span>|[<span data-ttu-id="ce88f-197">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ce88f-197">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="ce88f-198">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="ce88f-198">Not yet documented.</span></span> <span data-ttu-id="ce88f-199">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-199">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="ce88f-200">応答</span><span class="sxs-lookup"><span data-stu-id="ce88f-200">Response</span></span>
<span data-ttu-id="ce88f-201">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ce88f-201">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce88f-202">例</span><span class="sxs-lookup"><span data-stu-id="ce88f-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce88f-203">要求</span><span class="sxs-lookup"><span data-stu-id="ce88f-203">Request</span></span>
<span data-ttu-id="ce88f-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce88f-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 708

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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="ce88f-205">応答</span><span class="sxs-lookup"><span data-stu-id="ce88f-205">Response</span></span>
<span data-ttu-id="ce88f-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce88f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 891

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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
  "intendedPurpose": "smimeEncryption"
}
```




