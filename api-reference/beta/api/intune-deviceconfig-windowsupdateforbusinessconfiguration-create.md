---
title: Create windowsUpdateForBusinessConfiguration
description: 新しい windowsUpdateForBusinessConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94b81dd406e3ed4bb7cc1071f1a9f3604b7b492d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986296"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="02d51-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="02d51-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="02d51-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02d51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02d51-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="02d51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02d51-106">新しい [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="02d51-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02d51-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="02d51-107">Prerequisites</span></span>
<span data-ttu-id="02d51-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02d51-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02d51-110">Permission type</span></span>|<span data-ttu-id="02d51-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="02d51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02d51-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02d51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02d51-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02d51-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02d51-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02d51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02d51-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02d51-115">Not supported.</span></span>|
|<span data-ttu-id="02d51-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02d51-116">Application</span></span>|<span data-ttu-id="02d51-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02d51-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02d51-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02d51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="02d51-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02d51-119">Request headers</span></span>
|<span data-ttu-id="02d51-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02d51-120">Header</span></span>|<span data-ttu-id="02d51-121">値</span><span class="sxs-lookup"><span data-stu-id="02d51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02d51-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="02d51-122">Authorization</span></span>|<span data-ttu-id="02d51-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="02d51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02d51-124">承諾</span><span class="sxs-lookup"><span data-stu-id="02d51-124">Accept</span></span>|<span data-ttu-id="02d51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02d51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02d51-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="02d51-126">Request body</span></span>
<span data-ttu-id="02d51-127">要求本文で、windowsUpdateForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="02d51-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="02d51-128">次の表に、windowsUpdateForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="02d51-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="02d51-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02d51-129">Property</span></span>|<span data-ttu-id="02d51-130">型</span><span class="sxs-lookup"><span data-stu-id="02d51-130">Type</span></span>|<span data-ttu-id="02d51-131">説明</span><span class="sxs-lookup"><span data-stu-id="02d51-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02d51-132">id</span><span class="sxs-lookup"><span data-stu-id="02d51-132">id</span></span>|<span data-ttu-id="02d51-133">文字列</span><span class="sxs-lookup"><span data-stu-id="02d51-133">String</span></span>|<span data-ttu-id="02d51-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="02d51-134">Key of the entity.</span></span> <span data-ttu-id="02d51-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02d51-136">lastModifiedDateTime</span></span>|<span data-ttu-id="02d51-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d51-137">DateTimeOffset</span></span>|<span data-ttu-id="02d51-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="02d51-138">DateTime the object was last modified.</span></span> <span data-ttu-id="02d51-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="02d51-140">roleScopeTagIds</span></span>|<span data-ttu-id="02d51-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="02d51-141">String collection</span></span>|<span data-ttu-id="02d51-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="02d51-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="02d51-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="02d51-144">supportsScopeTags</span></span>|<span data-ttu-id="02d51-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d51-145">Boolean</span></span>|<span data-ttu-id="02d51-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02d51-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="02d51-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="02d51-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="02d51-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="02d51-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="02d51-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="02d51-149">This property is read-only.</span></span> <span data-ttu-id="02d51-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="02d51-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="02d51-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="02d51-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="02d51-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="02d51-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="02d51-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="02d51-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="02d51-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="02d51-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="02d51-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="02d51-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="02d51-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="02d51-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="02d51-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="02d51-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="02d51-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="02d51-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="02d51-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02d51-163">createdDateTime</span></span>|<span data-ttu-id="02d51-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d51-164">DateTimeOffset</span></span>|<span data-ttu-id="02d51-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="02d51-165">DateTime the object was created.</span></span> <span data-ttu-id="02d51-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-167">description</span><span class="sxs-lookup"><span data-stu-id="02d51-167">description</span></span>|<span data-ttu-id="02d51-168">String</span><span class="sxs-lookup"><span data-stu-id="02d51-168">String</span></span>|<span data-ttu-id="02d51-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="02d51-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="02d51-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-171">displayName</span><span class="sxs-lookup"><span data-stu-id="02d51-171">displayName</span></span>|<span data-ttu-id="02d51-172">String</span><span class="sxs-lookup"><span data-stu-id="02d51-172">String</span></span>|<span data-ttu-id="02d51-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="02d51-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="02d51-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-175">version</span><span class="sxs-lookup"><span data-stu-id="02d51-175">version</span></span>|<span data-ttu-id="02d51-176">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-176">Int32</span></span>|<span data-ttu-id="02d51-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="02d51-177">Version of the device configuration.</span></span> <span data-ttu-id="02d51-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02d51-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02d51-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="02d51-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="02d51-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="02d51-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="02d51-181">配信最適化モード。</span><span class="sxs-lookup"><span data-stu-id="02d51-181">Delivery Optimization Mode.</span></span> <span data-ttu-id="02d51-182">可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="02d51-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="02d51-183">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="02d51-183">prereleaseFeatures</span></span>|[<span data-ttu-id="02d51-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="02d51-184">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="02d51-185">プレリリース機能。</span><span class="sxs-lookup"><span data-stu-id="02d51-185">The pre-release features.</span></span> <span data-ttu-id="02d51-186">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="02d51-186">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="02d51-187">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="02d51-187">automaticUpdateMode</span></span>|[<span data-ttu-id="02d51-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="02d51-188">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="02d51-189">自動更新モード。</span><span class="sxs-lookup"><span data-stu-id="02d51-189">Automatic update mode.</span></span> <span data-ttu-id="02d51-190">可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`、`windowsDefault` です。</span><span class="sxs-lookup"><span data-stu-id="02d51-190">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="02d51-191">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="02d51-191">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="02d51-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d51-192">Boolean</span></span>|<span data-ttu-id="02d51-193">Microsoft Update サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="02d51-193">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="02d51-194">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="02d51-194">driversExcluded</span></span>|<span data-ttu-id="02d51-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d51-195">Boolean</span></span>|<span data-ttu-id="02d51-196">Windows Update のドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="02d51-196">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="02d51-197">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="02d51-197">installationSchedule</span></span>|[<span data-ttu-id="02d51-198">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="02d51-198">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="02d51-199">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="02d51-199">Installation schedule</span></span>|
|<span data-ttu-id="02d51-200">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="02d51-200">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="02d51-201">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-201">Int32</span></span>|<span data-ttu-id="02d51-202">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="02d51-202">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="02d51-203">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="02d51-203">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="02d51-204">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-204">Int32</span></span>|<span data-ttu-id="02d51-205">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="02d51-205">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="02d51-206">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="02d51-206">qualityUpdatesPaused</span></span>|<span data-ttu-id="02d51-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d51-207">Boolean</span></span>|<span data-ttu-id="02d51-208">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="02d51-208">Pause Quality Updates</span></span>|
|<span data-ttu-id="02d51-209">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="02d51-209">featureUpdatesPaused</span></span>|<span data-ttu-id="02d51-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d51-210">Boolean</span></span>|<span data-ttu-id="02d51-211">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="02d51-211">Pause Feature Updates</span></span>|
|<span data-ttu-id="02d51-212">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="02d51-212">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="02d51-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d51-213">DateTimeOffset</span></span>|<span data-ttu-id="02d51-214">品質更新プログラムの一時停止が終了する日時</span><span class="sxs-lookup"><span data-stu-id="02d51-214">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="02d51-215">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="02d51-215">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="02d51-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d51-216">DateTimeOffset</span></span>|<span data-ttu-id="02d51-217">機能更新プログラムの一時停止が終了する日時</span><span class="sxs-lookup"><span data-stu-id="02d51-217">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="02d51-218">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="02d51-218">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="02d51-219">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="02d51-219">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="02d51-220">更新プログラムを受信するブランチデバイスを決定します。</span><span class="sxs-lookup"><span data-stu-id="02d51-220">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="02d51-221">使用可能な値: `userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="02d51-221">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="02d51-222">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="02d51-222">skipChecksBeforeRestart</span></span>|<span data-ttu-id="02d51-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d51-223">Boolean</span></span>|<span data-ttu-id="02d51-224">再起動前にすべてのチェックをスキップするように設定: バッテリーレベル = 40%、ユーザープレゼンス、表示が必要、プレゼンテーションモード、全画面表示モード、電話呼び出しの状態、ゲームモードなど。</span><span class="sxs-lookup"><span data-stu-id="02d51-224">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="02d51-225">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="02d51-225">updateWeeks</span></span>|[<span data-ttu-id="02d51-226">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="02d51-226">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="02d51-227">月の週に更新プログラムのインストールをスケジュールしました。</span><span class="sxs-lookup"><span data-stu-id="02d51-227">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="02d51-228">使用可能な値: `userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="02d51-228">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="02d51-229">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="02d51-229">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="02d51-230">日付</span><span class="sxs-lookup"><span data-stu-id="02d51-230">Date</span></span>|<span data-ttu-id="02d51-231">品質更新の一時停止の開始日。</span><span class="sxs-lookup"><span data-stu-id="02d51-231">Quality Updates Pause start date.</span></span> <span data-ttu-id="02d51-232">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="02d51-232">This property is read-only.</span></span>|
|<span data-ttu-id="02d51-233">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="02d51-233">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="02d51-234">日付</span><span class="sxs-lookup"><span data-stu-id="02d51-234">Date</span></span>|<span data-ttu-id="02d51-235">機能の更新の開始日が一時停止します。</span><span class="sxs-lookup"><span data-stu-id="02d51-235">Feature Updates Pause start date.</span></span> <span data-ttu-id="02d51-236">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="02d51-236">This property is read-only.</span></span>|
|<span data-ttu-id="02d51-237">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="02d51-237">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="02d51-238">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-238">Int32</span></span>|<span data-ttu-id="02d51-239">ロールバックが有効になっている機能更新後の日数</span><span class="sxs-lookup"><span data-stu-id="02d51-239">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="02d51-240">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="02d51-240">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="02d51-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d51-241">Boolean</span></span>|<span data-ttu-id="02d51-242">次のデバイスチェックで品質更新プログラムをロールバックするかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="02d51-242">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="02d51-243">Featureupdateswillberolledbackqualityupdatesrollbackstartdatetime</span><span class="sxs-lookup"><span data-stu-id="02d51-243">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="02d51-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="02d51-244">Boolean</span></span>|<span data-ttu-id="02d51-245">次回のデバイスチェックで機能の更新をロールバックするかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="02d51-245">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="02d51-246">追加</span><span class="sxs-lookup"><span data-stu-id="02d51-246">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="02d51-247">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d51-247">DateTimeOffset</span></span>|<span data-ttu-id="02d51-248">品質更新プログラムのロールバック開始日時</span><span class="sxs-lookup"><span data-stu-id="02d51-248">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="02d51-249">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="02d51-249">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="02d51-250">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d51-250">DateTimeOffset</span></span>|<span data-ttu-id="02d51-251">機能更新プログラムのロールバック開始日時</span><span class="sxs-lookup"><span data-stu-id="02d51-251">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="02d51-252">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="02d51-252">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="02d51-253">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-253">Int32</span></span>|<span data-ttu-id="02d51-254">アクティブ時間外に保留中の再起動を自動的にスケジュールして実行するまでの期限 (日数は2から30日)</span><span class="sxs-lookup"><span data-stu-id="02d51-254">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="02d51-255">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="02d51-255">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="02d51-256">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-256">Int32</span></span>|<span data-ttu-id="02d51-257">ユーザーが参加を再開できるリマインダー通知通知の有効期間が 1 ~ 3 日の場合に、再通知できる日数</span><span class="sxs-lookup"><span data-stu-id="02d51-257">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="02d51-258">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="02d51-258">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="02d51-259">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-259">Int32</span></span>|<span data-ttu-id="02d51-260">アクティブ時間外に再起動が行われるようにスケジュールされた自動再起動から移行するまでの日数。0から30日の範囲で有効な範囲で、ユーザーのスケジュールを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="02d51-260">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="02d51-261">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="02d51-261">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="02d51-262">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="02d51-262">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="02d51-263">自動再起動必須通知を閉じる方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="02d51-263">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="02d51-264">可能な値は、`notConfigured`、`automatic`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="02d51-264">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="02d51-265">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="02d51-265">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="02d51-266">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-266">Int32</span></span>|<span data-ttu-id="02d51-267">自動再起動警告リマインダー通知の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="02d51-267">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="02d51-268">サポートされている値: 2、4、8、12、または 24 (時間)。</span><span class="sxs-lookup"><span data-stu-id="02d51-268">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="02d51-269">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="02d51-269">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="02d51-270">Int32</span><span class="sxs-lookup"><span data-stu-id="02d51-270">Int32</span></span>|<span data-ttu-id="02d51-271">差し迫った自動再起動警告通知の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="02d51-271">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="02d51-272">サポートされている値:15、30または 60 (分)。</span><span class="sxs-lookup"><span data-stu-id="02d51-272">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="02d51-273">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="02d51-273">userPauseAccess</span></span>|[<span data-ttu-id="02d51-274">購入</span><span class="sxs-lookup"><span data-stu-id="02d51-274">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="02d51-275">エンドユーザーのアクセスを有効にして、ソフトウェアの更新を一時停止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="02d51-275">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="02d51-276">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="02d51-276">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="02d51-277">Userwindowsupの Canaccess</span><span class="sxs-lookup"><span data-stu-id="02d51-277">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="02d51-278">購入</span><span class="sxs-lookup"><span data-stu-id="02d51-278">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="02d51-279">Windows Update をスキャンするためにユーザーのアクセスを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="02d51-279">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="02d51-280">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="02d51-280">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="02d51-281">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="02d51-281">updateNotificationLevel</span></span>|[<span data-ttu-id="02d51-282">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="02d51-282">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="02d51-283">ユーザーに表示する Windows Update 通知を指定します。</span><span class="sxs-lookup"><span data-stu-id="02d51-283">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="02d51-284">可能な値は、`notConfigured`、`defaultNotifications`、`restartWarningsOnly`、`disableAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="02d51-284">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="02d51-285">応答</span><span class="sxs-lookup"><span data-stu-id="02d51-285">Response</span></span>
<span data-ttu-id="02d51-286">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="02d51-286">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02d51-287">例</span><span class="sxs-lookup"><span data-stu-id="02d51-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="02d51-288">要求</span><span class="sxs-lookup"><span data-stu-id="02d51-288">Request</span></span>
<span data-ttu-id="02d51-289">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02d51-289">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2676

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="02d51-290">応答</span><span class="sxs-lookup"><span data-stu-id="02d51-290">Response</span></span>
<span data-ttu-id="02d51-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02d51-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2848

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
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
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```





