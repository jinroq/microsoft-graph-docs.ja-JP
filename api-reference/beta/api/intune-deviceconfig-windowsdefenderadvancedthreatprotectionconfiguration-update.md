---
title: windowsDefenderAdvancedThreatProtectionConfiguration の更新
description: windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fea7f12f3ea6e90aaeea38d828dbe072b2995430
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396372"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="d1893-103">windowsDefenderAdvancedThreatProtectionConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d1893-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="d1893-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1893-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1893-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1893-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1893-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1893-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1893-107">[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d1893-107">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1893-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d1893-108">Prerequisites</span></span>
<span data-ttu-id="d1893-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1893-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d1893-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1893-111">Permission type</span></span>|<span data-ttu-id="d1893-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1893-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1893-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1893-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1893-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1893-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1893-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1893-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1893-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1893-116">Not supported.</span></span>|
|<span data-ttu-id="d1893-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1893-117">Application</span></span>|<span data-ttu-id="d1893-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1893-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1893-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1893-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d1893-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1893-120">Request headers</span></span>
|<span data-ttu-id="d1893-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1893-121">Header</span></span>|<span data-ttu-id="d1893-122">値</span><span class="sxs-lookup"><span data-stu-id="d1893-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1893-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1893-123">Authorization</span></span>|<span data-ttu-id="d1893-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d1893-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1893-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1893-125">Accept</span></span>|<span data-ttu-id="d1893-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1893-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1893-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1893-127">Request body</span></span>
<span data-ttu-id="d1893-128">要求本文で、[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1893-128">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="d1893-129">次の表に、[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d1893-129">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="d1893-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1893-130">Property</span></span>|<span data-ttu-id="d1893-131">型</span><span class="sxs-lookup"><span data-stu-id="d1893-131">Type</span></span>|<span data-ttu-id="d1893-132">説明</span><span class="sxs-lookup"><span data-stu-id="d1893-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1893-133">id</span><span class="sxs-lookup"><span data-stu-id="d1893-133">id</span></span>|<span data-ttu-id="d1893-134">String</span><span class="sxs-lookup"><span data-stu-id="d1893-134">String</span></span>|<span data-ttu-id="d1893-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d1893-135">Key of the entity.</span></span> <span data-ttu-id="d1893-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1893-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1893-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1893-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d1893-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1893-138">DateTimeOffset</span></span>|<span data-ttu-id="d1893-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d1893-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d1893-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1893-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1893-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d1893-141">roleScopeTagIds</span></span>|<span data-ttu-id="d1893-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d1893-142">String collection</span></span>|<span data-ttu-id="d1893-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="d1893-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d1893-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1893-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1893-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d1893-145">supportsScopeTags</span></span>|<span data-ttu-id="d1893-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1893-146">Boolean</span></span>|<span data-ttu-id="d1893-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d1893-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d1893-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="d1893-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d1893-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="d1893-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d1893-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d1893-150">This property is read-only.</span></span> <span data-ttu-id="d1893-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1893-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1893-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1893-152">createdDateTime</span></span>|<span data-ttu-id="d1893-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1893-153">DateTimeOffset</span></span>|<span data-ttu-id="d1893-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d1893-154">DateTime the object was created.</span></span> <span data-ttu-id="d1893-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1893-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1893-156">説明</span><span class="sxs-lookup"><span data-stu-id="d1893-156">description</span></span>|<span data-ttu-id="d1893-157">String</span><span class="sxs-lookup"><span data-stu-id="d1893-157">String</span></span>|<span data-ttu-id="d1893-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d1893-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d1893-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1893-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1893-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d1893-160">displayName</span></span>|<span data-ttu-id="d1893-161">String</span><span class="sxs-lookup"><span data-stu-id="d1893-161">String</span></span>|<span data-ttu-id="d1893-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d1893-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d1893-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1893-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1893-164">version</span><span class="sxs-lookup"><span data-stu-id="d1893-164">version</span></span>|<span data-ttu-id="d1893-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d1893-165">Int32</span></span>|<span data-ttu-id="d1893-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d1893-166">Version of the device configuration.</span></span> <span data-ttu-id="d1893-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1893-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1893-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="d1893-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="d1893-169">String</span><span class="sxs-lookup"><span data-stu-id="d1893-169">String</span></span>|<span data-ttu-id="d1893-170">Windows Defender AdvancedThreatProtection 契約時の Blob です。</span><span class="sxs-lookup"><span data-stu-id="d1893-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="d1893-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="d1893-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="d1893-172">String</span><span class="sxs-lookup"><span data-stu-id="d1893-172">String</span></span>|<span data-ttu-id="d1893-173">AdvancedThreatProtectionOnboardingBlob の取得元となるファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="d1893-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="d1893-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="d1893-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="d1893-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1893-175">Boolean</span></span>|<span data-ttu-id="d1893-176">自動は、プログラムを使用して、脅威の高度な保護のサービスからの契約時の blob を挿入します。</span><span class="sxs-lookup"><span data-stu-id="d1893-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="d1893-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="d1893-177">allowSampleSharing</span></span>|<span data-ttu-id="d1893-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1893-178">Boolean</span></span>|<span data-ttu-id="d1893-179">Windows Defender AdvancedThreatProtection の "サンプルの共有を許可する" ルール</span><span class="sxs-lookup"><span data-stu-id="d1893-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="d1893-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="d1893-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="d1893-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1893-181">Boolean</span></span>|<span data-ttu-id="d1893-182">Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。</span><span class="sxs-lookup"><span data-stu-id="d1893-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="d1893-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="d1893-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="d1893-184">String</span><span class="sxs-lookup"><span data-stu-id="d1893-184">String</span></span>|<span data-ttu-id="d1893-185">Windows Defender の AdvancedThreatProtection の Offboarding の Blob です。</span><span class="sxs-lookup"><span data-stu-id="d1893-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="d1893-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="d1893-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="d1893-187">String</span><span class="sxs-lookup"><span data-stu-id="d1893-187">String</span></span>|<span data-ttu-id="d1893-188">AdvancedThreatProtectionOffboardingBlob の取得元となるファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="d1893-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="d1893-189">応答</span><span class="sxs-lookup"><span data-stu-id="d1893-189">Response</span></span>
<span data-ttu-id="d1893-190">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1893-190">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1893-191">例</span><span class="sxs-lookup"><span data-stu-id="d1893-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1893-192">要求</span><span class="sxs-lookup"><span data-stu-id="d1893-192">Request</span></span>
<span data-ttu-id="d1893-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1893-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="d1893-194">応答</span><span class="sxs-lookup"><span data-stu-id="d1893-194">Response</span></span>
<span data-ttu-id="d1893-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d1893-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




