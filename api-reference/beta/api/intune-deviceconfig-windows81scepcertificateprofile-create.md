---
title: Windows81SCEPCertificateProfile を作成します。
description: 新しい windows81SCEPCertificateProfile オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d28a0930493423885149fc27ad600783c8f2485b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422188"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="cc6ed-103">Windows81SCEPCertificateProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="cc6ed-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc6ed-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc6ed-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc6ed-107">新しい[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-107">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc6ed-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cc6ed-108">Prerequisites</span></span>
<span data-ttu-id="cc6ed-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc6ed-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc6ed-111">Permission type</span></span>|<span data-ttu-id="cc6ed-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc6ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc6ed-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc6ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc6ed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc6ed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc6ed-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc6ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc6ed-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-116">Not supported.</span></span>|
|<span data-ttu-id="cc6ed-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc6ed-117">Application</span></span>|<span data-ttu-id="cc6ed-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc6ed-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc6ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cc6ed-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc6ed-120">Request headers</span></span>
|<span data-ttu-id="cc6ed-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc6ed-121">Header</span></span>|<span data-ttu-id="cc6ed-122">値</span><span class="sxs-lookup"><span data-stu-id="cc6ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc6ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc6ed-123">Authorization</span></span>|<span data-ttu-id="cc6ed-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc6ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc6ed-125">Accept</span></span>|<span data-ttu-id="cc6ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc6ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc6ed-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc6ed-127">Request body</span></span>
<span data-ttu-id="cc6ed-128">要求の本文に windows81SCEPCertificateProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-128">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="cc6ed-129">次の表は、windows81SCEPCertificateProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-129">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="cc6ed-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc6ed-130">Property</span></span>|<span data-ttu-id="cc6ed-131">型</span><span class="sxs-lookup"><span data-stu-id="cc6ed-131">Type</span></span>|<span data-ttu-id="cc6ed-132">説明</span><span class="sxs-lookup"><span data-stu-id="cc6ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc6ed-133">id</span><span class="sxs-lookup"><span data-stu-id="cc6ed-133">id</span></span>|<span data-ttu-id="cc6ed-134">String</span><span class="sxs-lookup"><span data-stu-id="cc6ed-134">String</span></span>|<span data-ttu-id="cc6ed-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-135">Key of the entity.</span></span> <span data-ttu-id="cc6ed-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cc6ed-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc6ed-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc6ed-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cc6ed-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc6ed-138">DateTimeOffset</span></span>|<span data-ttu-id="cc6ed-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cc6ed-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cc6ed-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc6ed-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc6ed-141">roleScopeTagIds</span></span>|<span data-ttu-id="cc6ed-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cc6ed-142">String collection</span></span>|<span data-ttu-id="cc6ed-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cc6ed-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cc6ed-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc6ed-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cc6ed-145">supportsScopeTags</span></span>|<span data-ttu-id="cc6ed-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc6ed-146">Boolean</span></span>|<span data-ttu-id="cc6ed-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cc6ed-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cc6ed-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cc6ed-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-150">This property is read-only.</span></span> <span data-ttu-id="cc6ed-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cc6ed-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc6ed-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc6ed-152">createdDateTime</span></span>|<span data-ttu-id="cc6ed-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc6ed-153">DateTimeOffset</span></span>|<span data-ttu-id="cc6ed-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-154">DateTime the object was created.</span></span> <span data-ttu-id="cc6ed-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cc6ed-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc6ed-156">説明</span><span class="sxs-lookup"><span data-stu-id="cc6ed-156">description</span></span>|<span data-ttu-id="cc6ed-157">String</span><span class="sxs-lookup"><span data-stu-id="cc6ed-157">String</span></span>|<span data-ttu-id="cc6ed-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cc6ed-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cc6ed-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc6ed-160">displayName</span><span class="sxs-lookup"><span data-stu-id="cc6ed-160">displayName</span></span>|<span data-ttu-id="cc6ed-161">String</span><span class="sxs-lookup"><span data-stu-id="cc6ed-161">String</span></span>|<span data-ttu-id="cc6ed-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cc6ed-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cc6ed-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc6ed-164">version</span><span class="sxs-lookup"><span data-stu-id="cc6ed-164">version</span></span>|<span data-ttu-id="cc6ed-165">Int32</span><span class="sxs-lookup"><span data-stu-id="cc6ed-165">Int32</span></span>|<span data-ttu-id="cc6ed-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-166">Version of the device configuration.</span></span> <span data-ttu-id="cc6ed-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cc6ed-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc6ed-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="cc6ed-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="cc6ed-169">Int32</span><span class="sxs-lookup"><span data-stu-id="cc6ed-169">Int32</span></span>|<span data-ttu-id="cc6ed-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="cc6ed-171">有効な値は[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="cc6ed-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cc6ed-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="cc6ed-172">keyStorageProvider</span></span>|[<span data-ttu-id="cc6ed-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="cc6ed-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="cc6ed-174">[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)からキー記憶域プロバイダー (KSP) 継承します。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="cc6ed-175">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="cc6ed-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cc6ed-176">subjectNameFormat</span></span>|[<span data-ttu-id="cc6ed-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cc6ed-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="cc6ed-178">証明書サブジェクト名の形式から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="cc6ed-179">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="cc6ed-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cc6ed-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="cc6ed-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cc6ed-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="cc6ed-182">証明書サブジェクト代替名タイプから継承[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="cc6ed-183">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="cc6ed-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="cc6ed-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="cc6ed-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cc6ed-185">Int32</span></span>|<span data-ttu-id="cc6ed-186">証明書有効期間から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)の値</span><span class="sxs-lookup"><span data-stu-id="cc6ed-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cc6ed-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cc6ed-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="cc6ed-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cc6ed-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="cc6ed-189">証明書有効期間から継承された[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)のスケールです。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="cc6ed-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="cc6ed-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="cc6ed-191">extendedKeyUsages</span></span>|<span data-ttu-id="cc6ed-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc6ed-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="cc6ed-193">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="cc6ed-194">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="cc6ed-195">[Windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-195">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="cc6ed-196">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="cc6ed-196">customSubjectAlternativeNames</span></span>|<span data-ttu-id="cc6ed-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc6ed-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="cc6ed-198">Alterantive 名の設定をカスタムの件名です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-198">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="cc6ed-199">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="cc6ed-200">[Windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-200">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="cc6ed-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="cc6ed-201">scepServerUrls</span></span>|<span data-ttu-id="cc6ed-202">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cc6ed-202">String collection</span></span>|<span data-ttu-id="cc6ed-203">SCEP サーバー個の url。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="cc6ed-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="cc6ed-204">subjectNameFormatString</span></span>|<span data-ttu-id="cc6ed-205">String</span><span class="sxs-lookup"><span data-stu-id="cc6ed-205">String</span></span>|<span data-ttu-id="cc6ed-206">SubjectNameFormat で使用するカスタム書式指定 = カスタムです。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="cc6ed-207">例: CN = EmailAddress {{}}、E = EmailAddress {{}}、OU = エンタープライズ ユーザーの場合は、O = コントソ株式会社、L = Redmond、ST = ワシントン州 C = u. s.</span><span class="sxs-lookup"><span data-stu-id="cc6ed-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="cc6ed-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="cc6ed-208">keyUsage</span></span>|[<span data-ttu-id="cc6ed-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="cc6ed-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="cc6ed-210">SCEP のキー使用法です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-210">SCEP Key Usage.</span></span> <span data-ttu-id="cc6ed-211">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="cc6ed-212">キー長</span><span class="sxs-lookup"><span data-stu-id="cc6ed-212">keySize</span></span>|[<span data-ttu-id="cc6ed-213">キー長</span><span class="sxs-lookup"><span data-stu-id="cc6ed-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="cc6ed-214">SCEP のキー サイズ。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-214">SCEP Key Size.</span></span> <span data-ttu-id="cc6ed-215">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="cc6ed-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="cc6ed-216">hashAlgorithm</span></span>|[<span data-ttu-id="cc6ed-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="cc6ed-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="cc6ed-218">SCEP ハッシュ アルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="cc6ed-219">使用可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="cc6ed-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="cc6ed-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="cc6ed-221">String</span><span class="sxs-lookup"><span data-stu-id="cc6ed-221">String</span></span>|<span data-ttu-id="cc6ed-222">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-222">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="cc6ed-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="cc6ed-223">certificateStore</span></span>|[<span data-ttu-id="cc6ed-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="cc6ed-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="cc6ed-225">ターゲット ストアの証明書です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-225">Target store certificate.</span></span> <span data-ttu-id="cc6ed-226">使用可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-226">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="cc6ed-227">応答</span><span class="sxs-lookup"><span data-stu-id="cc6ed-227">Response</span></span>
<span data-ttu-id="cc6ed-228">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-228">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc6ed-229">例</span><span class="sxs-lookup"><span data-stu-id="cc6ed-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc6ed-230">要求</span><span class="sxs-lookup"><span data-stu-id="cc6ed-230">Request</span></span>
<span data-ttu-id="cc6ed-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1251

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="cc6ed-232">応答</span><span class="sxs-lookup"><span data-stu-id="cc6ed-232">Response</span></span>
<span data-ttu-id="cc6ed-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc6ed-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




