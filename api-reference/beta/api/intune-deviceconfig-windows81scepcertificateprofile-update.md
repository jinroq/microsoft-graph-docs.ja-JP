---
title: Windows81SCEPCertificateProfile を更新します。
description: Windows81SCEPCertificateProfile オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 39571d85a1eb7d9a2d5d0a18f178fb2cb1be7e02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338221"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="d55fc-103">Windows81SCEPCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="d55fc-103">Update windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="d55fc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d55fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d55fc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d55fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d55fc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d55fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d55fc-107">[Windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d55fc-107">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d55fc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d55fc-108">Prerequisites</span></span>
<span data-ttu-id="d55fc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d55fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d55fc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d55fc-111">Permission type</span></span>|<span data-ttu-id="d55fc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d55fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d55fc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d55fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d55fc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55fc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d55fc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d55fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d55fc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d55fc-116">Not supported.</span></span>|
|<span data-ttu-id="d55fc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d55fc-117">Application</span></span>|<span data-ttu-id="d55fc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d55fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d55fc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d55fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d55fc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d55fc-120">Request headers</span></span>
|<span data-ttu-id="d55fc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d55fc-121">Header</span></span>|<span data-ttu-id="d55fc-122">値</span><span class="sxs-lookup"><span data-stu-id="d55fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d55fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d55fc-123">Authorization</span></span>|<span data-ttu-id="d55fc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d55fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d55fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d55fc-125">Accept</span></span>|<span data-ttu-id="d55fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d55fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d55fc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d55fc-127">Request body</span></span>
<span data-ttu-id="d55fc-128">要求の本文に[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d55fc-128">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="d55fc-129">[Windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="d55fc-129">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="d55fc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d55fc-130">Property</span></span>|<span data-ttu-id="d55fc-131">種類</span><span class="sxs-lookup"><span data-stu-id="d55fc-131">Type</span></span>|<span data-ttu-id="d55fc-132">説明</span><span class="sxs-lookup"><span data-stu-id="d55fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d55fc-133">ID</span><span class="sxs-lookup"><span data-stu-id="d55fc-133">id</span></span>|<span data-ttu-id="d55fc-134">String</span><span class="sxs-lookup"><span data-stu-id="d55fc-134">String</span></span>|<span data-ttu-id="d55fc-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d55fc-135">Key of the entity.</span></span> <span data-ttu-id="d55fc-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d55fc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d55fc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d55fc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d55fc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d55fc-138">DateTimeOffset</span></span>|<span data-ttu-id="d55fc-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d55fc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d55fc-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d55fc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d55fc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d55fc-141">roleScopeTagIds</span></span>|<span data-ttu-id="d55fc-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d55fc-142">String collection</span></span>|<span data-ttu-id="d55fc-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="d55fc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d55fc-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d55fc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d55fc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d55fc-145">supportsScopeTags</span></span>|<span data-ttu-id="d55fc-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="d55fc-146">Boolean</span></span>|<span data-ttu-id="d55fc-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d55fc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d55fc-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="d55fc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d55fc-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="d55fc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d55fc-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-150">This property is read-only.</span></span> <span data-ttu-id="d55fc-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d55fc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d55fc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d55fc-152">createdDateTime</span></span>|<span data-ttu-id="d55fc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d55fc-153">DateTimeOffset</span></span>|<span data-ttu-id="d55fc-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d55fc-154">DateTime the object was created.</span></span> <span data-ttu-id="d55fc-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d55fc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d55fc-156">説明</span><span class="sxs-lookup"><span data-stu-id="d55fc-156">description</span></span>|<span data-ttu-id="d55fc-157">String</span><span class="sxs-lookup"><span data-stu-id="d55fc-157">String</span></span>|<span data-ttu-id="d55fc-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d55fc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d55fc-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d55fc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d55fc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d55fc-160">displayName</span></span>|<span data-ttu-id="d55fc-161">String</span><span class="sxs-lookup"><span data-stu-id="d55fc-161">String</span></span>|<span data-ttu-id="d55fc-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d55fc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d55fc-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d55fc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d55fc-164">version</span><span class="sxs-lookup"><span data-stu-id="d55fc-164">version</span></span>|<span data-ttu-id="d55fc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d55fc-165">Int32</span></span>|<span data-ttu-id="d55fc-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d55fc-166">Version of the device configuration.</span></span> <span data-ttu-id="d55fc-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d55fc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d55fc-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d55fc-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="d55fc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d55fc-169">Int32</span></span>|<span data-ttu-id="d55fc-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d55fc-171">有効な値は[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="d55fc-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d55fc-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="d55fc-172">keyStorageProvider</span></span>|[<span data-ttu-id="d55fc-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="d55fc-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="d55fc-174">[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)からキー記憶域プロバイダー (KSP) 継承します。</span><span class="sxs-lookup"><span data-stu-id="d55fc-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d55fc-175">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="d55fc-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d55fc-176">subjectNameFormat</span></span>|[<span data-ttu-id="d55fc-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d55fc-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d55fc-178">証明書サブジェクト名の形式から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d55fc-179">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d55fc-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d55fc-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d55fc-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d55fc-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d55fc-182">証明書サブジェクト代替名タイプから継承[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d55fc-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d55fc-183">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d55fc-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d55fc-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d55fc-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d55fc-185">Int32</span></span>|<span data-ttu-id="d55fc-186">証明書有効期間から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)の値</span><span class="sxs-lookup"><span data-stu-id="d55fc-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d55fc-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d55fc-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d55fc-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d55fc-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d55fc-189">証明書有効期間から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)のスケールです。</span><span class="sxs-lookup"><span data-stu-id="d55fc-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d55fc-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d55fc-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d55fc-191">extendedKeyUsages</span></span>|<span data-ttu-id="d55fc-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d55fc-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d55fc-193">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="d55fc-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d55fc-194">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d55fc-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d55fc-195">[Windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d55fc-195">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="d55fc-196">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="d55fc-196">customSubjectAlternativeNames</span></span>|<span data-ttu-id="d55fc-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d55fc-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="d55fc-198">Alterantive 名の設定をカスタムの件名です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-198">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="d55fc-199">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d55fc-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d55fc-200">[Windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d55fc-200">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="d55fc-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="d55fc-201">scepServerUrls</span></span>|<span data-ttu-id="d55fc-202">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d55fc-202">String collection</span></span>|<span data-ttu-id="d55fc-203">SCEP サーバー個の url。</span><span class="sxs-lookup"><span data-stu-id="d55fc-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="d55fc-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d55fc-204">subjectNameFormatString</span></span>|<span data-ttu-id="d55fc-205">String</span><span class="sxs-lookup"><span data-stu-id="d55fc-205">String</span></span>|<span data-ttu-id="d55fc-206">SubjectNameFormat で使用するカスタム書式指定 = カスタムです。</span><span class="sxs-lookup"><span data-stu-id="d55fc-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="d55fc-207">例: CN = EmailAddress {{}}、E = EmailAddress {{}}、OU = エンタープライズ ユーザーの場合は、O = コントソ株式会社、L = Redmond、ST = ワシントン州 C = u. s.</span><span class="sxs-lookup"><span data-stu-id="d55fc-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="d55fc-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="d55fc-208">keyUsage</span></span>|[<span data-ttu-id="d55fc-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="d55fc-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="d55fc-210">SCEP のキー使用法です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-210">SCEP Key Usage.</span></span> <span data-ttu-id="d55fc-211">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="d55fc-212">キー長</span><span class="sxs-lookup"><span data-stu-id="d55fc-212">keySize</span></span>|[<span data-ttu-id="d55fc-213">キー長</span><span class="sxs-lookup"><span data-stu-id="d55fc-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="d55fc-214">SCEP のキー サイズ。</span><span class="sxs-lookup"><span data-stu-id="d55fc-214">SCEP Key Size.</span></span> <span data-ttu-id="d55fc-215">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="d55fc-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d55fc-216">hashAlgorithm</span></span>|[<span data-ttu-id="d55fc-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="d55fc-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="d55fc-218">SCEP ハッシュ アルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="d55fc-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="d55fc-219">使用可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="d55fc-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d55fc-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d55fc-221">String</span><span class="sxs-lookup"><span data-stu-id="d55fc-221">String</span></span>|<span data-ttu-id="d55fc-222">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="d55fc-222">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="d55fc-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d55fc-223">certificateStore</span></span>|[<span data-ttu-id="d55fc-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d55fc-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="d55fc-225">ターゲット ストアの証明書です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-225">Target store certificate.</span></span> <span data-ttu-id="d55fc-226">使用可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-226">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="d55fc-227">応答</span><span class="sxs-lookup"><span data-stu-id="d55fc-227">Response</span></span>
<span data-ttu-id="d55fc-228">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d55fc-228">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d55fc-229">例</span><span class="sxs-lookup"><span data-stu-id="d55fc-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="d55fc-230">要求</span><span class="sxs-lookup"><span data-stu-id="d55fc-230">Request</span></span>
<span data-ttu-id="d55fc-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d55fc-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1245

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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
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
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="d55fc-232">応答</span><span class="sxs-lookup"><span data-stu-id="d55fc-232">Response</span></span>
<span data-ttu-id="d55fc-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d55fc-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1423

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
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
  "certificateStore": "machine"
}
```





