---
title: windowsDefenderAdvancedThreatProtectionConfiguration の更新
description: windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecf4d33b3bf03ed9c658f6210f2d2b952634eaea
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344596"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="8cd5d-103">windowsDefenderAdvancedThreatProtectionConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="8cd5d-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="8cd5d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cd5d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cd5d-106">[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-106">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cd5d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8cd5d-107">Prerequisites</span></span>
<span data-ttu-id="8cd5d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cd5d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cd5d-110">Permission type</span></span>|<span data-ttu-id="8cd5d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cd5d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cd5d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cd5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cd5d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd5d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8cd5d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cd5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cd5d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-115">Not supported.</span></span>|
|<span data-ttu-id="8cd5d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cd5d-116">Application</span></span>|<span data-ttu-id="8cd5d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd5d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cd5d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cd5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8cd5d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cd5d-119">Request headers</span></span>
|<span data-ttu-id="8cd5d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cd5d-120">Header</span></span>|<span data-ttu-id="8cd5d-121">値</span><span class="sxs-lookup"><span data-stu-id="8cd5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cd5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cd5d-122">Authorization</span></span>|<span data-ttu-id="8cd5d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cd5d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8cd5d-124">Accept</span></span>|<span data-ttu-id="8cd5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8cd5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cd5d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cd5d-126">Request body</span></span>
<span data-ttu-id="8cd5d-127">要求本文で、[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-127">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="8cd5d-128">次の表に、[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-128">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="8cd5d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cd5d-129">Property</span></span>|<span data-ttu-id="8cd5d-130">型</span><span class="sxs-lookup"><span data-stu-id="8cd5d-130">Type</span></span>|<span data-ttu-id="8cd5d-131">説明</span><span class="sxs-lookup"><span data-stu-id="8cd5d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cd5d-132">id</span><span class="sxs-lookup"><span data-stu-id="8cd5d-132">id</span></span>|<span data-ttu-id="8cd5d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8cd5d-133">String</span></span>|<span data-ttu-id="8cd5d-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-134">Key of the entity.</span></span> <span data-ttu-id="8cd5d-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cd5d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8cd5d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cd5d-137">DateTimeOffset</span></span>|<span data-ttu-id="8cd5d-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8cd5d-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8cd5d-140">roleScopeTagIds</span></span>|<span data-ttu-id="8cd5d-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8cd5d-141">String collection</span></span>|<span data-ttu-id="8cd5d-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8cd5d-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8cd5d-144">supportsScopeTags</span></span>|<span data-ttu-id="8cd5d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cd5d-145">Boolean</span></span>|<span data-ttu-id="8cd5d-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8cd5d-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8cd5d-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8cd5d-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-149">This property is read-only.</span></span> <span data-ttu-id="8cd5d-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8cd5d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8cd5d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8cd5d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8cd5d-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8cd5d-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8cd5d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8cd5d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8cd5d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8cd5d-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8cd5d-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="8cd5d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8cd5d-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="8cd5d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8cd5d-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8cd5d-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cd5d-163">createdDateTime</span></span>|<span data-ttu-id="8cd5d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cd5d-164">DateTimeOffset</span></span>|<span data-ttu-id="8cd5d-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-165">DateTime the object was created.</span></span> <span data-ttu-id="8cd5d-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-167">description</span><span class="sxs-lookup"><span data-stu-id="8cd5d-167">description</span></span>|<span data-ttu-id="8cd5d-168">String</span><span class="sxs-lookup"><span data-stu-id="8cd5d-168">String</span></span>|<span data-ttu-id="8cd5d-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8cd5d-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8cd5d-171">displayName</span></span>|<span data-ttu-id="8cd5d-172">String</span><span class="sxs-lookup"><span data-stu-id="8cd5d-172">String</span></span>|<span data-ttu-id="8cd5d-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8cd5d-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-175">version</span><span class="sxs-lookup"><span data-stu-id="8cd5d-175">version</span></span>|<span data-ttu-id="8cd5d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8cd5d-176">Int32</span></span>|<span data-ttu-id="8cd5d-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-177">Version of the device configuration.</span></span> <span data-ttu-id="8cd5d-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8cd5d-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cd5d-179">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8cd5d-179">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="8cd5d-180">String</span><span class="sxs-lookup"><span data-stu-id="8cd5d-180">String</span></span>|<span data-ttu-id="8cd5d-181">Windows Defender AdvancedThreatProtection オンボード Blob。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-181">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="8cd5d-182">追加</span><span class="sxs-lookup"><span data-stu-id="8cd5d-182">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="8cd5d-183">String</span><span class="sxs-lookup"><span data-stu-id="8cd5d-183">String</span></span>|<span data-ttu-id="8cd5d-184">AdvancedThreatProtectionOnboardingBlob が取得されたファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-184">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="8cd5d-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8cd5d-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="8cd5d-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cd5d-186">Boolean</span></span>|<span data-ttu-id="8cd5d-187">Advanced Threat protection サービスからプログラムによって、オンボード blob を自動入力する</span><span class="sxs-lookup"><span data-stu-id="8cd5d-187">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="8cd5d-188">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="8cd5d-188">allowSampleSharing</span></span>|<span data-ttu-id="8cd5d-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cd5d-189">Boolean</span></span>|<span data-ttu-id="8cd5d-190">Windows Defender AdvancedThreatProtection の "サンプルの共有を許可する" ルール</span><span class="sxs-lookup"><span data-stu-id="8cd5d-190">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="8cd5d-191">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="8cd5d-191">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="8cd5d-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cd5d-192">Boolean</span></span>|<span data-ttu-id="8cd5d-193">Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-193">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="8cd5d-194">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8cd5d-194">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="8cd5d-195">String</span><span class="sxs-lookup"><span data-stu-id="8cd5d-195">String</span></span>|<span data-ttu-id="8cd5d-196">Windows Defender AdvancedThreatProtection オフボード Blob。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-196">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="8cd5d-197">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="8cd5d-197">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="8cd5d-198">String</span><span class="sxs-lookup"><span data-stu-id="8cd5d-198">String</span></span>|<span data-ttu-id="8cd5d-199">AdvancedThreatProtectionOffboardingBlob が取得されたファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-199">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="8cd5d-200">応答</span><span class="sxs-lookup"><span data-stu-id="8cd5d-200">Response</span></span>
<span data-ttu-id="8cd5d-201">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-201">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cd5d-202">例</span><span class="sxs-lookup"><span data-stu-id="8cd5d-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cd5d-203">要求</span><span class="sxs-lookup"><span data-stu-id="8cd5d-203">Request</span></span>
<span data-ttu-id="8cd5d-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1603

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
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
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```

### <a name="response"></a><span data-ttu-id="8cd5d-205">応答</span><span class="sxs-lookup"><span data-stu-id="8cd5d-205">Response</span></span>
<span data-ttu-id="8cd5d-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8cd5d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1775

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
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
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```






