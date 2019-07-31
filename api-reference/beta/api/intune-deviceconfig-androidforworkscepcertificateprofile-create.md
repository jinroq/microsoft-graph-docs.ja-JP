---
title: AndroidForWorkScepCertificateProfile を作成する
description: 新しい androidForWorkScepCertificateProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c8e2a1f680441510bf8c921617fcafbe18e19c2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963263"
---
# <a name="create-androidforworkscepcertificateprofile"></a><span data-ttu-id="6647b-103">AndroidForWorkScepCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="6647b-103">Create androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="6647b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6647b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6647b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6647b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6647b-106">新しい[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6647b-106">Create a new [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6647b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6647b-107">Prerequisites</span></span>
<span data-ttu-id="6647b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6647b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6647b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6647b-110">Permission type</span></span>|<span data-ttu-id="6647b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6647b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6647b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6647b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6647b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6647b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6647b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6647b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6647b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6647b-115">Not supported.</span></span>|
|<span data-ttu-id="6647b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6647b-116">Application</span></span>|<span data-ttu-id="6647b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6647b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6647b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6647b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6647b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6647b-119">Request headers</span></span>
|<span data-ttu-id="6647b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6647b-120">Header</span></span>|<span data-ttu-id="6647b-121">値</span><span class="sxs-lookup"><span data-stu-id="6647b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6647b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6647b-122">Authorization</span></span>|<span data-ttu-id="6647b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6647b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6647b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6647b-124">Accept</span></span>|<span data-ttu-id="6647b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6647b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6647b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6647b-126">Request body</span></span>
<span data-ttu-id="6647b-127">要求本文で、androidForWorkScepCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6647b-127">In the request body, supply a JSON representation for the androidForWorkScepCertificateProfile object.</span></span>

<span data-ttu-id="6647b-128">次の表に、androidForWorkScepCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6647b-128">The following table shows the properties that are required when you create the androidForWorkScepCertificateProfile.</span></span>

|<span data-ttu-id="6647b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6647b-129">Property</span></span>|<span data-ttu-id="6647b-130">型</span><span class="sxs-lookup"><span data-stu-id="6647b-130">Type</span></span>|<span data-ttu-id="6647b-131">説明</span><span class="sxs-lookup"><span data-stu-id="6647b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6647b-132">id</span><span class="sxs-lookup"><span data-stu-id="6647b-132">id</span></span>|<span data-ttu-id="6647b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6647b-133">String</span></span>|<span data-ttu-id="6647b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6647b-134">Key of the entity.</span></span> <span data-ttu-id="6647b-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6647b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6647b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6647b-137">DateTimeOffset</span></span>|<span data-ttu-id="6647b-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="6647b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6647b-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6647b-140">roleScopeTagIds</span></span>|<span data-ttu-id="6647b-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6647b-141">String collection</span></span>|<span data-ttu-id="6647b-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="6647b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6647b-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6647b-144">supportsScopeTags</span></span>|<span data-ttu-id="6647b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6647b-145">Boolean</span></span>|<span data-ttu-id="6647b-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6647b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6647b-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="6647b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6647b-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="6647b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6647b-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="6647b-149">This property is read-only.</span></span> <span data-ttu-id="6647b-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6647b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6647b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6647b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6647b-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="6647b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6647b-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6647b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6647b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6647b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6647b-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="6647b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6647b-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="6647b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6647b-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="6647b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6647b-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="6647b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6647b-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6647b-163">createdDateTime</span></span>|<span data-ttu-id="6647b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6647b-164">DateTimeOffset</span></span>|<span data-ttu-id="6647b-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6647b-165">DateTime the object was created.</span></span> <span data-ttu-id="6647b-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-167">description</span><span class="sxs-lookup"><span data-stu-id="6647b-167">description</span></span>|<span data-ttu-id="6647b-168">String</span><span class="sxs-lookup"><span data-stu-id="6647b-168">String</span></span>|<span data-ttu-id="6647b-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="6647b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6647b-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6647b-171">displayName</span></span>|<span data-ttu-id="6647b-172">String</span><span class="sxs-lookup"><span data-stu-id="6647b-172">String</span></span>|<span data-ttu-id="6647b-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="6647b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6647b-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-175">version</span><span class="sxs-lookup"><span data-stu-id="6647b-175">version</span></span>|<span data-ttu-id="6647b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6647b-176">Int32</span></span>|<span data-ttu-id="6647b-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6647b-177">Version of the device configuration.</span></span> <span data-ttu-id="6647b-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6647b-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6647b-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="6647b-180">Int32</span><span class="sxs-lookup"><span data-stu-id="6647b-180">Int32</span></span>|<span data-ttu-id="6647b-181">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="6647b-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6647b-182">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承された有効な値 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="6647b-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6647b-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6647b-183">subjectNameFormat</span></span>|[<span data-ttu-id="6647b-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6647b-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6647b-185">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="6647b-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="6647b-186">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6647b-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6647b-187">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="6647b-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6647b-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6647b-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6647b-189">Int32</span><span class="sxs-lookup"><span data-stu-id="6647b-189">Int32</span></span>|<span data-ttu-id="6647b-190">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="6647b-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="6647b-191">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6647b-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6647b-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6647b-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6647b-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6647b-194">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="6647b-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="6647b-195">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6647b-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6647b-196">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="6647b-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6647b-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6647b-197">extendedKeyUsages</span></span>|<span data-ttu-id="6647b-198">[Extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6647b-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="6647b-199">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="6647b-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="6647b-200">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6647b-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6647b-201">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="6647b-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6647b-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6647b-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6647b-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6647b-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6647b-204">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="6647b-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="6647b-205">[Androidforwork Certificateprofilebase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6647b-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6647b-206">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="6647b-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="6647b-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="6647b-207">scepServerUrls</span></span>|<span data-ttu-id="6647b-208">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6647b-208">String collection</span></span>|<span data-ttu-id="6647b-209">SCEP サーバーの Url</span><span class="sxs-lookup"><span data-stu-id="6647b-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="6647b-210">Subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="6647b-210">subjectNameFormatString</span></span>|<span data-ttu-id="6647b-211">String</span><span class="sxs-lookup"><span data-stu-id="6647b-211">String</span></span>|<span data-ttu-id="6647b-212">SubjectNameFormat = Custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="6647b-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="6647b-213">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="6647b-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="6647b-214">keyUsage</span><span class="sxs-lookup"><span data-stu-id="6647b-214">keyUsage</span></span>|[<span data-ttu-id="6647b-215">keyUsages</span><span class="sxs-lookup"><span data-stu-id="6647b-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="6647b-216">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="6647b-216">SCEP Key Usage.</span></span> <span data-ttu-id="6647b-217">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="6647b-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="6647b-218">keySize</span><span class="sxs-lookup"><span data-stu-id="6647b-218">keySize</span></span>|[<span data-ttu-id="6647b-219">keySize</span><span class="sxs-lookup"><span data-stu-id="6647b-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="6647b-220">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="6647b-220">SCEP Key Size.</span></span> <span data-ttu-id="6647b-221">可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="6647b-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="6647b-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6647b-222">hashAlgorithm</span></span>|[<span data-ttu-id="6647b-223">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="6647b-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="6647b-224">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="6647b-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="6647b-225">可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="6647b-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="6647b-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6647b-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="6647b-227">String</span><span class="sxs-lookup"><span data-stu-id="6647b-227">String</span></span>|<span data-ttu-id="6647b-228">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="6647b-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="6647b-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="6647b-229">certificateStore</span></span>|[<span data-ttu-id="6647b-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="6647b-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="6647b-231">ターゲットストアの証明書。</span><span class="sxs-lookup"><span data-stu-id="6647b-231">Target store certificate.</span></span> <span data-ttu-id="6647b-232">可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="6647b-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="6647b-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="6647b-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="6647b-234">[Customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション</span><span class="sxs-lookup"><span data-stu-id="6647b-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="6647b-235">カスタムサブジェクトの別名設定。</span><span class="sxs-lookup"><span data-stu-id="6647b-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="6647b-236">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6647b-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6647b-237">応答</span><span class="sxs-lookup"><span data-stu-id="6647b-237">Response</span></span>
<span data-ttu-id="6647b-238">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6647b-238">If successful, this method returns a `201 Created` response code and a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6647b-239">例</span><span class="sxs-lookup"><span data-stu-id="6647b-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="6647b-240">要求</span><span class="sxs-lookup"><span data-stu-id="6647b-240">Request</span></span>
<span data-ttu-id="6647b-241">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6647b-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="6647b-242">応答</span><span class="sxs-lookup"><span data-stu-id="6647b-242">Response</span></span>
<span data-ttu-id="6647b-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6647b-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





