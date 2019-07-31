---
title: iosUpdateConfiguration の作成
description: 新しい iosUpdateConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dbf939c7731461ba7e3d31eec44a9a1d79c94765
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947880"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="559a4-103">iosUpdateConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="559a4-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="559a4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="559a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="559a4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="559a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="559a4-106">新しい [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="559a4-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="559a4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="559a4-107">Prerequisites</span></span>
<span data-ttu-id="559a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="559a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="559a4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="559a4-110">Permission type</span></span>|<span data-ttu-id="559a4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="559a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="559a4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="559a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="559a4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="559a4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="559a4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="559a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="559a4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="559a4-115">Not supported.</span></span>|
|<span data-ttu-id="559a4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="559a4-116">Application</span></span>|<span data-ttu-id="559a4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="559a4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="559a4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="559a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="559a4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="559a4-119">Request headers</span></span>
|<span data-ttu-id="559a4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="559a4-120">Header</span></span>|<span data-ttu-id="559a4-121">値</span><span class="sxs-lookup"><span data-stu-id="559a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="559a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="559a4-122">Authorization</span></span>|<span data-ttu-id="559a4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="559a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="559a4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="559a4-124">Accept</span></span>|<span data-ttu-id="559a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="559a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="559a4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="559a4-126">Request body</span></span>
<span data-ttu-id="559a4-127">要求本文で、iosUpdateConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="559a4-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="559a4-128">次の表に、iosUpdateConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="559a4-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="559a4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="559a4-129">Property</span></span>|<span data-ttu-id="559a4-130">型</span><span class="sxs-lookup"><span data-stu-id="559a4-130">Type</span></span>|<span data-ttu-id="559a4-131">説明</span><span class="sxs-lookup"><span data-stu-id="559a4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="559a4-132">id</span><span class="sxs-lookup"><span data-stu-id="559a4-132">id</span></span>|<span data-ttu-id="559a4-133">文字列</span><span class="sxs-lookup"><span data-stu-id="559a4-133">String</span></span>|<span data-ttu-id="559a4-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="559a4-134">Key of the entity.</span></span> <span data-ttu-id="559a4-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="559a4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="559a4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="559a4-137">DateTimeOffset</span></span>|<span data-ttu-id="559a4-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="559a4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="559a4-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="559a4-140">roleScopeTagIds</span></span>|<span data-ttu-id="559a4-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="559a4-141">String collection</span></span>|<span data-ttu-id="559a4-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="559a4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="559a4-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="559a4-144">supportsScopeTags</span></span>|<span data-ttu-id="559a4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="559a4-145">Boolean</span></span>|<span data-ttu-id="559a4-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="559a4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="559a4-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="559a4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="559a4-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="559a4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="559a4-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="559a4-149">This property is read-only.</span></span> <span data-ttu-id="559a4-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="559a4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="559a4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="559a4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="559a4-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="559a4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="559a4-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="559a4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="559a4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="559a4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="559a4-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="559a4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="559a4-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="559a4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="559a4-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="559a4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="559a4-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="559a4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="559a4-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="559a4-163">createdDateTime</span></span>|<span data-ttu-id="559a4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="559a4-164">DateTimeOffset</span></span>|<span data-ttu-id="559a4-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="559a4-165">DateTime the object was created.</span></span> <span data-ttu-id="559a4-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-167">description</span><span class="sxs-lookup"><span data-stu-id="559a4-167">description</span></span>|<span data-ttu-id="559a4-168">String</span><span class="sxs-lookup"><span data-stu-id="559a4-168">String</span></span>|<span data-ttu-id="559a4-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="559a4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="559a4-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="559a4-171">displayName</span></span>|<span data-ttu-id="559a4-172">String</span><span class="sxs-lookup"><span data-stu-id="559a4-172">String</span></span>|<span data-ttu-id="559a4-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="559a4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="559a4-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-175">version</span><span class="sxs-lookup"><span data-stu-id="559a4-175">version</span></span>|<span data-ttu-id="559a4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="559a4-176">Int32</span></span>|<span data-ttu-id="559a4-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="559a4-177">Version of the device configuration.</span></span> <span data-ttu-id="559a4-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="559a4-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="559a4-179">isEnabled</span><span class="sxs-lookup"><span data-stu-id="559a4-179">isEnabled</span></span>|<span data-ttu-id="559a4-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="559a4-180">Boolean</span></span>|<span data-ttu-id="559a4-181">UI での設定の有効化</span><span class="sxs-lookup"><span data-stu-id="559a4-181">Is setting enabled in UI</span></span>|
|<span data-ttu-id="559a4-182">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="559a4-182">activeHoursStart</span></span>|<span data-ttu-id="559a4-183">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="559a4-183">TimeOfDay</span></span>|<span data-ttu-id="559a4-184">アクティブ時間の開始 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="559a4-184">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="559a4-185">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="559a4-185">activeHoursEnd</span></span>|<span data-ttu-id="559a4-186">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="559a4-186">TimeOfDay</span></span>|<span data-ttu-id="559a4-187">アクティブ時間の終了 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="559a4-187">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="559a4-188">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="559a4-188">scheduledInstallDays</span></span>|<span data-ttu-id="559a4-189">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="559a4-189">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="559a4-190">アクティブ時間が設定されている曜日。</span><span class="sxs-lookup"><span data-stu-id="559a4-190">Days in week for which active hours are configured.</span></span> <span data-ttu-id="559a4-191">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="559a4-191">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="559a4-192">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="559a4-192">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="559a4-193">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="559a4-193">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="559a4-194">Int32</span><span class="sxs-lookup"><span data-stu-id="559a4-194">Int32</span></span>|<span data-ttu-id="559a4-195">UTC タイム オフセット (分単位で示されます)</span><span class="sxs-lookup"><span data-stu-id="559a4-195">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="559a4-196">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="559a4-196">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="559a4-197">Int32</span><span class="sxs-lookup"><span data-stu-id="559a4-197">Int32</span></span>|<span data-ttu-id="559a4-198">ソフトウェア更新プログラムが iOS デバイスに表示されるまでの日数。 0 ~ 90 の範囲内にある。</span><span class="sxs-lookup"><span data-stu-id="559a4-198">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="559a4-199">応答</span><span class="sxs-lookup"><span data-stu-id="559a4-199">Response</span></span>
<span data-ttu-id="559a4-200">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="559a4-200">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="559a4-201">例</span><span class="sxs-lookup"><span data-stu-id="559a4-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="559a4-202">要求</span><span class="sxs-lookup"><span data-stu-id="559a4-202">Request</span></span>
<span data-ttu-id="559a4-203">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="559a4-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1255

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="559a4-204">応答</span><span class="sxs-lookup"><span data-stu-id="559a4-204">Response</span></span>
<span data-ttu-id="559a4-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="559a4-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1427

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





