---
title: AndroidImportedPFXCertificateProfile を作成する
description: 新しい androidImportedPFXCertificateProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c88203d91fcc16570ea400db68df7cb366f5781
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970157"
---
# <a name="create-androidimportedpfxcertificateprofile"></a><span data-ttu-id="d6671-103">AndroidImportedPFXCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="d6671-103">Create androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="d6671-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6671-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6671-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6671-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6671-106">新しい[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d6671-106">Create a new [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6671-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d6671-107">Prerequisites</span></span>
<span data-ttu-id="d6671-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6671-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6671-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6671-110">Permission type</span></span>|<span data-ttu-id="d6671-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6671-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6671-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6671-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6671-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6671-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6671-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6671-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6671-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6671-115">Not supported.</span></span>|
|<span data-ttu-id="d6671-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6671-116">Application</span></span>|<span data-ttu-id="d6671-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6671-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6671-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6671-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6671-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6671-119">Request headers</span></span>
|<span data-ttu-id="d6671-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6671-120">Header</span></span>|<span data-ttu-id="d6671-121">値</span><span class="sxs-lookup"><span data-stu-id="d6671-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6671-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6671-122">Authorization</span></span>|<span data-ttu-id="d6671-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6671-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6671-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d6671-124">Accept</span></span>|<span data-ttu-id="d6671-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6671-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6671-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6671-126">Request body</span></span>
<span data-ttu-id="d6671-127">要求本文で、androidImportedPFXCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d6671-127">In the request body, supply a JSON representation for the androidImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="d6671-128">次の表に、androidImportedPFXCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d6671-128">The following table shows the properties that are required when you create the androidImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="d6671-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6671-129">Property</span></span>|<span data-ttu-id="d6671-130">型</span><span class="sxs-lookup"><span data-stu-id="d6671-130">Type</span></span>|<span data-ttu-id="d6671-131">説明</span><span class="sxs-lookup"><span data-stu-id="d6671-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6671-132">id</span><span class="sxs-lookup"><span data-stu-id="d6671-132">id</span></span>|<span data-ttu-id="d6671-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d6671-133">String</span></span>|<span data-ttu-id="d6671-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d6671-134">Key of the entity.</span></span> <span data-ttu-id="d6671-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6671-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d6671-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6671-137">DateTimeOffset</span></span>|<span data-ttu-id="d6671-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d6671-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d6671-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6671-140">roleScopeTagIds</span></span>|<span data-ttu-id="d6671-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d6671-141">String collection</span></span>|<span data-ttu-id="d6671-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="d6671-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d6671-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d6671-144">supportsScopeTags</span></span>|<span data-ttu-id="d6671-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6671-145">Boolean</span></span>|<span data-ttu-id="d6671-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d6671-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d6671-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="d6671-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d6671-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="d6671-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d6671-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d6671-149">This property is read-only.</span></span> <span data-ttu-id="d6671-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d6671-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d6671-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d6671-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d6671-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="d6671-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d6671-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d6671-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d6671-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d6671-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d6671-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d6671-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d6671-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d6671-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d6671-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d6671-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d6671-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d6671-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d6671-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6671-163">createdDateTime</span></span>|<span data-ttu-id="d6671-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6671-164">DateTimeOffset</span></span>|<span data-ttu-id="d6671-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d6671-165">DateTime the object was created.</span></span> <span data-ttu-id="d6671-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-167">description</span><span class="sxs-lookup"><span data-stu-id="d6671-167">description</span></span>|<span data-ttu-id="d6671-168">String</span><span class="sxs-lookup"><span data-stu-id="d6671-168">String</span></span>|<span data-ttu-id="d6671-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="d6671-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6671-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d6671-171">displayName</span></span>|<span data-ttu-id="d6671-172">String</span><span class="sxs-lookup"><span data-stu-id="d6671-172">String</span></span>|<span data-ttu-id="d6671-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d6671-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6671-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-175">version</span><span class="sxs-lookup"><span data-stu-id="d6671-175">version</span></span>|<span data-ttu-id="d6671-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d6671-176">Int32</span></span>|<span data-ttu-id="d6671-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d6671-177">Version of the device configuration.</span></span> <span data-ttu-id="d6671-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6671-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d6671-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="d6671-180">Int32</span><span class="sxs-lookup"><span data-stu-id="d6671-180">Int32</span></span>|<span data-ttu-id="d6671-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="d6671-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d6671-182">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="d6671-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d6671-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d6671-183">subjectNameFormat</span></span>|[<span data-ttu-id="d6671-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d6671-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d6671-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="d6671-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="d6671-186">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d6671-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d6671-187">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="d6671-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d6671-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d6671-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d6671-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d6671-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d6671-190">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="d6671-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d6671-191">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d6671-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d6671-192">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="d6671-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d6671-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d6671-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d6671-194">Int32</span><span class="sxs-lookup"><span data-stu-id="d6671-194">Int32</span></span>|<span data-ttu-id="d6671-195">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="d6671-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d6671-196">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d6671-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d6671-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d6671-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d6671-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d6671-199">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="d6671-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d6671-200">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d6671-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d6671-201">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="d6671-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d6671-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d6671-202">extendedKeyUsages</span></span>|<span data-ttu-id="d6671-203">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d6671-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d6671-204">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="d6671-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d6671-205">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d6671-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d6671-206">[Androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d6671-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d6671-207">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d6671-207">intendedPurpose</span></span>|[<span data-ttu-id="d6671-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d6671-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d6671-209">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="d6671-209">Not yet documented.</span></span> <span data-ttu-id="d6671-210">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="d6671-210">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d6671-211">応答</span><span class="sxs-lookup"><span data-stu-id="d6671-211">Response</span></span>
<span data-ttu-id="d6671-212">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d6671-212">If successful, this method returns a `201 Created` response code and a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6671-213">例</span><span class="sxs-lookup"><span data-stu-id="d6671-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6671-214">要求</span><span class="sxs-lookup"><span data-stu-id="d6671-214">Request</span></span>
<span data-ttu-id="d6671-215">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6671-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1492

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="d6671-216">応答</span><span class="sxs-lookup"><span data-stu-id="d6671-216">Response</span></span>
<span data-ttu-id="d6671-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6671-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1664

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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





