---
title: AndroidForWorkImportedPFXCertificateProfile を作成する
description: 新しい androidForWorkImportedPFXCertificateProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cccdd97350f71f1883ce9aeaa45bf04e62ceef2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341438"
---
# <a name="create-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="f334e-103">AndroidForWorkImportedPFXCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="f334e-103">Create androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="f334e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f334e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f334e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f334e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f334e-106">新しい[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f334e-106">Create a new [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f334e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f334e-107">Prerequisites</span></span>
<span data-ttu-id="f334e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f334e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f334e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f334e-110">Permission type</span></span>|<span data-ttu-id="f334e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f334e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f334e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f334e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f334e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f334e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f334e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f334e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f334e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f334e-115">Not supported.</span></span>|
|<span data-ttu-id="f334e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f334e-116">Application</span></span>|<span data-ttu-id="f334e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f334e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f334e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f334e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f334e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f334e-119">Request headers</span></span>
|<span data-ttu-id="f334e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f334e-120">Header</span></span>|<span data-ttu-id="f334e-121">値</span><span class="sxs-lookup"><span data-stu-id="f334e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f334e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f334e-122">Authorization</span></span>|<span data-ttu-id="f334e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f334e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f334e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f334e-124">Accept</span></span>|<span data-ttu-id="f334e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f334e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f334e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f334e-126">Request body</span></span>
<span data-ttu-id="f334e-127">要求本文で、androidForWorkImportedPFXCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f334e-127">In the request body, supply a JSON representation for the androidForWorkImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="f334e-128">次の表に、androidForWorkImportedPFXCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f334e-128">The following table shows the properties that are required when you create the androidForWorkImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="f334e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f334e-129">Property</span></span>|<span data-ttu-id="f334e-130">型</span><span class="sxs-lookup"><span data-stu-id="f334e-130">Type</span></span>|<span data-ttu-id="f334e-131">説明</span><span class="sxs-lookup"><span data-stu-id="f334e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f334e-132">id</span><span class="sxs-lookup"><span data-stu-id="f334e-132">id</span></span>|<span data-ttu-id="f334e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f334e-133">String</span></span>|<span data-ttu-id="f334e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f334e-134">Key of the entity.</span></span> <span data-ttu-id="f334e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f334e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f334e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f334e-137">DateTimeOffset</span></span>|<span data-ttu-id="f334e-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f334e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f334e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f334e-140">roleScopeTagIds</span></span>|<span data-ttu-id="f334e-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f334e-141">String collection</span></span>|<span data-ttu-id="f334e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f334e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f334e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f334e-144">supportsScopeTags</span></span>|<span data-ttu-id="f334e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f334e-145">Boolean</span></span>|<span data-ttu-id="f334e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f334e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f334e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f334e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f334e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f334e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f334e-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f334e-149">This property is read-only.</span></span> <span data-ttu-id="f334e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f334e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f334e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f334e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f334e-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="f334e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f334e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f334e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f334e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f334e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f334e-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f334e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f334e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f334e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f334e-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f334e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f334e-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f334e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f334e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f334e-163">createdDateTime</span></span>|<span data-ttu-id="f334e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f334e-164">DateTimeOffset</span></span>|<span data-ttu-id="f334e-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f334e-165">DateTime the object was created.</span></span> <span data-ttu-id="f334e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-167">description</span><span class="sxs-lookup"><span data-stu-id="f334e-167">description</span></span>|<span data-ttu-id="f334e-168">String</span><span class="sxs-lookup"><span data-stu-id="f334e-168">String</span></span>|<span data-ttu-id="f334e-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f334e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f334e-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f334e-171">displayName</span></span>|<span data-ttu-id="f334e-172">String</span><span class="sxs-lookup"><span data-stu-id="f334e-172">String</span></span>|<span data-ttu-id="f334e-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f334e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f334e-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-175">version</span><span class="sxs-lookup"><span data-stu-id="f334e-175">version</span></span>|<span data-ttu-id="f334e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f334e-176">Int32</span></span>|<span data-ttu-id="f334e-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f334e-177">Version of the device configuration.</span></span> <span data-ttu-id="f334e-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f334e-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f334e-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="f334e-180">Int32</span><span class="sxs-lookup"><span data-stu-id="f334e-180">Int32</span></span>|<span data-ttu-id="f334e-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="f334e-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f334e-182">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="f334e-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f334e-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f334e-183">subjectNameFormat</span></span>|[<span data-ttu-id="f334e-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f334e-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f334e-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="f334e-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="f334e-186">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f334e-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f334e-187">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="f334e-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f334e-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f334e-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f334e-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f334e-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f334e-190">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="f334e-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f334e-191">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f334e-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f334e-192">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="f334e-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f334e-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f334e-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f334e-194">Int32</span><span class="sxs-lookup"><span data-stu-id="f334e-194">Int32</span></span>|<span data-ttu-id="f334e-195">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="f334e-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f334e-196">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f334e-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f334e-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f334e-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f334e-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f334e-199">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="f334e-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f334e-200">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f334e-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f334e-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="f334e-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f334e-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f334e-202">extendedKeyUsages</span></span>|<span data-ttu-id="f334e-203">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f334e-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f334e-204">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="f334e-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f334e-205">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f334e-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f334e-206">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f334e-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f334e-207">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="f334e-207">intendedPurpose</span></span>|[<span data-ttu-id="f334e-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="f334e-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="f334e-209">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="f334e-209">Not yet documented.</span></span> <span data-ttu-id="f334e-210">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="f334e-210">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="f334e-211">応答</span><span class="sxs-lookup"><span data-stu-id="f334e-211">Response</span></span>
<span data-ttu-id="f334e-212">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f334e-212">If successful, this method returns a `201 Created` response code and a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f334e-213">例</span><span class="sxs-lookup"><span data-stu-id="f334e-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="f334e-214">要求</span><span class="sxs-lookup"><span data-stu-id="f334e-214">Request</span></span>
<span data-ttu-id="f334e-215">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f334e-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1499

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="f334e-216">応答</span><span class="sxs-lookup"><span data-stu-id="f334e-216">Response</span></span>
<span data-ttu-id="f334e-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f334e-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1671

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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
  "intendedPurpose": "smimeEncryption"
}
```






