---
title: WindowsPhone81SCEPCertificateProfile の更新
description: WindowsPhone81SCEPCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e6e3b57a693e6fbc6cf478c872ed6e9ecfc73d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313875"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="1d2e3-103">WindowsPhone81SCEPCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="1d2e3-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="1d2e3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d2e3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d2e3-106">[WindowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-106">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d2e3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1d2e3-107">Prerequisites</span></span>
<span data-ttu-id="1d2e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d2e3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d2e3-110">Permission type</span></span>|<span data-ttu-id="1d2e3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d2e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d2e3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d2e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d2e3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d2e3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d2e3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d2e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d2e3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-115">Not supported.</span></span>|
|<span data-ttu-id="1d2e3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d2e3-116">Application</span></span>|<span data-ttu-id="1d2e3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d2e3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d2e3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d2e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1d2e3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d2e3-119">Request headers</span></span>
|<span data-ttu-id="1d2e3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d2e3-120">Header</span></span>|<span data-ttu-id="1d2e3-121">値</span><span class="sxs-lookup"><span data-stu-id="1d2e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d2e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d2e3-122">Authorization</span></span>|<span data-ttu-id="1d2e3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d2e3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1d2e3-124">Accept</span></span>|<span data-ttu-id="1d2e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d2e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d2e3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d2e3-126">Request body</span></span>
<span data-ttu-id="1d2e3-127">要求本文で、 [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-127">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="1d2e3-128">次の表に、 [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-128">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="1d2e3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d2e3-129">Property</span></span>|<span data-ttu-id="1d2e3-130">型</span><span class="sxs-lookup"><span data-stu-id="1d2e3-130">Type</span></span>|<span data-ttu-id="1d2e3-131">説明</span><span class="sxs-lookup"><span data-stu-id="1d2e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d2e3-132">id</span><span class="sxs-lookup"><span data-stu-id="1d2e3-132">id</span></span>|<span data-ttu-id="1d2e3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1d2e3-133">String</span></span>|<span data-ttu-id="1d2e3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-134">Key of the entity.</span></span> <span data-ttu-id="1d2e3-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d2e3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1d2e3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d2e3-137">DateTimeOffset</span></span>|<span data-ttu-id="1d2e3-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1d2e3-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1d2e3-140">roleScopeTagIds</span></span>|<span data-ttu-id="1d2e3-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1d2e3-141">String collection</span></span>|<span data-ttu-id="1d2e3-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1d2e3-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1d2e3-144">supportsScopeTags</span></span>|<span data-ttu-id="1d2e3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d2e3-145">Boolean</span></span>|<span data-ttu-id="1d2e3-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1d2e3-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1d2e3-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1d2e3-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-149">This property is read-only.</span></span> <span data-ttu-id="1d2e3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1d2e3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1d2e3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1d2e3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1d2e3-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1d2e3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1d2e3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1d2e3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1d2e3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1d2e3-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1d2e3-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="1d2e3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1d2e3-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="1d2e3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1d2e3-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1d2e3-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d2e3-163">createdDateTime</span></span>|<span data-ttu-id="1d2e3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d2e3-164">DateTimeOffset</span></span>|<span data-ttu-id="1d2e3-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-165">DateTime the object was created.</span></span> <span data-ttu-id="1d2e3-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-167">description</span><span class="sxs-lookup"><span data-stu-id="1d2e3-167">description</span></span>|<span data-ttu-id="1d2e3-168">String</span><span class="sxs-lookup"><span data-stu-id="1d2e3-168">String</span></span>|<span data-ttu-id="1d2e3-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1d2e3-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1d2e3-171">displayName</span></span>|<span data-ttu-id="1d2e3-172">String</span><span class="sxs-lookup"><span data-stu-id="1d2e3-172">String</span></span>|<span data-ttu-id="1d2e3-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1d2e3-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-175">version</span><span class="sxs-lookup"><span data-stu-id="1d2e3-175">version</span></span>|<span data-ttu-id="1d2e3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1d2e3-176">Int32</span></span>|<span data-ttu-id="1d2e3-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-177">Version of the device configuration.</span></span> <span data-ttu-id="1d2e3-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1d2e3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d2e3-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1d2e3-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="1d2e3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="1d2e3-180">Int32</span></span>|<span data-ttu-id="1d2e3-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1d2e3-182">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-182">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="1d2e3-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="1d2e3-183">keyStorageProvider</span></span>|[<span data-ttu-id="1d2e3-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="1d2e3-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="1d2e3-185">キーストレージプロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-185">Key Storage Provider (KSP).</span></span> <span data-ttu-id="1d2e3-186">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-186">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="1d2e3-187">使用可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="1d2e3-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1d2e3-188">subjectNameFormat</span></span>|[<span data-ttu-id="1d2e3-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1d2e3-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="1d2e3-190">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-190">Certificate Subject Name Format.</span></span> <span data-ttu-id="1d2e3-191">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-191">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="1d2e3-192">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-192">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="1d2e3-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1d2e3-193">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1d2e3-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1d2e3-194">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="1d2e3-195">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-195">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="1d2e3-196">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-196">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="1d2e3-197">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-197">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="1d2e3-198">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1d2e3-198">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1d2e3-199">Int32</span><span class="sxs-lookup"><span data-stu-id="1d2e3-199">Int32</span></span>|<span data-ttu-id="1d2e3-200">証明書の Validtiy の値。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-200">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="1d2e3-201">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-201">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="1d2e3-202">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1d2e3-202">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1d2e3-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1d2e3-203">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1d2e3-204">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-204">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="1d2e3-205">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-205">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="1d2e3-206">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-206">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="1d2e3-207">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="1d2e3-207">extendedKeyUsages</span></span>|<span data-ttu-id="1d2e3-208">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1d2e3-208">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="1d2e3-209">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-209">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="1d2e3-210">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1d2e3-211">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-211">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="1d2e3-212">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="1d2e3-212">scepServerUrls</span></span>|<span data-ttu-id="1d2e3-213">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1d2e3-213">String collection</span></span>|<span data-ttu-id="1d2e3-214">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="1d2e3-215">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d2e3-215">subjectNameFormatString</span></span>|<span data-ttu-id="1d2e3-216">String</span><span class="sxs-lookup"><span data-stu-id="1d2e3-216">String</span></span>|<span data-ttu-id="1d2e3-217">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="1d2e3-218">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="1d2e3-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="1d2e3-219">keyUsage</span><span class="sxs-lookup"><span data-stu-id="1d2e3-219">keyUsage</span></span>|[<span data-ttu-id="1d2e3-220">keyUsages</span><span class="sxs-lookup"><span data-stu-id="1d2e3-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="1d2e3-221">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-221">SCEP Key Usage.</span></span> <span data-ttu-id="1d2e3-222">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="1d2e3-223">keySize</span><span class="sxs-lookup"><span data-stu-id="1d2e3-223">keySize</span></span>|[<span data-ttu-id="1d2e3-224">keySize</span><span class="sxs-lookup"><span data-stu-id="1d2e3-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="1d2e3-225">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-225">SCEP Key Size.</span></span> <span data-ttu-id="1d2e3-226">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="1d2e3-227">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="1d2e3-227">hashAlgorithm</span></span>|[<span data-ttu-id="1d2e3-228">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="1d2e3-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="1d2e3-229">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="1d2e3-230">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="1d2e3-231">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="1d2e3-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="1d2e3-232">String</span><span class="sxs-lookup"><span data-stu-id="1d2e3-232">String</span></span>|<span data-ttu-id="1d2e3-233">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-233">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="1d2e3-234">応答</span><span class="sxs-lookup"><span data-stu-id="1d2e3-234">Response</span></span>
<span data-ttu-id="1d2e3-235">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-235">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d2e3-236">例</span><span class="sxs-lookup"><span data-stu-id="1d2e3-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d2e3-237">要求</span><span class="sxs-lookup"><span data-stu-id="1d2e3-237">Request</span></span>
<span data-ttu-id="1d2e3-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1805

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="1d2e3-239">応答</span><span class="sxs-lookup"><span data-stu-id="1d2e3-239">Response</span></span>
<span data-ttu-id="1d2e3-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d2e3-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```






