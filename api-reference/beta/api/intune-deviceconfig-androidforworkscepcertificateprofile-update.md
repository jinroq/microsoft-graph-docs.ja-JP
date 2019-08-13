---
title: AndroidForWorkScepCertificateProfile の更新
description: AndroidForWorkScepCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d2c021c7aec4de899f01334836c5bb7d27d3771
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341333"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="86917-103">AndroidForWorkScepCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="86917-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="86917-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86917-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86917-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86917-106">[AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="86917-106">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86917-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="86917-107">Prerequisites</span></span>
<span data-ttu-id="86917-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86917-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86917-110">Permission type</span></span>|<span data-ttu-id="86917-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="86917-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86917-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86917-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86917-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86917-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86917-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86917-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86917-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86917-115">Not supported.</span></span>|
|<span data-ttu-id="86917-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86917-116">Application</span></span>|<span data-ttu-id="86917-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86917-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86917-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86917-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="86917-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86917-119">Request headers</span></span>
|<span data-ttu-id="86917-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86917-120">Header</span></span>|<span data-ttu-id="86917-121">値</span><span class="sxs-lookup"><span data-stu-id="86917-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86917-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86917-122">Authorization</span></span>|<span data-ttu-id="86917-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="86917-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86917-124">承諾</span><span class="sxs-lookup"><span data-stu-id="86917-124">Accept</span></span>|<span data-ttu-id="86917-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86917-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86917-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="86917-126">Request body</span></span>
<span data-ttu-id="86917-127">要求本文で、 [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="86917-127">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="86917-128">次の表に、 [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="86917-128">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="86917-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86917-129">Property</span></span>|<span data-ttu-id="86917-130">型</span><span class="sxs-lookup"><span data-stu-id="86917-130">Type</span></span>|<span data-ttu-id="86917-131">説明</span><span class="sxs-lookup"><span data-stu-id="86917-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86917-132">id</span><span class="sxs-lookup"><span data-stu-id="86917-132">id</span></span>|<span data-ttu-id="86917-133">文字列</span><span class="sxs-lookup"><span data-stu-id="86917-133">String</span></span>|<span data-ttu-id="86917-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="86917-134">Key of the entity.</span></span> <span data-ttu-id="86917-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86917-136">lastModifiedDateTime</span></span>|<span data-ttu-id="86917-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86917-137">DateTimeOffset</span></span>|<span data-ttu-id="86917-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="86917-138">DateTime the object was last modified.</span></span> <span data-ttu-id="86917-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86917-140">roleScopeTagIds</span></span>|<span data-ttu-id="86917-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="86917-141">String collection</span></span>|<span data-ttu-id="86917-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="86917-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86917-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86917-144">supportsScopeTags</span></span>|<span data-ttu-id="86917-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="86917-145">Boolean</span></span>|<span data-ttu-id="86917-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86917-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86917-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="86917-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86917-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="86917-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86917-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="86917-149">This property is read-only.</span></span> <span data-ttu-id="86917-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86917-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="86917-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86917-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="86917-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="86917-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="86917-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86917-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="86917-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86917-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="86917-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="86917-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="86917-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="86917-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="86917-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="86917-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="86917-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="86917-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="86917-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86917-163">createdDateTime</span></span>|<span data-ttu-id="86917-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86917-164">DateTimeOffset</span></span>|<span data-ttu-id="86917-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="86917-165">DateTime the object was created.</span></span> <span data-ttu-id="86917-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-167">description</span><span class="sxs-lookup"><span data-stu-id="86917-167">description</span></span>|<span data-ttu-id="86917-168">String</span><span class="sxs-lookup"><span data-stu-id="86917-168">String</span></span>|<span data-ttu-id="86917-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="86917-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86917-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-171">displayName</span><span class="sxs-lookup"><span data-stu-id="86917-171">displayName</span></span>|<span data-ttu-id="86917-172">String</span><span class="sxs-lookup"><span data-stu-id="86917-172">String</span></span>|<span data-ttu-id="86917-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="86917-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86917-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-175">version</span><span class="sxs-lookup"><span data-stu-id="86917-175">version</span></span>|<span data-ttu-id="86917-176">Int32</span><span class="sxs-lookup"><span data-stu-id="86917-176">Int32</span></span>|<span data-ttu-id="86917-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="86917-177">Version of the device configuration.</span></span> <span data-ttu-id="86917-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86917-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="86917-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="86917-180">Int32</span><span class="sxs-lookup"><span data-stu-id="86917-180">Int32</span></span>|<span data-ttu-id="86917-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="86917-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="86917-182">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承された有効な値 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="86917-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86917-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="86917-183">subjectNameFormat</span></span>|[<span data-ttu-id="86917-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="86917-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="86917-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="86917-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="86917-186">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="86917-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="86917-187">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="86917-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="86917-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="86917-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="86917-189">Int32</span><span class="sxs-lookup"><span data-stu-id="86917-189">Int32</span></span>|<span data-ttu-id="86917-190">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="86917-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="86917-191">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86917-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="86917-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="86917-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="86917-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="86917-194">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="86917-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="86917-195">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="86917-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="86917-196">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="86917-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="86917-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="86917-197">extendedKeyUsages</span></span>|<span data-ttu-id="86917-198">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="86917-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="86917-199">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="86917-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="86917-200">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="86917-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="86917-201">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="86917-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86917-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="86917-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="86917-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="86917-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="86917-204">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="86917-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="86917-205">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="86917-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="86917-206">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="86917-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="86917-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="86917-207">scepServerUrls</span></span>|<span data-ttu-id="86917-208">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="86917-208">String collection</span></span>|<span data-ttu-id="86917-209">SCEP サーバーの Url</span><span class="sxs-lookup"><span data-stu-id="86917-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="86917-210">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="86917-210">subjectNameFormatString</span></span>|<span data-ttu-id="86917-211">String</span><span class="sxs-lookup"><span data-stu-id="86917-211">String</span></span>|<span data-ttu-id="86917-212">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="86917-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="86917-213">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="86917-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="86917-214">keyUsage</span><span class="sxs-lookup"><span data-stu-id="86917-214">keyUsage</span></span>|[<span data-ttu-id="86917-215">keyUsages</span><span class="sxs-lookup"><span data-stu-id="86917-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="86917-216">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="86917-216">SCEP Key Usage.</span></span> <span data-ttu-id="86917-217">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="86917-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="86917-218">keySize</span><span class="sxs-lookup"><span data-stu-id="86917-218">keySize</span></span>|[<span data-ttu-id="86917-219">keySize</span><span class="sxs-lookup"><span data-stu-id="86917-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="86917-220">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="86917-220">SCEP Key Size.</span></span> <span data-ttu-id="86917-221">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="86917-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="86917-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="86917-222">hashAlgorithm</span></span>|[<span data-ttu-id="86917-223">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="86917-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="86917-224">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="86917-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="86917-225">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="86917-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="86917-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="86917-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="86917-227">String</span><span class="sxs-lookup"><span data-stu-id="86917-227">String</span></span>|<span data-ttu-id="86917-228">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="86917-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="86917-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="86917-229">certificateStore</span></span>|[<span data-ttu-id="86917-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="86917-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="86917-231">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="86917-231">Target store certificate.</span></span> <span data-ttu-id="86917-232">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="86917-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="86917-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="86917-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="86917-234">[Customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="86917-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="86917-235">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="86917-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="86917-236">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="86917-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="86917-237">応答</span><span class="sxs-lookup"><span data-stu-id="86917-237">Response</span></span>
<span data-ttu-id="86917-238">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="86917-238">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86917-239">例</span><span class="sxs-lookup"><span data-stu-id="86917-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="86917-240">要求</span><span class="sxs-lookup"><span data-stu-id="86917-240">Request</span></span>
<span data-ttu-id="86917-241">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86917-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1978

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
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
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
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

### <a name="response"></a><span data-ttu-id="86917-242">応答</span><span class="sxs-lookup"><span data-stu-id="86917-242">Response</span></span>
<span data-ttu-id="86917-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86917-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2150

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
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






