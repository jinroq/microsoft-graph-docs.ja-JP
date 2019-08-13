---
title: IosScepCertificateProfile の更新
description: IosScepCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6719cad7d36d0eebccad2e98354fe17bdd6b605
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315773"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="bf585-103">IosScepCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="bf585-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="bf585-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf585-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf585-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf585-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf585-106">[Iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bf585-106">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf585-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bf585-107">Prerequisites</span></span>
<span data-ttu-id="bf585-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf585-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bf585-110">Permission type</span></span>|<span data-ttu-id="bf585-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bf585-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf585-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bf585-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf585-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf585-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf585-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf585-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf585-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf585-115">Not supported.</span></span>|
|<span data-ttu-id="bf585-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bf585-116">Application</span></span>|<span data-ttu-id="bf585-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf585-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf585-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf585-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bf585-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf585-119">Request headers</span></span>
|<span data-ttu-id="bf585-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf585-120">Header</span></span>|<span data-ttu-id="bf585-121">値</span><span class="sxs-lookup"><span data-stu-id="bf585-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf585-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf585-122">Authorization</span></span>|<span data-ttu-id="bf585-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf585-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf585-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bf585-124">Accept</span></span>|<span data-ttu-id="bf585-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf585-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf585-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bf585-126">Request body</span></span>
<span data-ttu-id="bf585-127">要求本文で、 [Iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bf585-127">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="bf585-128">次の表に、 [Iosscepcertificateprofile プロファイル](../resources/intune-deviceconfig-iosscepcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bf585-128">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="bf585-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf585-129">Property</span></span>|<span data-ttu-id="bf585-130">型</span><span class="sxs-lookup"><span data-stu-id="bf585-130">Type</span></span>|<span data-ttu-id="bf585-131">説明</span><span class="sxs-lookup"><span data-stu-id="bf585-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf585-132">id</span><span class="sxs-lookup"><span data-stu-id="bf585-132">id</span></span>|<span data-ttu-id="bf585-133">文字列</span><span class="sxs-lookup"><span data-stu-id="bf585-133">String</span></span>|<span data-ttu-id="bf585-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bf585-134">Key of the entity.</span></span> <span data-ttu-id="bf585-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf585-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bf585-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf585-137">DateTimeOffset</span></span>|<span data-ttu-id="bf585-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="bf585-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bf585-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bf585-140">roleScopeTagIds</span></span>|<span data-ttu-id="bf585-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="bf585-141">String collection</span></span>|<span data-ttu-id="bf585-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="bf585-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bf585-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bf585-144">supportsScopeTags</span></span>|<span data-ttu-id="bf585-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf585-145">Boolean</span></span>|<span data-ttu-id="bf585-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bf585-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bf585-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="bf585-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bf585-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="bf585-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bf585-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="bf585-149">This property is read-only.</span></span> <span data-ttu-id="bf585-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bf585-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bf585-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bf585-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bf585-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="bf585-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bf585-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bf585-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bf585-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bf585-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bf585-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="bf585-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bf585-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="bf585-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bf585-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="bf585-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bf585-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="bf585-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bf585-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf585-163">createdDateTime</span></span>|<span data-ttu-id="bf585-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf585-164">DateTimeOffset</span></span>|<span data-ttu-id="bf585-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bf585-165">DateTime the object was created.</span></span> <span data-ttu-id="bf585-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-167">description</span><span class="sxs-lookup"><span data-stu-id="bf585-167">description</span></span>|<span data-ttu-id="bf585-168">String</span><span class="sxs-lookup"><span data-stu-id="bf585-168">String</span></span>|<span data-ttu-id="bf585-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="bf585-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bf585-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-171">displayName</span><span class="sxs-lookup"><span data-stu-id="bf585-171">displayName</span></span>|<span data-ttu-id="bf585-172">String</span><span class="sxs-lookup"><span data-stu-id="bf585-172">String</span></span>|<span data-ttu-id="bf585-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="bf585-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bf585-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-175">version</span><span class="sxs-lookup"><span data-stu-id="bf585-175">version</span></span>|<span data-ttu-id="bf585-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bf585-176">Int32</span></span>|<span data-ttu-id="bf585-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="bf585-177">Version of the device configuration.</span></span> <span data-ttu-id="bf585-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf585-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="bf585-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="bf585-180">Int32</span><span class="sxs-lookup"><span data-stu-id="bf585-180">Int32</span></span>|<span data-ttu-id="bf585-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="bf585-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="bf585-182">有効な値は、 [Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承された値 1 ~ 99 です。</span><span class="sxs-lookup"><span data-stu-id="bf585-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bf585-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bf585-183">subjectNameFormat</span></span>|[<span data-ttu-id="bf585-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bf585-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="bf585-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="bf585-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="bf585-186">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bf585-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="bf585-187">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="bf585-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="bf585-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bf585-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="bf585-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bf585-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bf585-190">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="bf585-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="bf585-191">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bf585-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="bf585-192">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="bf585-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="bf585-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="bf585-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="bf585-194">Int32</span><span class="sxs-lookup"><span data-stu-id="bf585-194">Int32</span></span>|<span data-ttu-id="bf585-195">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="bf585-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="bf585-196">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="bf585-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bf585-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bf585-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="bf585-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bf585-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="bf585-199">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="bf585-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="bf585-200">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bf585-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="bf585-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="bf585-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="bf585-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="bf585-202">scepServerUrls</span></span>|<span data-ttu-id="bf585-203">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="bf585-203">String collection</span></span>|<span data-ttu-id="bf585-204">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="bf585-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="bf585-205">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf585-205">subjectNameFormatString</span></span>|<span data-ttu-id="bf585-206">String</span><span class="sxs-lookup"><span data-stu-id="bf585-206">String</span></span>|<span data-ttu-id="bf585-207">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="bf585-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="bf585-208">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="bf585-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="bf585-209">keyUsage</span><span class="sxs-lookup"><span data-stu-id="bf585-209">keyUsage</span></span>|[<span data-ttu-id="bf585-210">keyUsages</span><span class="sxs-lookup"><span data-stu-id="bf585-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="bf585-211">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="bf585-211">SCEP Key Usage.</span></span> <span data-ttu-id="bf585-212">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="bf585-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="bf585-213">keySize</span><span class="sxs-lookup"><span data-stu-id="bf585-213">keySize</span></span>|[<span data-ttu-id="bf585-214">keySize</span><span class="sxs-lookup"><span data-stu-id="bf585-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="bf585-215">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="bf585-215">SCEP Key Size.</span></span> <span data-ttu-id="bf585-216">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="bf585-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="bf585-217">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="bf585-217">extendedKeyUsages</span></span>|<span data-ttu-id="bf585-218">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bf585-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="bf585-219">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="bf585-219">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="bf585-220">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bf585-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bf585-221">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bf585-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="bf585-222">String</span><span class="sxs-lookup"><span data-stu-id="bf585-222">String</span></span>|<span data-ttu-id="bf585-223">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="bf585-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="bf585-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bf585-224">certificateStore</span></span>|[<span data-ttu-id="bf585-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bf585-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="bf585-226">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="bf585-226">Target store certificate.</span></span> <span data-ttu-id="bf585-227">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="bf585-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="bf585-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="bf585-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="bf585-229">[Customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="bf585-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="bf585-230">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="bf585-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="bf585-231">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bf585-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="bf585-232">応答</span><span class="sxs-lookup"><span data-stu-id="bf585-232">Response</span></span>
<span data-ttu-id="bf585-233">成功した場合、このメソッド`200 OK`は応答コードと、更新された[Iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="bf585-233">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf585-234">例</span><span class="sxs-lookup"><span data-stu-id="bf585-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf585-235">要求</span><span class="sxs-lookup"><span data-stu-id="bf585-235">Request</span></span>
<span data-ttu-id="bf585-236">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bf585-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1932

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bf585-237">応答</span><span class="sxs-lookup"><span data-stu-id="bf585-237">Response</span></span>
<span data-ttu-id="bf585-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bf585-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```






