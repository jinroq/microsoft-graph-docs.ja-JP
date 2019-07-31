---
title: AndroidScepCertificateProfile の更新
description: AndroidScepCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a8e26d8c3b255369f1597e8c59b0f3bd8a2ebb3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962632"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="a5c3e-103">AndroidScepCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="a5c3e-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="a5c3e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5c3e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5c3e-106">[AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-106">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5c3e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a5c3e-107">Prerequisites</span></span>
<span data-ttu-id="a5c3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5c3e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5c3e-110">Permission type</span></span>|<span data-ttu-id="a5c3e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5c3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5c3e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5c3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5c3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5c3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5c3e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5c3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5c3e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-115">Not supported.</span></span>|
|<span data-ttu-id="a5c3e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5c3e-116">Application</span></span>|<span data-ttu-id="a5c3e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5c3e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5c3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a5c3e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5c3e-119">Request headers</span></span>
|<span data-ttu-id="a5c3e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5c3e-120">Header</span></span>|<span data-ttu-id="a5c3e-121">値</span><span class="sxs-lookup"><span data-stu-id="a5c3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5c3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5c3e-122">Authorization</span></span>|<span data-ttu-id="a5c3e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5c3e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a5c3e-124">Accept</span></span>|<span data-ttu-id="a5c3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5c3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5c3e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5c3e-126">Request body</span></span>
<span data-ttu-id="a5c3e-127">要求本文で、 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-127">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="a5c3e-128">次の表に、 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-128">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="a5c3e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5c3e-129">Property</span></span>|<span data-ttu-id="a5c3e-130">型</span><span class="sxs-lookup"><span data-stu-id="a5c3e-130">Type</span></span>|<span data-ttu-id="a5c3e-131">説明</span><span class="sxs-lookup"><span data-stu-id="a5c3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c3e-132">id</span><span class="sxs-lookup"><span data-stu-id="a5c3e-132">id</span></span>|<span data-ttu-id="a5c3e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a5c3e-133">String</span></span>|<span data-ttu-id="a5c3e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-134">Key of the entity.</span></span> <span data-ttu-id="a5c3e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c3e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a5c3e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c3e-137">DateTimeOffset</span></span>|<span data-ttu-id="a5c3e-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a5c3e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a5c3e-140">roleScopeTagIds</span></span>|<span data-ttu-id="a5c3e-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a5c3e-141">String collection</span></span>|<span data-ttu-id="a5c3e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a5c3e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a5c3e-144">supportsScopeTags</span></span>|<span data-ttu-id="a5c3e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c3e-145">Boolean</span></span>|<span data-ttu-id="a5c3e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a5c3e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a5c3e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a5c3e-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-149">This property is read-only.</span></span> <span data-ttu-id="a5c3e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a5c3e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a5c3e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a5c3e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a5c3e-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a5c3e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a5c3e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a5c3e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a5c3e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a5c3e-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a5c3e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="a5c3e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a5c3e-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="a5c3e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a5c3e-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a5c3e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c3e-163">createdDateTime</span></span>|<span data-ttu-id="a5c3e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c3e-164">DateTimeOffset</span></span>|<span data-ttu-id="a5c3e-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-165">DateTime the object was created.</span></span> <span data-ttu-id="a5c3e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-167">description</span><span class="sxs-lookup"><span data-stu-id="a5c3e-167">description</span></span>|<span data-ttu-id="a5c3e-168">String</span><span class="sxs-lookup"><span data-stu-id="a5c3e-168">String</span></span>|<span data-ttu-id="a5c3e-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a5c3e-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a5c3e-171">displayName</span></span>|<span data-ttu-id="a5c3e-172">String</span><span class="sxs-lookup"><span data-stu-id="a5c3e-172">String</span></span>|<span data-ttu-id="a5c3e-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a5c3e-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-175">version</span><span class="sxs-lookup"><span data-stu-id="a5c3e-175">version</span></span>|<span data-ttu-id="a5c3e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c3e-176">Int32</span></span>|<span data-ttu-id="a5c3e-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-177">Version of the device configuration.</span></span> <span data-ttu-id="a5c3e-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c3e-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a5c3e-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="a5c3e-180">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c3e-180">Int32</span></span>|<span data-ttu-id="a5c3e-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a5c3e-182">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a5c3e-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a5c3e-183">subjectNameFormat</span></span>|[<span data-ttu-id="a5c3e-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a5c3e-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a5c3e-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="a5c3e-186">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a5c3e-187">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a5c3e-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a5c3e-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a5c3e-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a5c3e-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a5c3e-190">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a5c3e-191">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a5c3e-192">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a5c3e-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a5c3e-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a5c3e-194">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c3e-194">Int32</span></span>|<span data-ttu-id="a5c3e-195">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a5c3e-196">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a5c3e-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a5c3e-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a5c3e-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a5c3e-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a5c3e-199">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a5c3e-200">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a5c3e-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a5c3e-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a5c3e-202">extendedKeyUsages</span></span>|<span data-ttu-id="a5c3e-203">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a5c3e-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a5c3e-204">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a5c3e-205">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a5c3e-206">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="a5c3e-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a5c3e-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="a5c3e-207">scepServerUrls</span></span>|<span data-ttu-id="a5c3e-208">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a5c3e-208">String collection</span></span>|<span data-ttu-id="a5c3e-209">SCEP サーバーの Url</span><span class="sxs-lookup"><span data-stu-id="a5c3e-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="a5c3e-210">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5c3e-210">subjectNameFormatString</span></span>|<span data-ttu-id="a5c3e-211">String</span><span class="sxs-lookup"><span data-stu-id="a5c3e-211">String</span></span>|<span data-ttu-id="a5c3e-212">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a5c3e-213">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="a5c3e-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a5c3e-214">keyUsage</span><span class="sxs-lookup"><span data-stu-id="a5c3e-214">keyUsage</span></span>|[<span data-ttu-id="a5c3e-215">keyUsages</span><span class="sxs-lookup"><span data-stu-id="a5c3e-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a5c3e-216">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-216">SCEP Key Usage.</span></span> <span data-ttu-id="a5c3e-217">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a5c3e-218">keySize</span><span class="sxs-lookup"><span data-stu-id="a5c3e-218">keySize</span></span>|[<span data-ttu-id="a5c3e-219">keySize</span><span class="sxs-lookup"><span data-stu-id="a5c3e-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="a5c3e-220">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-220">SCEP Key Size.</span></span> <span data-ttu-id="a5c3e-221">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="a5c3e-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a5c3e-222">hashAlgorithm</span></span>|[<span data-ttu-id="a5c3e-223">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="a5c3e-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="a5c3e-224">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="a5c3e-225">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="a5c3e-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a5c3e-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a5c3e-227">String</span><span class="sxs-lookup"><span data-stu-id="a5c3e-227">String</span></span>|<span data-ttu-id="a5c3e-228">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-228">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="a5c3e-229">応答</span><span class="sxs-lookup"><span data-stu-id="a5c3e-229">Response</span></span>
<span data-ttu-id="a5c3e-230">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-230">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5c3e-231">例</span><span class="sxs-lookup"><span data-stu-id="a5c3e-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5c3e-232">要求</span><span class="sxs-lookup"><span data-stu-id="a5c3e-232">Request</span></span>
<span data-ttu-id="a5c3e-233">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1747

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="a5c3e-234">応答</span><span class="sxs-lookup"><span data-stu-id="a5c3e-234">Response</span></span>
<span data-ttu-id="a5c3e-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5c3e-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1919

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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





