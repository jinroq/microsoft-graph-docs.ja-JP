---
title: windowsDefenderAdvancedThreatProtectionConfiguration の作成
description: 新しい windowsDefenderAdvancedThreatProtectionConfigurations オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: ab9dbf4132c18e40e4a72194d1fe456a2777d02e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313308"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="8bc2d-103">windowsDefenderAdvancedThreatProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="8bc2d-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="8bc2d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bc2d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8bc2d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bc2d-107">新しい [windowsDefenderAdvancedThreatProtectionConfigurations](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-107">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8bc2d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8bc2d-108">Prerequisites</span></span>
<span data-ttu-id="8bc2d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bc2d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bc2d-111">Permission type</span></span>|<span data-ttu-id="8bc2d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bc2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bc2d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bc2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bc2d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bc2d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bc2d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bc2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bc2d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-116">Not supported.</span></span>|
|<span data-ttu-id="8bc2d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bc2d-117">Application</span></span>|<span data-ttu-id="8bc2d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bc2d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bc2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8bc2d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bc2d-120">Request headers</span></span>
|<span data-ttu-id="8bc2d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bc2d-121">Header</span></span>|<span data-ttu-id="8bc2d-122">値</span><span class="sxs-lookup"><span data-stu-id="8bc2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bc2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bc2d-123">Authorization</span></span>|<span data-ttu-id="8bc2d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bc2d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8bc2d-125">Accept</span></span>|<span data-ttu-id="8bc2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bc2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bc2d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bc2d-127">Request body</span></span>
<span data-ttu-id="8bc2d-128">要求本文で、windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-128">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="8bc2d-129">次の表に、windowsDefenderAdvancedThreatProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-129">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="8bc2d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bc2d-130">Property</span></span>|<span data-ttu-id="8bc2d-131">種類</span><span class="sxs-lookup"><span data-stu-id="8bc2d-131">Type</span></span>|<span data-ttu-id="8bc2d-132">説明</span><span class="sxs-lookup"><span data-stu-id="8bc2d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc2d-133">ID</span><span class="sxs-lookup"><span data-stu-id="8bc2d-133">id</span></span>|<span data-ttu-id="8bc2d-134">String</span><span class="sxs-lookup"><span data-stu-id="8bc2d-134">String</span></span>|<span data-ttu-id="8bc2d-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-135">Key of the entity.</span></span> <span data-ttu-id="8bc2d-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bc2d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc2d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bc2d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8bc2d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc2d-138">DateTimeOffset</span></span>|<span data-ttu-id="8bc2d-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8bc2d-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bc2d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc2d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8bc2d-141">roleScopeTagIds</span></span>|<span data-ttu-id="8bc2d-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8bc2d-142">String collection</span></span>|<span data-ttu-id="8bc2d-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8bc2d-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bc2d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc2d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8bc2d-145">supportsScopeTags</span></span>|<span data-ttu-id="8bc2d-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="8bc2d-146">Boolean</span></span>|<span data-ttu-id="8bc2d-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8bc2d-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8bc2d-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8bc2d-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-150">This property is read-only.</span></span> <span data-ttu-id="8bc2d-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bc2d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc2d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bc2d-152">createdDateTime</span></span>|<span data-ttu-id="8bc2d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc2d-153">DateTimeOffset</span></span>|<span data-ttu-id="8bc2d-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-154">DateTime the object was created.</span></span> <span data-ttu-id="8bc2d-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bc2d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc2d-156">説明</span><span class="sxs-lookup"><span data-stu-id="8bc2d-156">description</span></span>|<span data-ttu-id="8bc2d-157">String</span><span class="sxs-lookup"><span data-stu-id="8bc2d-157">String</span></span>|<span data-ttu-id="8bc2d-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8bc2d-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bc2d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc2d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8bc2d-160">displayName</span></span>|<span data-ttu-id="8bc2d-161">String</span><span class="sxs-lookup"><span data-stu-id="8bc2d-161">String</span></span>|<span data-ttu-id="8bc2d-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8bc2d-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bc2d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc2d-164">version</span><span class="sxs-lookup"><span data-stu-id="8bc2d-164">version</span></span>|<span data-ttu-id="8bc2d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8bc2d-165">Int32</span></span>|<span data-ttu-id="8bc2d-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-166">Version of the device configuration.</span></span> <span data-ttu-id="8bc2d-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bc2d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc2d-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8bc2d-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="8bc2d-169">String</span><span class="sxs-lookup"><span data-stu-id="8bc2d-169">String</span></span>|<span data-ttu-id="8bc2d-170">Windows Defender AdvancedThreatProtection 契約時の Blob です。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="8bc2d-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="8bc2d-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="8bc2d-172">String</span><span class="sxs-lookup"><span data-stu-id="8bc2d-172">String</span></span>|<span data-ttu-id="8bc2d-173">AdvancedThreatProtectionOnboardingBlob の取得元となるファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="8bc2d-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8bc2d-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="8bc2d-175">ブール型</span><span class="sxs-lookup"><span data-stu-id="8bc2d-175">Boolean</span></span>|<span data-ttu-id="8bc2d-176">自動は、プログラムを使用して、脅威の高度な保護のサービスからの契約時の blob を挿入します。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="8bc2d-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="8bc2d-177">allowSampleSharing</span></span>|<span data-ttu-id="8bc2d-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bc2d-178">Boolean</span></span>|<span data-ttu-id="8bc2d-179">Windows Defender AdvancedThreatProtection の "サンプルの共有を許可する" ルール</span><span class="sxs-lookup"><span data-stu-id="8bc2d-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="8bc2d-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="8bc2d-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="8bc2d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bc2d-181">Boolean</span></span>|<span data-ttu-id="8bc2d-182">Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="8bc2d-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8bc2d-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="8bc2d-184">String</span><span class="sxs-lookup"><span data-stu-id="8bc2d-184">String</span></span>|<span data-ttu-id="8bc2d-185">Windows Defender の AdvancedThreatProtection の Offboarding の Blob です。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="8bc2d-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="8bc2d-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="8bc2d-187">String</span><span class="sxs-lookup"><span data-stu-id="8bc2d-187">String</span></span>|<span data-ttu-id="8bc2d-188">AdvancedThreatProtectionOffboardingBlob の取得元となるファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="8bc2d-189">応答</span><span class="sxs-lookup"><span data-stu-id="8bc2d-189">Response</span></span>
<span data-ttu-id="8bc2d-190">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-190">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bc2d-191">例</span><span class="sxs-lookup"><span data-stu-id="8bc2d-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="8bc2d-192">要求</span><span class="sxs-lookup"><span data-stu-id="8bc2d-192">Request</span></span>
<span data-ttu-id="8bc2d-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 894

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="8bc2d-194">応答</span><span class="sxs-lookup"><span data-stu-id="8bc2d-194">Response</span></span>
<span data-ttu-id="8bc2d-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8bc2d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





