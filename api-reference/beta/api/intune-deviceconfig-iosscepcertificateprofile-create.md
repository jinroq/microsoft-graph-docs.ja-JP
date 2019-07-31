---
title: IosScepCertificateProfile の作成
description: 新しい iosScepCertificateProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7eb3da55ca6806772b1dec7c1abc326d8456715d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948027"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="f102a-103">IosScepCertificateProfile の作成</span><span class="sxs-lookup"><span data-stu-id="f102a-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="f102a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f102a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f102a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f102a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f102a-106">新しい[Iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f102a-106">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f102a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f102a-107">Prerequisites</span></span>
<span data-ttu-id="f102a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f102a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f102a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f102a-110">Permission type</span></span>|<span data-ttu-id="f102a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f102a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f102a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f102a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f102a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f102a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f102a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f102a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f102a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f102a-115">Not supported.</span></span>|
|<span data-ttu-id="f102a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f102a-116">Application</span></span>|<span data-ttu-id="f102a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f102a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f102a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f102a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f102a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f102a-119">Request headers</span></span>
|<span data-ttu-id="f102a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f102a-120">Header</span></span>|<span data-ttu-id="f102a-121">値</span><span class="sxs-lookup"><span data-stu-id="f102a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f102a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f102a-122">Authorization</span></span>|<span data-ttu-id="f102a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f102a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f102a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f102a-124">Accept</span></span>|<span data-ttu-id="f102a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f102a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f102a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f102a-126">Request body</span></span>
<span data-ttu-id="f102a-127">要求本文で、iosScepCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f102a-127">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="f102a-128">次の表に、iosScepCertificateProfile プロファイルの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f102a-128">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="f102a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f102a-129">Property</span></span>|<span data-ttu-id="f102a-130">型</span><span class="sxs-lookup"><span data-stu-id="f102a-130">Type</span></span>|<span data-ttu-id="f102a-131">説明</span><span class="sxs-lookup"><span data-stu-id="f102a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f102a-132">id</span><span class="sxs-lookup"><span data-stu-id="f102a-132">id</span></span>|<span data-ttu-id="f102a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f102a-133">String</span></span>|<span data-ttu-id="f102a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f102a-134">Key of the entity.</span></span> <span data-ttu-id="f102a-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f102a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f102a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f102a-137">DateTimeOffset</span></span>|<span data-ttu-id="f102a-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f102a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f102a-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f102a-140">roleScopeTagIds</span></span>|<span data-ttu-id="f102a-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f102a-141">String collection</span></span>|<span data-ttu-id="f102a-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f102a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f102a-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f102a-144">supportsScopeTags</span></span>|<span data-ttu-id="f102a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f102a-145">Boolean</span></span>|<span data-ttu-id="f102a-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f102a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f102a-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f102a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f102a-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f102a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f102a-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f102a-149">This property is read-only.</span></span> <span data-ttu-id="f102a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f102a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f102a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f102a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f102a-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="f102a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f102a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f102a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f102a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f102a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f102a-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f102a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f102a-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f102a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f102a-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f102a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f102a-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f102a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f102a-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f102a-163">createdDateTime</span></span>|<span data-ttu-id="f102a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f102a-164">DateTimeOffset</span></span>|<span data-ttu-id="f102a-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f102a-165">DateTime the object was created.</span></span> <span data-ttu-id="f102a-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-167">description</span><span class="sxs-lookup"><span data-stu-id="f102a-167">description</span></span>|<span data-ttu-id="f102a-168">String</span><span class="sxs-lookup"><span data-stu-id="f102a-168">String</span></span>|<span data-ttu-id="f102a-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f102a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f102a-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f102a-171">displayName</span></span>|<span data-ttu-id="f102a-172">String</span><span class="sxs-lookup"><span data-stu-id="f102a-172">String</span></span>|<span data-ttu-id="f102a-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f102a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f102a-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-175">version</span><span class="sxs-lookup"><span data-stu-id="f102a-175">version</span></span>|<span data-ttu-id="f102a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f102a-176">Int32</span></span>|<span data-ttu-id="f102a-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f102a-177">Version of the device configuration.</span></span> <span data-ttu-id="f102a-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f102a-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f102a-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="f102a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="f102a-180">Int32</span></span>|<span data-ttu-id="f102a-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="f102a-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f102a-182">有効な値は、 [Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承された値 1 ~ 99 です。</span><span class="sxs-lookup"><span data-stu-id="f102a-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f102a-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f102a-183">subjectNameFormat</span></span>|[<span data-ttu-id="f102a-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f102a-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="f102a-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="f102a-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="f102a-186">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f102a-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f102a-187">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="f102a-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="f102a-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f102a-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f102a-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f102a-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f102a-190">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="f102a-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="f102a-191">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f102a-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f102a-192">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="f102a-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f102a-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f102a-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f102a-194">Int32</span><span class="sxs-lookup"><span data-stu-id="f102a-194">Int32</span></span>|<span data-ttu-id="f102a-195">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="f102a-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f102a-196">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f102a-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f102a-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f102a-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f102a-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f102a-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f102a-199">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="f102a-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f102a-200">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f102a-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="f102a-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="f102a-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f102a-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f102a-202">scepServerUrls</span></span>|<span data-ttu-id="f102a-203">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f102a-203">String collection</span></span>|<span data-ttu-id="f102a-204">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="f102a-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f102a-205">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="f102a-205">subjectNameFormatString</span></span>|<span data-ttu-id="f102a-206">String</span><span class="sxs-lookup"><span data-stu-id="f102a-206">String</span></span>|<span data-ttu-id="f102a-207">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="f102a-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f102a-208">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="f102a-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f102a-209">keyUsage</span><span class="sxs-lookup"><span data-stu-id="f102a-209">keyUsage</span></span>|[<span data-ttu-id="f102a-210">keyUsages</span><span class="sxs-lookup"><span data-stu-id="f102a-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f102a-211">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="f102a-211">SCEP Key Usage.</span></span> <span data-ttu-id="f102a-212">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="f102a-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f102a-213">keySize</span><span class="sxs-lookup"><span data-stu-id="f102a-213">keySize</span></span>|[<span data-ttu-id="f102a-214">keySize</span><span class="sxs-lookup"><span data-stu-id="f102a-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f102a-215">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="f102a-215">SCEP Key Size.</span></span> <span data-ttu-id="f102a-216">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="f102a-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f102a-217">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f102a-217">extendedKeyUsages</span></span>|<span data-ttu-id="f102a-218">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f102a-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f102a-219">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="f102a-219">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f102a-220">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f102a-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f102a-221">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f102a-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f102a-222">String</span><span class="sxs-lookup"><span data-stu-id="f102a-222">String</span></span>|<span data-ttu-id="f102a-223">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="f102a-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f102a-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f102a-224">certificateStore</span></span>|[<span data-ttu-id="f102a-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f102a-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f102a-226">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="f102a-226">Target store certificate.</span></span> <span data-ttu-id="f102a-227">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="f102a-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f102a-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f102a-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f102a-229">[Customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="f102a-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f102a-230">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="f102a-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f102a-231">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f102a-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f102a-232">応答</span><span class="sxs-lookup"><span data-stu-id="f102a-232">Response</span></span>
<span data-ttu-id="f102a-233">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f102a-233">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f102a-234">例</span><span class="sxs-lookup"><span data-stu-id="f102a-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="f102a-235">要求</span><span class="sxs-lookup"><span data-stu-id="f102a-235">Request</span></span>
<span data-ttu-id="f102a-236">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f102a-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f102a-237">応答</span><span class="sxs-lookup"><span data-stu-id="f102a-237">Response</span></span>
<span data-ttu-id="f102a-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f102a-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





