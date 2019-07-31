---
title: MacOSImportedPFXCertificateProfile の更新
description: MacOSImportedPFXCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21b83a8ffb7154762e7e72af588da8ae08bbf71c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947123"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="11082-103">MacOSImportedPFXCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="11082-103">Update macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="11082-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11082-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11082-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="11082-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11082-106">[MacOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="11082-106">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11082-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="11082-107">Prerequisites</span></span>
<span data-ttu-id="11082-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11082-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11082-110">Permission type</span></span>|<span data-ttu-id="11082-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="11082-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11082-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11082-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11082-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11082-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11082-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11082-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11082-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11082-115">Not supported.</span></span>|
|<span data-ttu-id="11082-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11082-116">Application</span></span>|<span data-ttu-id="11082-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11082-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11082-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11082-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="11082-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11082-119">Request headers</span></span>
|<span data-ttu-id="11082-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11082-120">Header</span></span>|<span data-ttu-id="11082-121">値</span><span class="sxs-lookup"><span data-stu-id="11082-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11082-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11082-122">Authorization</span></span>|<span data-ttu-id="11082-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="11082-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11082-124">承諾</span><span class="sxs-lookup"><span data-stu-id="11082-124">Accept</span></span>|<span data-ttu-id="11082-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11082-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11082-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="11082-126">Request body</span></span>
<span data-ttu-id="11082-127">要求本文で、 [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="11082-127">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="11082-128">次の表に、 [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="11082-128">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="11082-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11082-129">Property</span></span>|<span data-ttu-id="11082-130">型</span><span class="sxs-lookup"><span data-stu-id="11082-130">Type</span></span>|<span data-ttu-id="11082-131">説明</span><span class="sxs-lookup"><span data-stu-id="11082-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11082-132">id</span><span class="sxs-lookup"><span data-stu-id="11082-132">id</span></span>|<span data-ttu-id="11082-133">文字列</span><span class="sxs-lookup"><span data-stu-id="11082-133">String</span></span>|<span data-ttu-id="11082-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="11082-134">Key of the entity.</span></span> <span data-ttu-id="11082-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11082-136">lastModifiedDateTime</span></span>|<span data-ttu-id="11082-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11082-137">DateTimeOffset</span></span>|<span data-ttu-id="11082-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="11082-138">DateTime the object was last modified.</span></span> <span data-ttu-id="11082-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="11082-140">roleScopeTagIds</span></span>|<span data-ttu-id="11082-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="11082-141">String collection</span></span>|<span data-ttu-id="11082-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="11082-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="11082-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="11082-144">supportsScopeTags</span></span>|<span data-ttu-id="11082-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="11082-145">Boolean</span></span>|<span data-ttu-id="11082-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="11082-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="11082-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="11082-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="11082-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="11082-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="11082-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="11082-149">This property is read-only.</span></span> <span data-ttu-id="11082-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="11082-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="11082-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="11082-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="11082-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="11082-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="11082-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="11082-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="11082-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="11082-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="11082-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="11082-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="11082-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="11082-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="11082-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="11082-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="11082-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="11082-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="11082-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11082-163">createdDateTime</span></span>|<span data-ttu-id="11082-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11082-164">DateTimeOffset</span></span>|<span data-ttu-id="11082-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="11082-165">DateTime the object was created.</span></span> <span data-ttu-id="11082-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-167">description</span><span class="sxs-lookup"><span data-stu-id="11082-167">description</span></span>|<span data-ttu-id="11082-168">String</span><span class="sxs-lookup"><span data-stu-id="11082-168">String</span></span>|<span data-ttu-id="11082-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="11082-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="11082-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-171">displayName</span><span class="sxs-lookup"><span data-stu-id="11082-171">displayName</span></span>|<span data-ttu-id="11082-172">String</span><span class="sxs-lookup"><span data-stu-id="11082-172">String</span></span>|<span data-ttu-id="11082-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="11082-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="11082-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-175">version</span><span class="sxs-lookup"><span data-stu-id="11082-175">version</span></span>|<span data-ttu-id="11082-176">Int32</span><span class="sxs-lookup"><span data-stu-id="11082-176">Int32</span></span>|<span data-ttu-id="11082-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="11082-177">Version of the device configuration.</span></span> <span data-ttu-id="11082-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="11082-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="11082-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="11082-180">Int32</span><span class="sxs-lookup"><span data-stu-id="11082-180">Int32</span></span>|<span data-ttu-id="11082-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="11082-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="11082-182">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="11082-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="11082-183">subjectNameFormat</span></span>|[<span data-ttu-id="11082-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="11082-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="11082-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="11082-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="11082-186">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="11082-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="11082-187">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="11082-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="11082-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="11082-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="11082-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="11082-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="11082-190">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="11082-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="11082-191">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="11082-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="11082-192">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="11082-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="11082-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="11082-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="11082-194">Int32</span><span class="sxs-lookup"><span data-stu-id="11082-194">Int32</span></span>|<span data-ttu-id="11082-195">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="11082-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="11082-196">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="11082-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="11082-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="11082-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="11082-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="11082-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="11082-199">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="11082-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="11082-200">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="11082-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="11082-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="11082-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="11082-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="11082-202">intendedPurpose</span></span>|[<span data-ttu-id="11082-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="11082-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="11082-204">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="11082-204">Not yet documented.</span></span> <span data-ttu-id="11082-205">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="11082-205">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="11082-206">応答</span><span class="sxs-lookup"><span data-stu-id="11082-206">Response</span></span>
<span data-ttu-id="11082-207">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="11082-207">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11082-208">例</span><span class="sxs-lookup"><span data-stu-id="11082-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="11082-209">要求</span><span class="sxs-lookup"><span data-stu-id="11082-209">Request</span></span>
<span data-ttu-id="11082-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="11082-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1297

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="11082-211">応答</span><span class="sxs-lookup"><span data-stu-id="11082-211">Response</span></span>
<span data-ttu-id="11082-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="11082-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1469

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```





