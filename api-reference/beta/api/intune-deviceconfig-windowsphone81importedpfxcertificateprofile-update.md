---
title: WindowsPhone81ImportedPFXCertificateProfile の更新
description: WindowsPhone81ImportedPFXCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b21bdc460013034cdb8ec3ec3549c1dbf985b11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982054"
---
# <a name="update-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="95a00-103">WindowsPhone81ImportedPFXCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="95a00-103">Update windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="95a00-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95a00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95a00-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95a00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95a00-106">[WindowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="95a00-106">Update the properties of a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95a00-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="95a00-107">Prerequisites</span></span>
<span data-ttu-id="95a00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95a00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95a00-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95a00-110">Permission type</span></span>|<span data-ttu-id="95a00-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95a00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95a00-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95a00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95a00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95a00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95a00-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95a00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95a00-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95a00-115">Not supported.</span></span>|
|<span data-ttu-id="95a00-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95a00-116">Application</span></span>|<span data-ttu-id="95a00-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95a00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95a00-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95a00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="95a00-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95a00-119">Request headers</span></span>
|<span data-ttu-id="95a00-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95a00-120">Header</span></span>|<span data-ttu-id="95a00-121">値</span><span class="sxs-lookup"><span data-stu-id="95a00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95a00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95a00-122">Authorization</span></span>|<span data-ttu-id="95a00-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95a00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95a00-124">承諾</span><span class="sxs-lookup"><span data-stu-id="95a00-124">Accept</span></span>|<span data-ttu-id="95a00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95a00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95a00-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="95a00-126">Request body</span></span>
<span data-ttu-id="95a00-127">要求本文で、 [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="95a00-127">In the request body, supply a JSON representation for the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="95a00-128">次の表に、 [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="95a00-128">The following table shows the properties that are required when you create the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="95a00-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95a00-129">Property</span></span>|<span data-ttu-id="95a00-130">型</span><span class="sxs-lookup"><span data-stu-id="95a00-130">Type</span></span>|<span data-ttu-id="95a00-131">説明</span><span class="sxs-lookup"><span data-stu-id="95a00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95a00-132">id</span><span class="sxs-lookup"><span data-stu-id="95a00-132">id</span></span>|<span data-ttu-id="95a00-133">文字列</span><span class="sxs-lookup"><span data-stu-id="95a00-133">String</span></span>|<span data-ttu-id="95a00-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="95a00-134">Key of the entity.</span></span> <span data-ttu-id="95a00-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95a00-136">lastModifiedDateTime</span></span>|<span data-ttu-id="95a00-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95a00-137">DateTimeOffset</span></span>|<span data-ttu-id="95a00-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="95a00-138">DateTime the object was last modified.</span></span> <span data-ttu-id="95a00-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95a00-140">roleScopeTagIds</span></span>|<span data-ttu-id="95a00-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="95a00-141">String collection</span></span>|<span data-ttu-id="95a00-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="95a00-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95a00-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95a00-144">supportsScopeTags</span></span>|<span data-ttu-id="95a00-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="95a00-145">Boolean</span></span>|<span data-ttu-id="95a00-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="95a00-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95a00-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="95a00-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95a00-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="95a00-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95a00-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="95a00-149">This property is read-only.</span></span> <span data-ttu-id="95a00-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95a00-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="95a00-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95a00-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="95a00-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="95a00-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="95a00-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95a00-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="95a00-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95a00-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="95a00-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="95a00-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="95a00-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="95a00-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="95a00-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="95a00-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="95a00-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="95a00-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="95a00-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95a00-163">createdDateTime</span></span>|<span data-ttu-id="95a00-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95a00-164">DateTimeOffset</span></span>|<span data-ttu-id="95a00-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="95a00-165">DateTime the object was created.</span></span> <span data-ttu-id="95a00-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-167">description</span><span class="sxs-lookup"><span data-stu-id="95a00-167">description</span></span>|<span data-ttu-id="95a00-168">String</span><span class="sxs-lookup"><span data-stu-id="95a00-168">String</span></span>|<span data-ttu-id="95a00-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="95a00-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95a00-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-171">displayName</span><span class="sxs-lookup"><span data-stu-id="95a00-171">displayName</span></span>|<span data-ttu-id="95a00-172">String</span><span class="sxs-lookup"><span data-stu-id="95a00-172">String</span></span>|<span data-ttu-id="95a00-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="95a00-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95a00-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-175">version</span><span class="sxs-lookup"><span data-stu-id="95a00-175">version</span></span>|<span data-ttu-id="95a00-176">Int32</span><span class="sxs-lookup"><span data-stu-id="95a00-176">Int32</span></span>|<span data-ttu-id="95a00-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="95a00-177">Version of the device configuration.</span></span> <span data-ttu-id="95a00-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95a00-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95a00-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="95a00-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="95a00-180">Int32</span><span class="sxs-lookup"><span data-stu-id="95a00-180">Int32</span></span>|<span data-ttu-id="95a00-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="95a00-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="95a00-182">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="95a00-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="95a00-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="95a00-183">keyStorageProvider</span></span>|[<span data-ttu-id="95a00-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="95a00-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="95a00-185">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承したキー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="95a00-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="95a00-186">使用可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="95a00-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="95a00-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="95a00-187">subjectNameFormat</span></span>|[<span data-ttu-id="95a00-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="95a00-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="95a00-189">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される証明書のサブジェクト名形式。</span><span class="sxs-lookup"><span data-stu-id="95a00-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="95a00-190">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="95a00-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="95a00-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="95a00-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="95a00-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="95a00-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="95a00-193">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書のサブジェクトの別名型。</span><span class="sxs-lookup"><span data-stu-id="95a00-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="95a00-194">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="95a00-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="95a00-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="95a00-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="95a00-196">Int32</span><span class="sxs-lookup"><span data-stu-id="95a00-196">Int32</span></span>|<span data-ttu-id="95a00-197">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間の値</span><span class="sxs-lookup"><span data-stu-id="95a00-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="95a00-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="95a00-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="95a00-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="95a00-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="95a00-200">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="95a00-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="95a00-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="95a00-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="95a00-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="95a00-202">intendedPurpose</span></span>|[<span data-ttu-id="95a00-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="95a00-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="95a00-204">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="95a00-204">Not yet documented.</span></span> <span data-ttu-id="95a00-205">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="95a00-205">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="95a00-206">応答</span><span class="sxs-lookup"><span data-stu-id="95a00-206">Response</span></span>
<span data-ttu-id="95a00-207">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95a00-207">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95a00-208">例</span><span class="sxs-lookup"><span data-stu-id="95a00-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="95a00-209">要求</span><span class="sxs-lookup"><span data-stu-id="95a00-209">Request</span></span>
<span data-ttu-id="95a00-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95a00-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1364

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="95a00-211">応答</span><span class="sxs-lookup"><span data-stu-id="95a00-211">Response</span></span>
<span data-ttu-id="95a00-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95a00-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1536

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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





