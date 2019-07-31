---
title: Windows10ImportedPFXCertificateProfile の更新
description: Windows10ImportedPFXCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cdb796bbd7c38eef5792f26c10a92f640c953116
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975558"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="f2f38-103">Windows10ImportedPFXCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="f2f38-103">Update windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="f2f38-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2f38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2f38-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2f38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2f38-106">[Windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f2f38-106">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2f38-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f2f38-107">Prerequisites</span></span>
<span data-ttu-id="f2f38-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2f38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2f38-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2f38-110">Permission type</span></span>|<span data-ttu-id="f2f38-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2f38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2f38-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2f38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2f38-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2f38-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2f38-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2f38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2f38-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2f38-115">Not supported.</span></span>|
|<span data-ttu-id="f2f38-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2f38-116">Application</span></span>|<span data-ttu-id="f2f38-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2f38-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2f38-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2f38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f2f38-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2f38-119">Request headers</span></span>
|<span data-ttu-id="f2f38-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2f38-120">Header</span></span>|<span data-ttu-id="f2f38-121">値</span><span class="sxs-lookup"><span data-stu-id="f2f38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2f38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2f38-122">Authorization</span></span>|<span data-ttu-id="f2f38-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2f38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2f38-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f2f38-124">Accept</span></span>|<span data-ttu-id="f2f38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2f38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2f38-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2f38-126">Request body</span></span>
<span data-ttu-id="f2f38-127">要求本文で、 [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2f38-127">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="f2f38-128">次の表に、 [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f2f38-128">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="f2f38-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2f38-129">Property</span></span>|<span data-ttu-id="f2f38-130">型</span><span class="sxs-lookup"><span data-stu-id="f2f38-130">Type</span></span>|<span data-ttu-id="f2f38-131">説明</span><span class="sxs-lookup"><span data-stu-id="f2f38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2f38-132">id</span><span class="sxs-lookup"><span data-stu-id="f2f38-132">id</span></span>|<span data-ttu-id="f2f38-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f2f38-133">String</span></span>|<span data-ttu-id="f2f38-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f2f38-134">Key of the entity.</span></span> <span data-ttu-id="f2f38-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2f38-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f2f38-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f38-137">DateTimeOffset</span></span>|<span data-ttu-id="f2f38-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f2f38-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f2f38-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2f38-140">roleScopeTagIds</span></span>|<span data-ttu-id="f2f38-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f2f38-141">String collection</span></span>|<span data-ttu-id="f2f38-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f2f38-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f2f38-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f2f38-144">supportsScopeTags</span></span>|<span data-ttu-id="f2f38-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2f38-145">Boolean</span></span>|<span data-ttu-id="f2f38-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f2f38-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f2f38-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f2f38-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f2f38-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f2f38-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f2f38-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f2f38-149">This property is read-only.</span></span> <span data-ttu-id="f2f38-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f2f38-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f2f38-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f2f38-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f2f38-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="f2f38-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f2f38-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f2f38-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f2f38-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f2f38-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f2f38-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f2f38-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f2f38-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f2f38-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f2f38-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f2f38-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f2f38-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f2f38-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f2f38-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2f38-163">createdDateTime</span></span>|<span data-ttu-id="f2f38-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f38-164">DateTimeOffset</span></span>|<span data-ttu-id="f2f38-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f2f38-165">DateTime the object was created.</span></span> <span data-ttu-id="f2f38-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-167">description</span><span class="sxs-lookup"><span data-stu-id="f2f38-167">description</span></span>|<span data-ttu-id="f2f38-168">String</span><span class="sxs-lookup"><span data-stu-id="f2f38-168">String</span></span>|<span data-ttu-id="f2f38-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f2f38-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2f38-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f2f38-171">displayName</span></span>|<span data-ttu-id="f2f38-172">String</span><span class="sxs-lookup"><span data-stu-id="f2f38-172">String</span></span>|<span data-ttu-id="f2f38-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f2f38-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2f38-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-175">version</span><span class="sxs-lookup"><span data-stu-id="f2f38-175">version</span></span>|<span data-ttu-id="f2f38-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f2f38-176">Int32</span></span>|<span data-ttu-id="f2f38-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f2f38-177">Version of the device configuration.</span></span> <span data-ttu-id="f2f38-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2f38-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2f38-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f2f38-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="f2f38-180">Int32</span><span class="sxs-lookup"><span data-stu-id="f2f38-180">Int32</span></span>|<span data-ttu-id="f2f38-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="f2f38-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f2f38-182">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="f2f38-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f2f38-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f2f38-183">keyStorageProvider</span></span>|[<span data-ttu-id="f2f38-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f2f38-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="f2f38-185">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承したキー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="f2f38-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f2f38-186">使用可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="f2f38-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="f2f38-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f2f38-187">subjectNameFormat</span></span>|[<span data-ttu-id="f2f38-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f2f38-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f2f38-189">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される証明書のサブジェクト名形式。</span><span class="sxs-lookup"><span data-stu-id="f2f38-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f2f38-190">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="f2f38-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f2f38-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f2f38-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f2f38-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f2f38-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f2f38-193">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書のサブジェクトの別名型。</span><span class="sxs-lookup"><span data-stu-id="f2f38-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f2f38-194">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="f2f38-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f2f38-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f2f38-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f2f38-196">Int32</span><span class="sxs-lookup"><span data-stu-id="f2f38-196">Int32</span></span>|<span data-ttu-id="f2f38-197">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間の値</span><span class="sxs-lookup"><span data-stu-id="f2f38-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f2f38-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f2f38-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f2f38-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f2f38-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f2f38-200">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="f2f38-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f2f38-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="f2f38-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f2f38-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="f2f38-202">intendedPurpose</span></span>|[<span data-ttu-id="f2f38-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="f2f38-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="f2f38-204">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="f2f38-204">Not yet documented.</span></span> <span data-ttu-id="f2f38-205">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="f2f38-205">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="f2f38-206">応答</span><span class="sxs-lookup"><span data-stu-id="f2f38-206">Response</span></span>
<span data-ttu-id="f2f38-207">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f2f38-207">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2f38-208">例</span><span class="sxs-lookup"><span data-stu-id="f2f38-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2f38-209">要求</span><span class="sxs-lookup"><span data-stu-id="f2f38-209">Request</span></span>
<span data-ttu-id="f2f38-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2f38-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1359

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="f2f38-211">応答</span><span class="sxs-lookup"><span data-stu-id="f2f38-211">Response</span></span>
<span data-ttu-id="f2f38-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2f38-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1531

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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
  "intendedPurpose": "smimeEncryption"
}
```





