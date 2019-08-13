---
title: WindowsPhone81SCEPCertificateProfile を作成する
description: 新しい windowsPhone81SCEPCertificateProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 150dd1a8d971d46da568f3d3cb638427e5baef01
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313931"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="41c89-103">WindowsPhone81SCEPCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="41c89-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="41c89-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41c89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41c89-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="41c89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41c89-106">新しい[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="41c89-106">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41c89-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="41c89-107">Prerequisites</span></span>
<span data-ttu-id="41c89-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41c89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c89-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41c89-110">Permission type</span></span>|<span data-ttu-id="41c89-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="41c89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41c89-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41c89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41c89-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41c89-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41c89-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41c89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41c89-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41c89-115">Not supported.</span></span>|
|<span data-ttu-id="41c89-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41c89-116">Application</span></span>|<span data-ttu-id="41c89-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41c89-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41c89-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41c89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="41c89-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41c89-119">Request headers</span></span>
|<span data-ttu-id="41c89-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41c89-120">Header</span></span>|<span data-ttu-id="41c89-121">値</span><span class="sxs-lookup"><span data-stu-id="41c89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41c89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41c89-122">Authorization</span></span>|<span data-ttu-id="41c89-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="41c89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41c89-124">承諾</span><span class="sxs-lookup"><span data-stu-id="41c89-124">Accept</span></span>|<span data-ttu-id="41c89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41c89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41c89-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="41c89-126">Request body</span></span>
<span data-ttu-id="41c89-127">要求本文で、windowsPhone81SCEPCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="41c89-127">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="41c89-128">次の表に、windowsPhone81SCEPCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="41c89-128">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="41c89-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41c89-129">Property</span></span>|<span data-ttu-id="41c89-130">型</span><span class="sxs-lookup"><span data-stu-id="41c89-130">Type</span></span>|<span data-ttu-id="41c89-131">説明</span><span class="sxs-lookup"><span data-stu-id="41c89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41c89-132">id</span><span class="sxs-lookup"><span data-stu-id="41c89-132">id</span></span>|<span data-ttu-id="41c89-133">文字列</span><span class="sxs-lookup"><span data-stu-id="41c89-133">String</span></span>|<span data-ttu-id="41c89-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="41c89-134">Key of the entity.</span></span> <span data-ttu-id="41c89-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41c89-136">lastModifiedDateTime</span></span>|<span data-ttu-id="41c89-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41c89-137">DateTimeOffset</span></span>|<span data-ttu-id="41c89-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="41c89-138">DateTime the object was last modified.</span></span> <span data-ttu-id="41c89-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41c89-140">roleScopeTagIds</span></span>|<span data-ttu-id="41c89-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="41c89-141">String collection</span></span>|<span data-ttu-id="41c89-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="41c89-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="41c89-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="41c89-144">supportsScopeTags</span></span>|<span data-ttu-id="41c89-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="41c89-145">Boolean</span></span>|<span data-ttu-id="41c89-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="41c89-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="41c89-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="41c89-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="41c89-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="41c89-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="41c89-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="41c89-149">This property is read-only.</span></span> <span data-ttu-id="41c89-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="41c89-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="41c89-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="41c89-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="41c89-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="41c89-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="41c89-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="41c89-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="41c89-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="41c89-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="41c89-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="41c89-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="41c89-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="41c89-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="41c89-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="41c89-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="41c89-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="41c89-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="41c89-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41c89-163">createdDateTime</span></span>|<span data-ttu-id="41c89-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41c89-164">DateTimeOffset</span></span>|<span data-ttu-id="41c89-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="41c89-165">DateTime the object was created.</span></span> <span data-ttu-id="41c89-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-167">description</span><span class="sxs-lookup"><span data-stu-id="41c89-167">description</span></span>|<span data-ttu-id="41c89-168">String</span><span class="sxs-lookup"><span data-stu-id="41c89-168">String</span></span>|<span data-ttu-id="41c89-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="41c89-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="41c89-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-171">displayName</span><span class="sxs-lookup"><span data-stu-id="41c89-171">displayName</span></span>|<span data-ttu-id="41c89-172">String</span><span class="sxs-lookup"><span data-stu-id="41c89-172">String</span></span>|<span data-ttu-id="41c89-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="41c89-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="41c89-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-175">version</span><span class="sxs-lookup"><span data-stu-id="41c89-175">version</span></span>|<span data-ttu-id="41c89-176">Int32</span><span class="sxs-lookup"><span data-stu-id="41c89-176">Int32</span></span>|<span data-ttu-id="41c89-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="41c89-177">Version of the device configuration.</span></span> <span data-ttu-id="41c89-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41c89-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41c89-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="41c89-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="41c89-180">Int32</span><span class="sxs-lookup"><span data-stu-id="41c89-180">Int32</span></span>|<span data-ttu-id="41c89-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="41c89-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="41c89-182">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="41c89-182">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="41c89-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="41c89-183">keyStorageProvider</span></span>|[<span data-ttu-id="41c89-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="41c89-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="41c89-185">キーストレージプロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="41c89-185">Key Storage Provider (KSP).</span></span> <span data-ttu-id="41c89-186">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="41c89-186">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="41c89-187">使用可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="41c89-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="41c89-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="41c89-188">subjectNameFormat</span></span>|[<span data-ttu-id="41c89-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="41c89-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="41c89-190">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="41c89-190">Certificate Subject Name Format.</span></span> <span data-ttu-id="41c89-191">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="41c89-191">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="41c89-192">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="41c89-192">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="41c89-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="41c89-193">subjectAlternativeNameType</span></span>|[<span data-ttu-id="41c89-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="41c89-194">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="41c89-195">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="41c89-195">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="41c89-196">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="41c89-196">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="41c89-197">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="41c89-197">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="41c89-198">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="41c89-198">certificateValidityPeriodValue</span></span>|<span data-ttu-id="41c89-199">Int32</span><span class="sxs-lookup"><span data-stu-id="41c89-199">Int32</span></span>|<span data-ttu-id="41c89-200">証明書の Validtiy の値。</span><span class="sxs-lookup"><span data-stu-id="41c89-200">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="41c89-201">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="41c89-201">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="41c89-202">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="41c89-202">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="41c89-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="41c89-203">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="41c89-204">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="41c89-204">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="41c89-205">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="41c89-205">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="41c89-206">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="41c89-206">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="41c89-207">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="41c89-207">extendedKeyUsages</span></span>|<span data-ttu-id="41c89-208">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="41c89-208">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="41c89-209">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="41c89-209">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="41c89-210">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="41c89-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="41c89-211">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="41c89-211">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="41c89-212">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="41c89-212">scepServerUrls</span></span>|<span data-ttu-id="41c89-213">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="41c89-213">String collection</span></span>|<span data-ttu-id="41c89-214">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="41c89-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="41c89-215">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="41c89-215">subjectNameFormatString</span></span>|<span data-ttu-id="41c89-216">String</span><span class="sxs-lookup"><span data-stu-id="41c89-216">String</span></span>|<span data-ttu-id="41c89-217">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="41c89-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="41c89-218">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="41c89-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="41c89-219">keyUsage</span><span class="sxs-lookup"><span data-stu-id="41c89-219">keyUsage</span></span>|[<span data-ttu-id="41c89-220">keyUsages</span><span class="sxs-lookup"><span data-stu-id="41c89-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="41c89-221">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="41c89-221">SCEP Key Usage.</span></span> <span data-ttu-id="41c89-222">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="41c89-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="41c89-223">keySize</span><span class="sxs-lookup"><span data-stu-id="41c89-223">keySize</span></span>|[<span data-ttu-id="41c89-224">keySize</span><span class="sxs-lookup"><span data-stu-id="41c89-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="41c89-225">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="41c89-225">SCEP Key Size.</span></span> <span data-ttu-id="41c89-226">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="41c89-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="41c89-227">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="41c89-227">hashAlgorithm</span></span>|[<span data-ttu-id="41c89-228">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="41c89-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="41c89-229">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="41c89-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="41c89-230">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="41c89-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="41c89-231">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="41c89-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="41c89-232">String</span><span class="sxs-lookup"><span data-stu-id="41c89-232">String</span></span>|<span data-ttu-id="41c89-233">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="41c89-233">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="41c89-234">応答</span><span class="sxs-lookup"><span data-stu-id="41c89-234">Response</span></span>
<span data-ttu-id="41c89-235">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="41c89-235">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41c89-236">例</span><span class="sxs-lookup"><span data-stu-id="41c89-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="41c89-237">要求</span><span class="sxs-lookup"><span data-stu-id="41c89-237">Request</span></span>
<span data-ttu-id="41c89-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41c89-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="41c89-239">応答</span><span class="sxs-lookup"><span data-stu-id="41c89-239">Response</span></span>
<span data-ttu-id="41c89-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="41c89-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






