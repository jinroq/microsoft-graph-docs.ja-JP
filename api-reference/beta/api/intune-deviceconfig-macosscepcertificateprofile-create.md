---
title: MacOSScepCertificateProfile の作成
description: 新しい macOSScepCertificateProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ee957036997bbf0392f14cb592bfe8007273e34
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315219"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="ee969-103">MacOSScepCertificateProfile の作成</span><span class="sxs-lookup"><span data-stu-id="ee969-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="ee969-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee969-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee969-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee969-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee969-106">新しい[Macosscepcertificateprofile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee969-106">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee969-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee969-107">Prerequisites</span></span>
<span data-ttu-id="ee969-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee969-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee969-110">Permission type</span></span>|<span data-ttu-id="ee969-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee969-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee969-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee969-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee969-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee969-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee969-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee969-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee969-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee969-115">Not supported.</span></span>|
|<span data-ttu-id="ee969-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee969-116">Application</span></span>|<span data-ttu-id="ee969-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee969-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee969-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee969-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ee969-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee969-119">Request headers</span></span>
|<span data-ttu-id="ee969-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee969-120">Header</span></span>|<span data-ttu-id="ee969-121">値</span><span class="sxs-lookup"><span data-stu-id="ee969-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee969-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee969-122">Authorization</span></span>|<span data-ttu-id="ee969-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee969-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee969-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ee969-124">Accept</span></span>|<span data-ttu-id="ee969-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee969-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee969-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee969-126">Request body</span></span>
<span data-ttu-id="ee969-127">要求本文で、macOSScepCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee969-127">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="ee969-128">次の表に、macOSScepCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ee969-128">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="ee969-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee969-129">Property</span></span>|<span data-ttu-id="ee969-130">型</span><span class="sxs-lookup"><span data-stu-id="ee969-130">Type</span></span>|<span data-ttu-id="ee969-131">説明</span><span class="sxs-lookup"><span data-stu-id="ee969-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee969-132">id</span><span class="sxs-lookup"><span data-stu-id="ee969-132">id</span></span>|<span data-ttu-id="ee969-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ee969-133">String</span></span>|<span data-ttu-id="ee969-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ee969-134">Key of the entity.</span></span> <span data-ttu-id="ee969-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee969-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ee969-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee969-137">DateTimeOffset</span></span>|<span data-ttu-id="ee969-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ee969-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ee969-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee969-140">roleScopeTagIds</span></span>|<span data-ttu-id="ee969-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ee969-141">String collection</span></span>|<span data-ttu-id="ee969-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ee969-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee969-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ee969-144">supportsScopeTags</span></span>|<span data-ttu-id="ee969-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee969-145">Boolean</span></span>|<span data-ttu-id="ee969-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ee969-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ee969-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="ee969-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ee969-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="ee969-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ee969-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ee969-149">This property is read-only.</span></span> <span data-ttu-id="ee969-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ee969-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ee969-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ee969-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ee969-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="ee969-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ee969-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ee969-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ee969-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ee969-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ee969-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ee969-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ee969-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ee969-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ee969-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ee969-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ee969-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ee969-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ee969-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee969-163">createdDateTime</span></span>|<span data-ttu-id="ee969-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee969-164">DateTimeOffset</span></span>|<span data-ttu-id="ee969-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ee969-165">DateTime the object was created.</span></span> <span data-ttu-id="ee969-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-167">description</span><span class="sxs-lookup"><span data-stu-id="ee969-167">description</span></span>|<span data-ttu-id="ee969-168">String</span><span class="sxs-lookup"><span data-stu-id="ee969-168">String</span></span>|<span data-ttu-id="ee969-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ee969-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee969-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ee969-171">displayName</span></span>|<span data-ttu-id="ee969-172">String</span><span class="sxs-lookup"><span data-stu-id="ee969-172">String</span></span>|<span data-ttu-id="ee969-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ee969-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee969-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-175">version</span><span class="sxs-lookup"><span data-stu-id="ee969-175">version</span></span>|<span data-ttu-id="ee969-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ee969-176">Int32</span></span>|<span data-ttu-id="ee969-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ee969-177">Version of the device configuration.</span></span> <span data-ttu-id="ee969-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee969-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ee969-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="ee969-180">Int32</span><span class="sxs-lookup"><span data-stu-id="ee969-180">Int32</span></span>|<span data-ttu-id="ee969-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="ee969-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ee969-182">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ee969-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ee969-183">subjectNameFormat</span></span>|[<span data-ttu-id="ee969-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ee969-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="ee969-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="ee969-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="ee969-186">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ee969-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ee969-187">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="ee969-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="ee969-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ee969-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ee969-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ee969-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ee969-190">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="ee969-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="ee969-191">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ee969-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ee969-192">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="ee969-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ee969-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ee969-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ee969-194">Int32</span><span class="sxs-lookup"><span data-stu-id="ee969-194">Int32</span></span>|<span data-ttu-id="ee969-195">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="ee969-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="ee969-196">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="ee969-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ee969-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ee969-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ee969-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ee969-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ee969-199">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="ee969-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ee969-200">[Macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ee969-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ee969-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="ee969-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ee969-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="ee969-202">scepServerUrls</span></span>|<span data-ttu-id="ee969-203">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ee969-203">String collection</span></span>|<span data-ttu-id="ee969-204">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="ee969-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="ee969-205">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee969-205">subjectNameFormatString</span></span>|<span data-ttu-id="ee969-206">String</span><span class="sxs-lookup"><span data-stu-id="ee969-206">String</span></span>|<span data-ttu-id="ee969-207">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="ee969-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ee969-208">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="ee969-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ee969-209">keyUsage</span><span class="sxs-lookup"><span data-stu-id="ee969-209">keyUsage</span></span>|[<span data-ttu-id="ee969-210">keyUsages</span><span class="sxs-lookup"><span data-stu-id="ee969-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="ee969-211">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="ee969-211">SCEP Key Usage.</span></span> <span data-ttu-id="ee969-212">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="ee969-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ee969-213">keySize</span><span class="sxs-lookup"><span data-stu-id="ee969-213">keySize</span></span>|[<span data-ttu-id="ee969-214">keySize</span><span class="sxs-lookup"><span data-stu-id="ee969-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="ee969-215">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="ee969-215">SCEP Key Size.</span></span> <span data-ttu-id="ee969-216">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="ee969-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="ee969-217">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ee969-217">hashAlgorithm</span></span>|[<span data-ttu-id="ee969-218">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="ee969-218">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="ee969-219">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="ee969-219">SCEP Hash Algorithm.</span></span> <span data-ttu-id="ee969-220">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="ee969-220">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="ee969-221">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ee969-221">extendedKeyUsages</span></span>|<span data-ttu-id="ee969-222">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ee969-222">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ee969-223">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="ee969-223">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ee969-224">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ee969-224">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ee969-225">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ee969-225">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ee969-226">String</span><span class="sxs-lookup"><span data-stu-id="ee969-226">String</span></span>|<span data-ttu-id="ee969-227">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="ee969-227">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="ee969-228">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ee969-228">certificateStore</span></span>|[<span data-ttu-id="ee969-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ee969-229">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="ee969-230">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="ee969-230">Target store certificate.</span></span> <span data-ttu-id="ee969-231">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="ee969-231">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="ee969-232">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="ee969-232">customSubjectAlternativeNames</span></span>|<span data-ttu-id="ee969-233">[Customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="ee969-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="ee969-234">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="ee969-234">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="ee969-235">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ee969-235">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ee969-236">応答</span><span class="sxs-lookup"><span data-stu-id="ee969-236">Response</span></span>
<span data-ttu-id="ee969-237">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Macosscepcertificateprofile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee969-237">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee969-238">例</span><span class="sxs-lookup"><span data-stu-id="ee969-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee969-239">要求</span><span class="sxs-lookup"><span data-stu-id="ee969-239">Request</span></span>
<span data-ttu-id="ee969-240">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee969-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1962

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "hashAlgorithm": "sha2",
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

### <a name="response"></a><span data-ttu-id="ee969-241">応答</span><span class="sxs-lookup"><span data-stu-id="ee969-241">Response</span></span>
<span data-ttu-id="ee969-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee969-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2134

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "hashAlgorithm": "sha2",
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






