---
title: Windows10PkcsCertificateProfile を作成する
description: 新しい windows10PkcsCertificateProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb65bd1b7061dc991232f376b5810ebedf7bb703
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978004"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="890ee-103">Windows10PkcsCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="890ee-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="890ee-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="890ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="890ee-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="890ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="890ee-106">新しい[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="890ee-106">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="890ee-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="890ee-107">Prerequisites</span></span>
<span data-ttu-id="890ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="890ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="890ee-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="890ee-110">Permission type</span></span>|<span data-ttu-id="890ee-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="890ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="890ee-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="890ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="890ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="890ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="890ee-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="890ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="890ee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="890ee-115">Not supported.</span></span>|
|<span data-ttu-id="890ee-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="890ee-116">Application</span></span>|<span data-ttu-id="890ee-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="890ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="890ee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="890ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="890ee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="890ee-119">Request headers</span></span>
|<span data-ttu-id="890ee-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="890ee-120">Header</span></span>|<span data-ttu-id="890ee-121">値</span><span class="sxs-lookup"><span data-stu-id="890ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="890ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="890ee-122">Authorization</span></span>|<span data-ttu-id="890ee-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="890ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="890ee-124">承諾</span><span class="sxs-lookup"><span data-stu-id="890ee-124">Accept</span></span>|<span data-ttu-id="890ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="890ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="890ee-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="890ee-126">Request body</span></span>
<span data-ttu-id="890ee-127">要求本文で、windows10PkcsCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="890ee-127">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="890ee-128">次の表に、windows10PkcsCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="890ee-128">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="890ee-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="890ee-129">Property</span></span>|<span data-ttu-id="890ee-130">型</span><span class="sxs-lookup"><span data-stu-id="890ee-130">Type</span></span>|<span data-ttu-id="890ee-131">説明</span><span class="sxs-lookup"><span data-stu-id="890ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="890ee-132">id</span><span class="sxs-lookup"><span data-stu-id="890ee-132">id</span></span>|<span data-ttu-id="890ee-133">文字列</span><span class="sxs-lookup"><span data-stu-id="890ee-133">String</span></span>|<span data-ttu-id="890ee-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="890ee-134">Key of the entity.</span></span> <span data-ttu-id="890ee-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="890ee-136">lastModifiedDateTime</span></span>|<span data-ttu-id="890ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="890ee-137">DateTimeOffset</span></span>|<span data-ttu-id="890ee-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="890ee-138">DateTime the object was last modified.</span></span> <span data-ttu-id="890ee-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="890ee-140">roleScopeTagIds</span></span>|<span data-ttu-id="890ee-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="890ee-141">String collection</span></span>|<span data-ttu-id="890ee-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="890ee-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="890ee-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="890ee-144">supportsScopeTags</span></span>|<span data-ttu-id="890ee-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="890ee-145">Boolean</span></span>|<span data-ttu-id="890ee-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="890ee-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="890ee-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="890ee-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="890ee-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="890ee-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="890ee-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="890ee-149">This property is read-only.</span></span> <span data-ttu-id="890ee-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="890ee-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="890ee-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="890ee-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="890ee-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="890ee-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="890ee-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="890ee-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="890ee-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="890ee-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="890ee-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="890ee-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="890ee-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="890ee-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="890ee-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="890ee-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="890ee-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="890ee-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="890ee-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="890ee-163">createdDateTime</span></span>|<span data-ttu-id="890ee-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="890ee-164">DateTimeOffset</span></span>|<span data-ttu-id="890ee-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="890ee-165">DateTime the object was created.</span></span> <span data-ttu-id="890ee-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-167">description</span><span class="sxs-lookup"><span data-stu-id="890ee-167">description</span></span>|<span data-ttu-id="890ee-168">String</span><span class="sxs-lookup"><span data-stu-id="890ee-168">String</span></span>|<span data-ttu-id="890ee-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="890ee-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="890ee-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-171">displayName</span><span class="sxs-lookup"><span data-stu-id="890ee-171">displayName</span></span>|<span data-ttu-id="890ee-172">String</span><span class="sxs-lookup"><span data-stu-id="890ee-172">String</span></span>|<span data-ttu-id="890ee-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="890ee-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="890ee-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-175">version</span><span class="sxs-lookup"><span data-stu-id="890ee-175">version</span></span>|<span data-ttu-id="890ee-176">Int32</span><span class="sxs-lookup"><span data-stu-id="890ee-176">Int32</span></span>|<span data-ttu-id="890ee-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="890ee-177">Version of the device configuration.</span></span> <span data-ttu-id="890ee-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="890ee-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="890ee-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="890ee-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="890ee-180">Int32</span><span class="sxs-lookup"><span data-stu-id="890ee-180">Int32</span></span>|<span data-ttu-id="890ee-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="890ee-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="890ee-182">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="890ee-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="890ee-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="890ee-183">keyStorageProvider</span></span>|[<span data-ttu-id="890ee-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="890ee-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="890ee-185">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承したキー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="890ee-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="890ee-186">使用可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="890ee-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="890ee-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="890ee-187">subjectNameFormat</span></span>|[<span data-ttu-id="890ee-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="890ee-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="890ee-189">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される証明書のサブジェクト名形式。</span><span class="sxs-lookup"><span data-stu-id="890ee-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="890ee-190">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="890ee-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="890ee-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="890ee-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="890ee-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="890ee-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="890ee-193">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書のサブジェクトの別名型。</span><span class="sxs-lookup"><span data-stu-id="890ee-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="890ee-194">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="890ee-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="890ee-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="890ee-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="890ee-196">Int32</span><span class="sxs-lookup"><span data-stu-id="890ee-196">Int32</span></span>|<span data-ttu-id="890ee-197">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間の値</span><span class="sxs-lookup"><span data-stu-id="890ee-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="890ee-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="890ee-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="890ee-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="890ee-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="890ee-200">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="890ee-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="890ee-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="890ee-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="890ee-202">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="890ee-202">certificationAuthority</span></span>|<span data-ttu-id="890ee-203">String</span><span class="sxs-lookup"><span data-stu-id="890ee-203">String</span></span>|<span data-ttu-id="890ee-204">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="890ee-204">PKCS Certification Authority</span></span>|
|<span data-ttu-id="890ee-205">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="890ee-205">certificationAuthorityName</span></span>|<span data-ttu-id="890ee-206">String</span><span class="sxs-lookup"><span data-stu-id="890ee-206">String</span></span>|<span data-ttu-id="890ee-207">PKCS 証明機関名</span><span class="sxs-lookup"><span data-stu-id="890ee-207">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="890ee-208">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="890ee-208">certificateTemplateName</span></span>|<span data-ttu-id="890ee-209">String</span><span class="sxs-lookup"><span data-stu-id="890ee-209">String</span></span>|<span data-ttu-id="890ee-210">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="890ee-210">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="890ee-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="890ee-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="890ee-212">String</span><span class="sxs-lookup"><span data-stu-id="890ee-212">String</span></span>|<span data-ttu-id="890ee-213">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="890ee-213">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="890ee-214">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="890ee-214">extendedKeyUsages</span></span>|<span data-ttu-id="890ee-215">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="890ee-215">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="890ee-216">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="890ee-216">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="890ee-217">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="890ee-217">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="890ee-218">応答</span><span class="sxs-lookup"><span data-stu-id="890ee-218">Response</span></span>
<span data-ttu-id="890ee-219">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="890ee-219">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="890ee-220">例</span><span class="sxs-lookup"><span data-stu-id="890ee-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="890ee-221">要求</span><span class="sxs-lookup"><span data-stu-id="890ee-221">Request</span></span>
<span data-ttu-id="890ee-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="890ee-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1784

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="890ee-223">応答</span><span class="sxs-lookup"><span data-stu-id="890ee-223">Response</span></span>
<span data-ttu-id="890ee-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="890ee-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1956

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```





