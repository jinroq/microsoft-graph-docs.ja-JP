---
title: AndroidForWorkPkcsCertificateProfile の更新
description: AndroidForWorkPkcsCertificateProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a46155be8bd5d8a0445b356e3dc2a956a60b528a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963277"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="d4a6f-103">AndroidForWorkPkcsCertificateProfile の更新</span><span class="sxs-lookup"><span data-stu-id="d4a6f-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="d4a6f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4a6f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4a6f-106">[AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-106">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4a6f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4a6f-107">Prerequisites</span></span>
<span data-ttu-id="d4a6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4a6f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4a6f-110">Permission type</span></span>|<span data-ttu-id="d4a6f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4a6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4a6f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4a6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4a6f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a6f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4a6f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4a6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4a6f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-115">Not supported.</span></span>|
|<span data-ttu-id="d4a6f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4a6f-116">Application</span></span>|<span data-ttu-id="d4a6f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4a6f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4a6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4a6f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4a6f-119">Request headers</span></span>
|<span data-ttu-id="d4a6f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4a6f-120">Header</span></span>|<span data-ttu-id="d4a6f-121">値</span><span class="sxs-lookup"><span data-stu-id="d4a6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4a6f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4a6f-122">Authorization</span></span>|<span data-ttu-id="d4a6f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4a6f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d4a6f-124">Accept</span></span>|<span data-ttu-id="d4a6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4a6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4a6f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4a6f-126">Request body</span></span>
<span data-ttu-id="d4a6f-127">要求本文で、 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-127">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="d4a6f-128">次の表に、 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-128">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="d4a6f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4a6f-129">Property</span></span>|<span data-ttu-id="d4a6f-130">型</span><span class="sxs-lookup"><span data-stu-id="d4a6f-130">Type</span></span>|<span data-ttu-id="d4a6f-131">説明</span><span class="sxs-lookup"><span data-stu-id="d4a6f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4a6f-132">id</span><span class="sxs-lookup"><span data-stu-id="d4a6f-132">id</span></span>|<span data-ttu-id="d4a6f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d4a6f-133">String</span></span>|<span data-ttu-id="d4a6f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-134">Key of the entity.</span></span> <span data-ttu-id="d4a6f-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4a6f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d4a6f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4a6f-137">DateTimeOffset</span></span>|<span data-ttu-id="d4a6f-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d4a6f-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4a6f-140">roleScopeTagIds</span></span>|<span data-ttu-id="d4a6f-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d4a6f-141">String collection</span></span>|<span data-ttu-id="d4a6f-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4a6f-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d4a6f-144">supportsScopeTags</span></span>|<span data-ttu-id="d4a6f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4a6f-145">Boolean</span></span>|<span data-ttu-id="d4a6f-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d4a6f-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d4a6f-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d4a6f-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-149">This property is read-only.</span></span> <span data-ttu-id="d4a6f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d4a6f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d4a6f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d4a6f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d4a6f-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d4a6f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d4a6f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d4a6f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d4a6f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d4a6f-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d4a6f-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d4a6f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d4a6f-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d4a6f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d4a6f-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d4a6f-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4a6f-163">createdDateTime</span></span>|<span data-ttu-id="d4a6f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4a6f-164">DateTimeOffset</span></span>|<span data-ttu-id="d4a6f-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-165">DateTime the object was created.</span></span> <span data-ttu-id="d4a6f-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-167">description</span><span class="sxs-lookup"><span data-stu-id="d4a6f-167">description</span></span>|<span data-ttu-id="d4a6f-168">String</span><span class="sxs-lookup"><span data-stu-id="d4a6f-168">String</span></span>|<span data-ttu-id="d4a6f-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4a6f-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d4a6f-171">displayName</span></span>|<span data-ttu-id="d4a6f-172">String</span><span class="sxs-lookup"><span data-stu-id="d4a6f-172">String</span></span>|<span data-ttu-id="d4a6f-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4a6f-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-175">version</span><span class="sxs-lookup"><span data-stu-id="d4a6f-175">version</span></span>|<span data-ttu-id="d4a6f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d4a6f-176">Int32</span></span>|<span data-ttu-id="d4a6f-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-177">Version of the device configuration.</span></span> <span data-ttu-id="d4a6f-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a6f-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d4a6f-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="d4a6f-180">Int32</span><span class="sxs-lookup"><span data-stu-id="d4a6f-180">Int32</span></span>|<span data-ttu-id="d4a6f-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d4a6f-182">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承された有効な値 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="d4a6f-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d4a6f-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d4a6f-183">subjectNameFormat</span></span>|[<span data-ttu-id="d4a6f-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d4a6f-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d4a6f-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="d4a6f-186">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d4a6f-187">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d4a6f-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d4a6f-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d4a6f-189">Int32</span><span class="sxs-lookup"><span data-stu-id="d4a6f-189">Int32</span></span>|<span data-ttu-id="d4a6f-190">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d4a6f-191">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d4a6f-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d4a6f-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d4a6f-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d4a6f-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d4a6f-194">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d4a6f-195">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d4a6f-196">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d4a6f-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d4a6f-197">extendedKeyUsages</span></span>|<span data-ttu-id="d4a6f-198">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d4a6f-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d4a6f-199">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d4a6f-200">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d4a6f-201">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d4a6f-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d4a6f-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d4a6f-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d4a6f-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d4a6f-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d4a6f-204">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d4a6f-205">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d4a6f-206">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d4a6f-207">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="d4a6f-207">certificationAuthority</span></span>|<span data-ttu-id="d4a6f-208">String</span><span class="sxs-lookup"><span data-stu-id="d4a6f-208">String</span></span>|<span data-ttu-id="d4a6f-209">PKCS 証明機関</span><span class="sxs-lookup"><span data-stu-id="d4a6f-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="d4a6f-210">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="d4a6f-210">certificationAuthorityName</span></span>|<span data-ttu-id="d4a6f-211">String</span><span class="sxs-lookup"><span data-stu-id="d4a6f-211">String</span></span>|<span data-ttu-id="d4a6f-212">PKCS 証明機関名</span><span class="sxs-lookup"><span data-stu-id="d4a6f-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="d4a6f-213">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="d4a6f-213">certificateTemplateName</span></span>|<span data-ttu-id="d4a6f-214">String</span><span class="sxs-lookup"><span data-stu-id="d4a6f-214">String</span></span>|<span data-ttu-id="d4a6f-215">PKCS 証明書テンプレート名</span><span class="sxs-lookup"><span data-stu-id="d4a6f-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="d4a6f-216">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d4a6f-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d4a6f-217">String</span><span class="sxs-lookup"><span data-stu-id="d4a6f-217">String</span></span>|<span data-ttu-id="d4a6f-218">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-218">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="d4a6f-219">応答</span><span class="sxs-lookup"><span data-stu-id="d4a6f-219">Response</span></span>
<span data-ttu-id="d4a6f-220">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-220">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4a6f-221">例</span><span class="sxs-lookup"><span data-stu-id="d4a6f-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4a6f-222">要求</span><span class="sxs-lookup"><span data-stu-id="d4a6f-222">Request</span></span>
<span data-ttu-id="d4a6f-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1738

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="d4a6f-224">応答</span><span class="sxs-lookup"><span data-stu-id="d4a6f-224">Response</span></span>
<span data-ttu-id="d4a6f-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4a6f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1910

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





