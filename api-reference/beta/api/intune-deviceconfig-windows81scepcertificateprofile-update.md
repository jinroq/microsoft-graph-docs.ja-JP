---
title: Windows81SCEPCertificateProfile の更新
description: Windows81SCEPCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc436e360de4964692d355a0c7517c3e459b7053
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977752"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="89094-103">Windows81SCEPCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="89094-103">Update windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="89094-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89094-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89094-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="89094-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89094-106">[Windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="89094-106">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89094-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="89094-107">Prerequisites</span></span>
<span data-ttu-id="89094-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89094-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89094-110">Permission type</span></span>|<span data-ttu-id="89094-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="89094-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89094-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89094-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89094-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89094-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89094-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89094-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89094-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89094-115">Not supported.</span></span>|
|<span data-ttu-id="89094-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89094-116">Application</span></span>|<span data-ttu-id="89094-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89094-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89094-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89094-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="89094-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89094-119">Request headers</span></span>
|<span data-ttu-id="89094-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89094-120">Header</span></span>|<span data-ttu-id="89094-121">値</span><span class="sxs-lookup"><span data-stu-id="89094-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89094-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89094-122">Authorization</span></span>|<span data-ttu-id="89094-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="89094-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89094-124">承諾</span><span class="sxs-lookup"><span data-stu-id="89094-124">Accept</span></span>|<span data-ttu-id="89094-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89094-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89094-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="89094-126">Request body</span></span>
<span data-ttu-id="89094-127">要求本文で、 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="89094-127">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="89094-128">次の表に、 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="89094-128">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="89094-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89094-129">Property</span></span>|<span data-ttu-id="89094-130">型</span><span class="sxs-lookup"><span data-stu-id="89094-130">Type</span></span>|<span data-ttu-id="89094-131">説明</span><span class="sxs-lookup"><span data-stu-id="89094-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89094-132">id</span><span class="sxs-lookup"><span data-stu-id="89094-132">id</span></span>|<span data-ttu-id="89094-133">文字列</span><span class="sxs-lookup"><span data-stu-id="89094-133">String</span></span>|<span data-ttu-id="89094-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="89094-134">Key of the entity.</span></span> <span data-ttu-id="89094-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89094-136">lastModifiedDateTime</span></span>|<span data-ttu-id="89094-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89094-137">DateTimeOffset</span></span>|<span data-ttu-id="89094-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="89094-138">DateTime the object was last modified.</span></span> <span data-ttu-id="89094-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89094-140">roleScopeTagIds</span></span>|<span data-ttu-id="89094-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="89094-141">String collection</span></span>|<span data-ttu-id="89094-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="89094-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="89094-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="89094-144">supportsScopeTags</span></span>|<span data-ttu-id="89094-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="89094-145">Boolean</span></span>|<span data-ttu-id="89094-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="89094-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="89094-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="89094-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="89094-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="89094-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="89094-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="89094-149">This property is read-only.</span></span> <span data-ttu-id="89094-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89094-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="89094-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89094-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="89094-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="89094-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="89094-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89094-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="89094-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89094-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="89094-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="89094-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="89094-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="89094-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="89094-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="89094-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="89094-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="89094-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="89094-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89094-163">createdDateTime</span></span>|<span data-ttu-id="89094-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89094-164">DateTimeOffset</span></span>|<span data-ttu-id="89094-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="89094-165">DateTime the object was created.</span></span> <span data-ttu-id="89094-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-167">description</span><span class="sxs-lookup"><span data-stu-id="89094-167">description</span></span>|<span data-ttu-id="89094-168">String</span><span class="sxs-lookup"><span data-stu-id="89094-168">String</span></span>|<span data-ttu-id="89094-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="89094-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89094-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-171">displayName</span><span class="sxs-lookup"><span data-stu-id="89094-171">displayName</span></span>|<span data-ttu-id="89094-172">String</span><span class="sxs-lookup"><span data-stu-id="89094-172">String</span></span>|<span data-ttu-id="89094-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="89094-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89094-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-175">version</span><span class="sxs-lookup"><span data-stu-id="89094-175">version</span></span>|<span data-ttu-id="89094-176">Int32</span><span class="sxs-lookup"><span data-stu-id="89094-176">Int32</span></span>|<span data-ttu-id="89094-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="89094-177">Version of the device configuration.</span></span> <span data-ttu-id="89094-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89094-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89094-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="89094-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="89094-180">Int32</span><span class="sxs-lookup"><span data-stu-id="89094-180">Int32</span></span>|<span data-ttu-id="89094-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="89094-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="89094-182">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="89094-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="89094-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="89094-183">keyStorageProvider</span></span>|[<span data-ttu-id="89094-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="89094-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="89094-185">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承したキー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="89094-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="89094-186">使用可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="89094-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="89094-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="89094-187">subjectNameFormat</span></span>|[<span data-ttu-id="89094-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="89094-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="89094-189">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承される証明書のサブジェクト名形式。</span><span class="sxs-lookup"><span data-stu-id="89094-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="89094-190">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="89094-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="89094-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="89094-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="89094-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="89094-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="89094-193">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書のサブジェクトの別名型。</span><span class="sxs-lookup"><span data-stu-id="89094-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="89094-194">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="89094-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="89094-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="89094-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="89094-196">Int32</span><span class="sxs-lookup"><span data-stu-id="89094-196">Int32</span></span>|<span data-ttu-id="89094-197">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間の値</span><span class="sxs-lookup"><span data-stu-id="89094-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="89094-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="89094-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="89094-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="89094-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="89094-200">[Windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)から継承された証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="89094-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="89094-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="89094-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="89094-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="89094-202">extendedKeyUsages</span></span>|<span data-ttu-id="89094-203">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89094-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="89094-204">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="89094-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="89094-205">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="89094-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="89094-206">[Windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="89094-206">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="89094-207">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="89094-207">customSubjectAlternativeNames</span></span>|<span data-ttu-id="89094-208">[Customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="89094-208">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="89094-209">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="89094-209">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="89094-210">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="89094-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="89094-211">[Windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="89094-211">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="89094-212">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="89094-212">scepServerUrls</span></span>|<span data-ttu-id="89094-213">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="89094-213">String collection</span></span>|<span data-ttu-id="89094-214">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="89094-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="89094-215">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="89094-215">subjectNameFormatString</span></span>|<span data-ttu-id="89094-216">String</span><span class="sxs-lookup"><span data-stu-id="89094-216">String</span></span>|<span data-ttu-id="89094-217">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="89094-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="89094-218">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="89094-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="89094-219">keyUsage</span><span class="sxs-lookup"><span data-stu-id="89094-219">keyUsage</span></span>|[<span data-ttu-id="89094-220">keyUsages</span><span class="sxs-lookup"><span data-stu-id="89094-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="89094-221">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="89094-221">SCEP Key Usage.</span></span> <span data-ttu-id="89094-222">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="89094-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="89094-223">keySize</span><span class="sxs-lookup"><span data-stu-id="89094-223">keySize</span></span>|[<span data-ttu-id="89094-224">keySize</span><span class="sxs-lookup"><span data-stu-id="89094-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="89094-225">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="89094-225">SCEP Key Size.</span></span> <span data-ttu-id="89094-226">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="89094-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="89094-227">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="89094-227">hashAlgorithm</span></span>|[<span data-ttu-id="89094-228">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="89094-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="89094-229">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="89094-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="89094-230">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="89094-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="89094-231">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="89094-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="89094-232">String</span><span class="sxs-lookup"><span data-stu-id="89094-232">String</span></span>|<span data-ttu-id="89094-233">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="89094-233">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="89094-234">certificateStore</span><span class="sxs-lookup"><span data-stu-id="89094-234">certificateStore</span></span>|[<span data-ttu-id="89094-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="89094-235">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="89094-236">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="89094-236">Target store certificate.</span></span> <span data-ttu-id="89094-237">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="89094-237">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="89094-238">応答</span><span class="sxs-lookup"><span data-stu-id="89094-238">Response</span></span>
<span data-ttu-id="89094-239">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89094-239">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89094-240">例</span><span class="sxs-lookup"><span data-stu-id="89094-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="89094-241">要求</span><span class="sxs-lookup"><span data-stu-id="89094-241">Request</span></span>
<span data-ttu-id="89094-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89094-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2024

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="89094-243">応答</span><span class="sxs-lookup"><span data-stu-id="89094-243">Response</span></span>
<span data-ttu-id="89094-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89094-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2196

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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





