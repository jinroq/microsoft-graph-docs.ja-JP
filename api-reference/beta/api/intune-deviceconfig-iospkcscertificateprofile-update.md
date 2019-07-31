---
title: IosPkcsCertificateProfile の更新
description: IosPkcsCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89f549542e89d95303d09c8ace0c7848eb3c7e52
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948055"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="40cbc-103">IosPkcsCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="40cbc-103">Update iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="40cbc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40cbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40cbc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="40cbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40cbc-106">[Iospkcscertificateprofile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-106">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40cbc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="40cbc-107">Prerequisites</span></span>
<span data-ttu-id="40cbc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40cbc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40cbc-110">Permission type</span></span>|<span data-ttu-id="40cbc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40cbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40cbc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40cbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40cbc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40cbc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40cbc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40cbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40cbc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40cbc-115">Not supported.</span></span>|
|<span data-ttu-id="40cbc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40cbc-116">Application</span></span>|<span data-ttu-id="40cbc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40cbc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40cbc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40cbc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="40cbc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40cbc-119">Request headers</span></span>
|<span data-ttu-id="40cbc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40cbc-120">Header</span></span>|<span data-ttu-id="40cbc-121">値</span><span class="sxs-lookup"><span data-stu-id="40cbc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40cbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40cbc-122">Authorization</span></span>|<span data-ttu-id="40cbc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="40cbc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40cbc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="40cbc-124">Accept</span></span>|<span data-ttu-id="40cbc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40cbc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40cbc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="40cbc-126">Request body</span></span>
<span data-ttu-id="40cbc-127">要求本文で、 [Iospkcscertificateprofile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-127">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="40cbc-128">次の表に、 [Iospkcscertificateprofile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-128">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="40cbc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40cbc-129">Property</span></span>|<span data-ttu-id="40cbc-130">型</span><span class="sxs-lookup"><span data-stu-id="40cbc-130">Type</span></span>|<span data-ttu-id="40cbc-131">説明</span><span class="sxs-lookup"><span data-stu-id="40cbc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40cbc-132">id</span><span class="sxs-lookup"><span data-stu-id="40cbc-132">id</span></span>|<span data-ttu-id="40cbc-133">文字列</span><span class="sxs-lookup"><span data-stu-id="40cbc-133">String</span></span>|<span data-ttu-id="40cbc-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="40cbc-134">Key of the entity.</span></span> <span data-ttu-id="40cbc-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40cbc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="40cbc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40cbc-137">DateTimeOffset</span></span>|<span data-ttu-id="40cbc-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="40cbc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="40cbc-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="40cbc-140">roleScopeTagIds</span></span>|<span data-ttu-id="40cbc-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="40cbc-141">String collection</span></span>|<span data-ttu-id="40cbc-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="40cbc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="40cbc-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="40cbc-144">supportsScopeTags</span></span>|<span data-ttu-id="40cbc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="40cbc-145">Boolean</span></span>|<span data-ttu-id="40cbc-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="40cbc-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="40cbc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="40cbc-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="40cbc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="40cbc-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-149">This property is read-only.</span></span> <span data-ttu-id="40cbc-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="40cbc-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="40cbc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="40cbc-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="40cbc-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="40cbc-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="40cbc-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="40cbc-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="40cbc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="40cbc-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="40cbc-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="40cbc-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="40cbc-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="40cbc-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="40cbc-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="40cbc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="40cbc-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="40cbc-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="40cbc-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40cbc-163">createdDateTime</span></span>|<span data-ttu-id="40cbc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40cbc-164">DateTimeOffset</span></span>|<span data-ttu-id="40cbc-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="40cbc-165">DateTime the object was created.</span></span> <span data-ttu-id="40cbc-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-167">description</span><span class="sxs-lookup"><span data-stu-id="40cbc-167">description</span></span>|<span data-ttu-id="40cbc-168">String</span><span class="sxs-lookup"><span data-stu-id="40cbc-168">String</span></span>|<span data-ttu-id="40cbc-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="40cbc-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="40cbc-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-171">displayName</span><span class="sxs-lookup"><span data-stu-id="40cbc-171">displayName</span></span>|<span data-ttu-id="40cbc-172">String</span><span class="sxs-lookup"><span data-stu-id="40cbc-172">String</span></span>|<span data-ttu-id="40cbc-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="40cbc-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="40cbc-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-175">version</span><span class="sxs-lookup"><span data-stu-id="40cbc-175">version</span></span>|<span data-ttu-id="40cbc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="40cbc-176">Int32</span></span>|<span data-ttu-id="40cbc-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="40cbc-177">Version of the device configuration.</span></span> <span data-ttu-id="40cbc-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40cbc-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="40cbc-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="40cbc-180">Int32</span><span class="sxs-lookup"><span data-stu-id="40cbc-180">Int32</span></span>|<span data-ttu-id="40cbc-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="40cbc-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="40cbc-182">有効な値は、 [Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承された値 1 ~ 99 です。</span><span class="sxs-lookup"><span data-stu-id="40cbc-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="40cbc-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="40cbc-183">subjectNameFormat</span></span>|[<span data-ttu-id="40cbc-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="40cbc-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="40cbc-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="40cbc-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="40cbc-186">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="40cbc-187">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="40cbc-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="40cbc-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="40cbc-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="40cbc-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="40cbc-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="40cbc-190">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="40cbc-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="40cbc-191">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="40cbc-192">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="40cbc-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="40cbc-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="40cbc-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="40cbc-194">Int32</span><span class="sxs-lookup"><span data-stu-id="40cbc-194">Int32</span></span>|<span data-ttu-id="40cbc-195">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="40cbc-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="40cbc-196">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="40cbc-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="40cbc-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="40cbc-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="40cbc-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="40cbc-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="40cbc-199">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="40cbc-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="40cbc-200">[Ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="40cbc-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="40cbc-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="40cbc-202">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="40cbc-202">certificationAuthority</span></span>|<span data-ttu-id="40cbc-203">String</span><span class="sxs-lookup"><span data-stu-id="40cbc-203">String</span></span>|<span data-ttu-id="40cbc-204">PKCS 証明機関。</span><span class="sxs-lookup"><span data-stu-id="40cbc-204">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="40cbc-205">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="40cbc-205">certificationAuthorityName</span></span>|<span data-ttu-id="40cbc-206">String</span><span class="sxs-lookup"><span data-stu-id="40cbc-206">String</span></span>|<span data-ttu-id="40cbc-207">PKCS 証明機関名。</span><span class="sxs-lookup"><span data-stu-id="40cbc-207">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="40cbc-208">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="40cbc-208">certificateTemplateName</span></span>|<span data-ttu-id="40cbc-209">String</span><span class="sxs-lookup"><span data-stu-id="40cbc-209">String</span></span>|<span data-ttu-id="40cbc-210">PKCS 証明書テンプレート名。</span><span class="sxs-lookup"><span data-stu-id="40cbc-210">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="40cbc-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="40cbc-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="40cbc-212">String</span><span class="sxs-lookup"><span data-stu-id="40cbc-212">String</span></span>|<span data-ttu-id="40cbc-213">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="40cbc-213">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="40cbc-214">応答</span><span class="sxs-lookup"><span data-stu-id="40cbc-214">Response</span></span>
<span data-ttu-id="40cbc-215">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Iospkcscertificateprofile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40cbc-215">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40cbc-216">例</span><span class="sxs-lookup"><span data-stu-id="40cbc-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="40cbc-217">要求</span><span class="sxs-lookup"><span data-stu-id="40cbc-217">Request</span></span>
<span data-ttu-id="40cbc-218">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40cbc-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1534

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="40cbc-219">応答</span><span class="sxs-lookup"><span data-stu-id="40cbc-219">Response</span></span>
<span data-ttu-id="40cbc-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40cbc-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1706

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





