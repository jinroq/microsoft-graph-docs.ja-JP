---
title: windowsDefenderAdvancedThreatProtectionConfiguration の作成
description: 新しい windowsDefenderAdvancedThreatProtectionConfigurations オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f39fc97a648b7613baa7a034e97400e08ce40ee
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918067"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="95467-103">windowsDefenderAdvancedThreatProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="95467-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="95467-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95467-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95467-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95467-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95467-106">新しい [windowsDefenderAdvancedThreatProtectionConfigurations](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="95467-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95467-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="95467-107">Prerequisites</span></span>
<span data-ttu-id="95467-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95467-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95467-110">Permission type</span></span>|<span data-ttu-id="95467-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95467-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95467-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95467-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95467-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95467-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95467-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95467-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95467-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95467-115">Not supported.</span></span>|
|<span data-ttu-id="95467-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95467-116">Application</span></span>|<span data-ttu-id="95467-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95467-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95467-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95467-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="95467-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95467-119">Request headers</span></span>
|<span data-ttu-id="95467-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95467-120">Header</span></span>|<span data-ttu-id="95467-121">値</span><span class="sxs-lookup"><span data-stu-id="95467-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95467-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95467-122">Authorization</span></span>|<span data-ttu-id="95467-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95467-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95467-124">承諾</span><span class="sxs-lookup"><span data-stu-id="95467-124">Accept</span></span>|<span data-ttu-id="95467-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95467-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95467-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="95467-126">Request body</span></span>
<span data-ttu-id="95467-127">要求本文で、windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="95467-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="95467-128">次の表に、windowsDefenderAdvancedThreatProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="95467-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="95467-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95467-129">Property</span></span>|<span data-ttu-id="95467-130">型</span><span class="sxs-lookup"><span data-stu-id="95467-130">Type</span></span>|<span data-ttu-id="95467-131">説明</span><span class="sxs-lookup"><span data-stu-id="95467-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95467-132">id</span><span class="sxs-lookup"><span data-stu-id="95467-132">id</span></span>|<span data-ttu-id="95467-133">文字列</span><span class="sxs-lookup"><span data-stu-id="95467-133">String</span></span>|<span data-ttu-id="95467-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="95467-134">Key of the entity.</span></span> <span data-ttu-id="95467-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95467-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95467-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95467-136">lastModifiedDateTime</span></span>|<span data-ttu-id="95467-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95467-137">DateTimeOffset</span></span>|<span data-ttu-id="95467-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="95467-138">DateTime the object was last modified.</span></span> <span data-ttu-id="95467-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95467-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95467-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95467-140">roleScopeTagIds</span></span>|<span data-ttu-id="95467-141">String collection</span><span class="sxs-lookup"><span data-stu-id="95467-141">String collection</span></span>|<span data-ttu-id="95467-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="95467-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95467-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95467-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95467-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95467-144">supportsScopeTags</span></span>|<span data-ttu-id="95467-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="95467-145">Boolean</span></span>|<span data-ttu-id="95467-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="95467-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95467-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="95467-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95467-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="95467-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95467-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="95467-149">This property is read-only.</span></span> <span data-ttu-id="95467-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95467-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95467-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95467-151">createdDateTime</span></span>|<span data-ttu-id="95467-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95467-152">DateTimeOffset</span></span>|<span data-ttu-id="95467-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="95467-153">DateTime the object was created.</span></span> <span data-ttu-id="95467-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95467-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95467-155">description</span><span class="sxs-lookup"><span data-stu-id="95467-155">description</span></span>|<span data-ttu-id="95467-156">String</span><span class="sxs-lookup"><span data-stu-id="95467-156">String</span></span>|<span data-ttu-id="95467-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="95467-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95467-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95467-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95467-159">displayName</span><span class="sxs-lookup"><span data-stu-id="95467-159">displayName</span></span>|<span data-ttu-id="95467-160">String</span><span class="sxs-lookup"><span data-stu-id="95467-160">String</span></span>|<span data-ttu-id="95467-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="95467-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95467-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95467-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95467-163">version</span><span class="sxs-lookup"><span data-stu-id="95467-163">version</span></span>|<span data-ttu-id="95467-164">Int32</span><span class="sxs-lookup"><span data-stu-id="95467-164">Int32</span></span>|<span data-ttu-id="95467-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="95467-165">Version of the device configuration.</span></span> <span data-ttu-id="95467-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95467-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95467-167">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="95467-167">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="95467-168">String</span><span class="sxs-lookup"><span data-stu-id="95467-168">String</span></span>|<span data-ttu-id="95467-169">Windows Defender AdvancedThreatProtection オンボード Blob。</span><span class="sxs-lookup"><span data-stu-id="95467-169">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="95467-170">追加</span><span class="sxs-lookup"><span data-stu-id="95467-170">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="95467-171">String</span><span class="sxs-lookup"><span data-stu-id="95467-171">String</span></span>|<span data-ttu-id="95467-172">AdvancedThreatProtectionOnboardingBlob が取得されたファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="95467-172">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="95467-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="95467-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="95467-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="95467-174">Boolean</span></span>|<span data-ttu-id="95467-175">Advanced Threat protection サービスからプログラムによって、オンボード blob を自動入力する</span><span class="sxs-lookup"><span data-stu-id="95467-175">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="95467-176">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="95467-176">allowSampleSharing</span></span>|<span data-ttu-id="95467-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="95467-177">Boolean</span></span>|<span data-ttu-id="95467-178">Windows Defender AdvancedThreatProtection の "サンプルの共有を許可する" ルール</span><span class="sxs-lookup"><span data-stu-id="95467-178">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="95467-179">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="95467-179">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="95467-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="95467-180">Boolean</span></span>|<span data-ttu-id="95467-181">Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。</span><span class="sxs-lookup"><span data-stu-id="95467-181">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="95467-182">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="95467-182">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="95467-183">String</span><span class="sxs-lookup"><span data-stu-id="95467-183">String</span></span>|<span data-ttu-id="95467-184">Windows Defender AdvancedThreatProtection オフボード Blob。</span><span class="sxs-lookup"><span data-stu-id="95467-184">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="95467-185">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="95467-185">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="95467-186">String</span><span class="sxs-lookup"><span data-stu-id="95467-186">String</span></span>|<span data-ttu-id="95467-187">AdvancedThreatProtectionOffboardingBlob が取得されたファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="95467-187">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="95467-188">応答</span><span class="sxs-lookup"><span data-stu-id="95467-188">Response</span></span>
<span data-ttu-id="95467-189">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95467-189">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95467-190">例</span><span class="sxs-lookup"><span data-stu-id="95467-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="95467-191">要求</span><span class="sxs-lookup"><span data-stu-id="95467-191">Request</span></span>
<span data-ttu-id="95467-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95467-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 830

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="95467-193">応答</span><span class="sxs-lookup"><span data-stu-id="95467-193">Response</span></span>
<span data-ttu-id="95467-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95467-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1002

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




