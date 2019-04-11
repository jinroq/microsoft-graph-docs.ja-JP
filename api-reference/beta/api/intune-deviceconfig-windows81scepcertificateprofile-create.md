---
title: windows81SCEPCertificateProfile を作成する
description: 新しい windows81SCEPCertificateProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18448f308a8b7fd0056ec86ebf31ecc181b0ec82
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788234"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="17bbb-103">windows81SCEPCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="17bbb-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="17bbb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17bbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17bbb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17bbb-106">新しい[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="17bbb-106">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17bbb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="17bbb-107">Prerequisites</span></span>
<span data-ttu-id="17bbb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17bbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17bbb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="17bbb-110">Permission type</span></span>|<span data-ttu-id="17bbb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="17bbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17bbb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="17bbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17bbb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17bbb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17bbb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="17bbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17bbb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17bbb-115">Not supported.</span></span>|
|<span data-ttu-id="17bbb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="17bbb-116">Application</span></span>|<span data-ttu-id="17bbb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17bbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17bbb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17bbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="17bbb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17bbb-119">Request headers</span></span>
|<span data-ttu-id="17bbb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17bbb-120">Header</span></span>|<span data-ttu-id="17bbb-121">値</span><span class="sxs-lookup"><span data-stu-id="17bbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17bbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17bbb-122">Authorization</span></span>|<span data-ttu-id="17bbb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17bbb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="17bbb-124">Accept</span></span>|<span data-ttu-id="17bbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17bbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17bbb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="17bbb-126">Request body</span></span>
<span data-ttu-id="17bbb-127">要求本文で、windows81SCEPCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="17bbb-127">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="17bbb-128">次の表に、windows81SCEPCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="17bbb-128">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="17bbb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17bbb-129">Property</span></span>|<span data-ttu-id="17bbb-130">型</span><span class="sxs-lookup"><span data-stu-id="17bbb-130">Type</span></span>|<span data-ttu-id="17bbb-131">説明</span><span class="sxs-lookup"><span data-stu-id="17bbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17bbb-132">id</span><span class="sxs-lookup"><span data-stu-id="17bbb-132">id</span></span>|<span data-ttu-id="17bbb-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="17bbb-133">String</span></span>|<span data-ttu-id="17bbb-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="17bbb-134">Key of the entity.</span></span> <span data-ttu-id="17bbb-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="17bbb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17bbb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17bbb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="17bbb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17bbb-137">DateTimeOffset</span></span>|<span data-ttu-id="17bbb-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="17bbb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="17bbb-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="17bbb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17bbb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17bbb-140">roleScopeTagIds</span></span>|<span data-ttu-id="17bbb-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="17bbb-141">String collection</span></span>|<span data-ttu-id="17bbb-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="17bbb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="17bbb-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="17bbb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17bbb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="17bbb-144">supportsScopeTags</span></span>|<span data-ttu-id="17bbb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="17bbb-145">Boolean</span></span>|<span data-ttu-id="17bbb-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="17bbb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="17bbb-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="17bbb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="17bbb-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="17bbb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="17bbb-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="17bbb-149">This property is read-only.</span></span> <span data-ttu-id="17bbb-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="17bbb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17bbb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17bbb-151">createdDateTime</span></span>|<span data-ttu-id="17bbb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17bbb-152">DateTimeOffset</span></span>|<span data-ttu-id="17bbb-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="17bbb-153">DateTime the object was created.</span></span> <span data-ttu-id="17bbb-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="17bbb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17bbb-155">説明</span><span class="sxs-lookup"><span data-stu-id="17bbb-155">description</span></span>|<span data-ttu-id="17bbb-156">String</span><span class="sxs-lookup"><span data-stu-id="17bbb-156">String</span></span>|<span data-ttu-id="17bbb-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="17bbb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17bbb-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="17bbb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17bbb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="17bbb-159">displayName</span></span>|<span data-ttu-id="17bbb-160">String</span><span class="sxs-lookup"><span data-stu-id="17bbb-160">String</span></span>|<span data-ttu-id="17bbb-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="17bbb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17bbb-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="17bbb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17bbb-163">version</span><span class="sxs-lookup"><span data-stu-id="17bbb-163">version</span></span>|<span data-ttu-id="17bbb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="17bbb-164">Int32</span></span>|<span data-ttu-id="17bbb-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="17bbb-165">Version of the device configuration.</span></span> <span data-ttu-id="17bbb-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="17bbb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17bbb-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="17bbb-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="17bbb-168">Int32</span><span class="sxs-lookup"><span data-stu-id="17bbb-168">Int32</span></span>|<span data-ttu-id="17bbb-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="17bbb-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="17bbb-170">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="17bbb-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="17bbb-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="17bbb-171">keyStorageProvider</span></span>|[<span data-ttu-id="17bbb-172">keystorageprovideroption</span><span class="sxs-lookup"><span data-stu-id="17bbb-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="17bbb-173">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承したキー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="17bbb-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="17bbb-174">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="17bbb-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="17bbb-175">subjectNameFormat</span></span>|[<span data-ttu-id="17bbb-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="17bbb-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="17bbb-177">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される証明書のサブジェクト名形式。</span><span class="sxs-lookup"><span data-stu-id="17bbb-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="17bbb-178">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="17bbb-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="17bbb-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="17bbb-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="17bbb-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="17bbb-181">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書のサブジェクトの別名型。</span><span class="sxs-lookup"><span data-stu-id="17bbb-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="17bbb-182">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="17bbb-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="17bbb-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="17bbb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="17bbb-184">Int32</span></span>|<span data-ttu-id="17bbb-185">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間の値</span><span class="sxs-lookup"><span data-stu-id="17bbb-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="17bbb-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="17bbb-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="17bbb-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="17bbb-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="17bbb-188">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="17bbb-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="17bbb-189">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="17bbb-190">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="17bbb-190">extendedKeyUsages</span></span>|<span data-ttu-id="17bbb-191">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="17bbb-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="17bbb-192">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="17bbb-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="17bbb-193">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="17bbb-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="17bbb-194">[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="17bbb-194">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="17bbb-195">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="17bbb-195">customSubjectAlternativeNames</span></span>|<span data-ttu-id="17bbb-196">[customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="17bbb-196">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="17bbb-197">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="17bbb-197">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="17bbb-198">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="17bbb-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="17bbb-199">[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="17bbb-199">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="17bbb-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="17bbb-200">scepServerUrls</span></span>|<span data-ttu-id="17bbb-201">String コレクション</span><span class="sxs-lookup"><span data-stu-id="17bbb-201">String collection</span></span>|<span data-ttu-id="17bbb-202">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="17bbb-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="17bbb-203">subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="17bbb-203">subjectNameFormatString</span></span>|<span data-ttu-id="17bbb-204">文字列</span><span class="sxs-lookup"><span data-stu-id="17bbb-204">String</span></span>|<span data-ttu-id="17bbb-205">SubjectNameFormat = custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="17bbb-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="17bbb-206">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="17bbb-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="17bbb-207">keyusage</span><span class="sxs-lookup"><span data-stu-id="17bbb-207">keyUsage</span></span>|[<span data-ttu-id="17bbb-208">keyusages</span><span class="sxs-lookup"><span data-stu-id="17bbb-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="17bbb-209">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="17bbb-209">SCEP Key Usage.</span></span> <span data-ttu-id="17bbb-210">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="17bbb-211">keySize</span><span class="sxs-lookup"><span data-stu-id="17bbb-211">keySize</span></span>|[<span data-ttu-id="17bbb-212">keySize</span><span class="sxs-lookup"><span data-stu-id="17bbb-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="17bbb-213">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="17bbb-213">SCEP Key Size.</span></span> <span data-ttu-id="17bbb-214">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="17bbb-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="17bbb-215">hashAlgorithm</span></span>|[<span data-ttu-id="17bbb-216">hashalgorithms</span><span class="sxs-lookup"><span data-stu-id="17bbb-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="17bbb-217">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="17bbb-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="17bbb-218">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="17bbb-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="17bbb-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="17bbb-220">文字列</span><span class="sxs-lookup"><span data-stu-id="17bbb-220">String</span></span>|<span data-ttu-id="17bbb-221">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="17bbb-221">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="17bbb-222">certificateStore</span><span class="sxs-lookup"><span data-stu-id="17bbb-222">certificateStore</span></span>|[<span data-ttu-id="17bbb-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="17bbb-223">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="17bbb-224">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="17bbb-224">Target store certificate.</span></span> <span data-ttu-id="17bbb-225">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-225">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="17bbb-226">応答</span><span class="sxs-lookup"><span data-stu-id="17bbb-226">Response</span></span>
<span data-ttu-id="17bbb-227">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="17bbb-227">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17bbb-228">例</span><span class="sxs-lookup"><span data-stu-id="17bbb-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="17bbb-229">要求</span><span class="sxs-lookup"><span data-stu-id="17bbb-229">Request</span></span>
<span data-ttu-id="17bbb-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="17bbb-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17bbb-231">応答</span><span class="sxs-lookup"><span data-stu-id="17bbb-231">Response</span></span>
<span data-ttu-id="17bbb-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="17bbb-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





