---
title: windowsUpdateForBusinessConfiguration の更新
description: windowsUpdateForBusinessConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c3295d3dd5eb703725c33bfa3ebaedeae2962481
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338197"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="f1e94-103">windowsUpdateForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="f1e94-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="f1e94-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1e94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1e94-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1e94-106">[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1e94-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f1e94-107">Prerequisites</span></span>
<span data-ttu-id="f1e94-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1e94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1e94-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1e94-110">Permission type</span></span>|<span data-ttu-id="f1e94-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1e94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1e94-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1e94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1e94-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1e94-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1e94-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1e94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1e94-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1e94-115">Not supported.</span></span>|
|<span data-ttu-id="f1e94-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1e94-116">Application</span></span>|<span data-ttu-id="f1e94-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1e94-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1e94-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1e94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1e94-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1e94-119">Request headers</span></span>
|<span data-ttu-id="f1e94-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1e94-120">Header</span></span>|<span data-ttu-id="f1e94-121">値</span><span class="sxs-lookup"><span data-stu-id="f1e94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1e94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1e94-122">Authorization</span></span>|<span data-ttu-id="f1e94-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1e94-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f1e94-124">Accept</span></span>|<span data-ttu-id="f1e94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1e94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1e94-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1e94-126">Request body</span></span>
<span data-ttu-id="f1e94-127">要求本文では、[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="f1e94-128">次の表に、[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="f1e94-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1e94-129">Property</span></span>|<span data-ttu-id="f1e94-130">型</span><span class="sxs-lookup"><span data-stu-id="f1e94-130">Type</span></span>|<span data-ttu-id="f1e94-131">説明</span><span class="sxs-lookup"><span data-stu-id="f1e94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1e94-132">id</span><span class="sxs-lookup"><span data-stu-id="f1e94-132">id</span></span>|<span data-ttu-id="f1e94-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f1e94-133">String</span></span>|<span data-ttu-id="f1e94-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f1e94-134">Key of the entity.</span></span> <span data-ttu-id="f1e94-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e94-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f1e94-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e94-137">DateTimeOffset</span></span>|<span data-ttu-id="f1e94-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f1e94-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f1e94-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1e94-140">roleScopeTagIds</span></span>|<span data-ttu-id="f1e94-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f1e94-141">String collection</span></span>|<span data-ttu-id="f1e94-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f1e94-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1e94-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1e94-144">supportsScopeTags</span></span>|<span data-ttu-id="f1e94-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-145">Boolean</span></span>|<span data-ttu-id="f1e94-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1e94-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f1e94-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1e94-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f1e94-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1e94-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-149">This property is read-only.</span></span> <span data-ttu-id="f1e94-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1e94-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f1e94-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1e94-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f1e94-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="f1e94-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f1e94-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1e94-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f1e94-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1e94-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f1e94-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f1e94-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f1e94-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f1e94-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f1e94-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f1e94-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f1e94-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f1e94-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f1e94-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e94-163">createdDateTime</span></span>|<span data-ttu-id="f1e94-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e94-164">DateTimeOffset</span></span>|<span data-ttu-id="f1e94-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f1e94-165">DateTime the object was created.</span></span> <span data-ttu-id="f1e94-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-167">description</span><span class="sxs-lookup"><span data-stu-id="f1e94-167">description</span></span>|<span data-ttu-id="f1e94-168">String</span><span class="sxs-lookup"><span data-stu-id="f1e94-168">String</span></span>|<span data-ttu-id="f1e94-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f1e94-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1e94-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f1e94-171">displayName</span></span>|<span data-ttu-id="f1e94-172">String</span><span class="sxs-lookup"><span data-stu-id="f1e94-172">String</span></span>|<span data-ttu-id="f1e94-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f1e94-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1e94-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-175">version</span><span class="sxs-lookup"><span data-stu-id="f1e94-175">version</span></span>|<span data-ttu-id="f1e94-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-176">Int32</span></span>|<span data-ttu-id="f1e94-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f1e94-177">Version of the device configuration.</span></span> <span data-ttu-id="f1e94-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1e94-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e94-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f1e94-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="f1e94-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f1e94-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="f1e94-181">配信最適化モード。</span><span class="sxs-lookup"><span data-stu-id="f1e94-181">Delivery Optimization Mode.</span></span> <span data-ttu-id="f1e94-182">可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="f1e94-183">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f1e94-183">prereleaseFeatures</span></span>|[<span data-ttu-id="f1e94-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f1e94-184">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="f1e94-185">プレリリース機能。</span><span class="sxs-lookup"><span data-stu-id="f1e94-185">The pre-release features.</span></span> <span data-ttu-id="f1e94-186">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-186">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="f1e94-187">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f1e94-187">automaticUpdateMode</span></span>|[<span data-ttu-id="f1e94-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f1e94-188">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="f1e94-189">自動更新モード。</span><span class="sxs-lookup"><span data-stu-id="f1e94-189">Automatic update mode.</span></span> <span data-ttu-id="f1e94-190">可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`、`windowsDefault` です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-190">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="f1e94-191">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="f1e94-191">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="f1e94-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-192">Boolean</span></span>|<span data-ttu-id="f1e94-193">Microsoft Update サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-193">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="f1e94-194">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="f1e94-194">driversExcluded</span></span>|<span data-ttu-id="f1e94-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-195">Boolean</span></span>|<span data-ttu-id="f1e94-196">Windows Update のドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-196">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="f1e94-197">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="f1e94-197">installationSchedule</span></span>|[<span data-ttu-id="f1e94-198">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="f1e94-198">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="f1e94-199">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="f1e94-199">Installation schedule</span></span>|
|<span data-ttu-id="f1e94-200">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-200">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f1e94-201">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-201">Int32</span></span>|<span data-ttu-id="f1e94-202">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="f1e94-202">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="f1e94-203">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-203">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f1e94-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-204">Int32</span></span>|<span data-ttu-id="f1e94-205">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="f1e94-205">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="f1e94-206">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f1e94-206">qualityUpdatesPaused</span></span>|<span data-ttu-id="f1e94-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-207">Boolean</span></span>|<span data-ttu-id="f1e94-208">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="f1e94-208">Pause Quality Updates</span></span>|
|<span data-ttu-id="f1e94-209">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f1e94-209">featureUpdatesPaused</span></span>|<span data-ttu-id="f1e94-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-210">Boolean</span></span>|<span data-ttu-id="f1e94-211">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="f1e94-211">Pause Feature Updates</span></span>|
|<span data-ttu-id="f1e94-212">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e94-212">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f1e94-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e94-213">DateTimeOffset</span></span>|<span data-ttu-id="f1e94-214">品質更新プログラムの一時停止が終了する日時</span><span class="sxs-lookup"><span data-stu-id="f1e94-214">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f1e94-215">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e94-215">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f1e94-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e94-216">DateTimeOffset</span></span>|<span data-ttu-id="f1e94-217">機能更新プログラムの一時停止が終了する日時</span><span class="sxs-lookup"><span data-stu-id="f1e94-217">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f1e94-218">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="f1e94-218">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="f1e94-219">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="f1e94-219">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="f1e94-220">更新プログラムを受信するブランチデバイスを決定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-220">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="f1e94-221">使用可能な値: `userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="f1e94-221">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="f1e94-222">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="f1e94-222">skipChecksBeforeRestart</span></span>|<span data-ttu-id="f1e94-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-223">Boolean</span></span>|<span data-ttu-id="f1e94-224">再起動前にすべてのチェックをスキップするように設定: バッテリーレベル = 40%、ユーザープレゼンス、表示が必要、プレゼンテーションモード、全画面表示モード、電話呼び出しの状態、ゲームモードなど。</span><span class="sxs-lookup"><span data-stu-id="f1e94-224">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="f1e94-225">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="f1e94-225">updateWeeks</span></span>|[<span data-ttu-id="f1e94-226">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="f1e94-226">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="f1e94-227">月の週に更新プログラムのインストールをスケジュールしました。</span><span class="sxs-lookup"><span data-stu-id="f1e94-227">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="f1e94-228">使用可能な値: `userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="f1e94-228">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="f1e94-229">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="f1e94-229">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="f1e94-230">日付</span><span class="sxs-lookup"><span data-stu-id="f1e94-230">Date</span></span>|<span data-ttu-id="f1e94-231">品質更新の一時停止の開始日。</span><span class="sxs-lookup"><span data-stu-id="f1e94-231">Quality Updates Pause start date.</span></span> <span data-ttu-id="f1e94-232">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-232">This property is read-only.</span></span>|
|<span data-ttu-id="f1e94-233">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="f1e94-233">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="f1e94-234">日付</span><span class="sxs-lookup"><span data-stu-id="f1e94-234">Date</span></span>|<span data-ttu-id="f1e94-235">機能の更新の開始日が一時停止します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-235">Feature Updates Pause start date.</span></span> <span data-ttu-id="f1e94-236">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-236">This property is read-only.</span></span>|
|<span data-ttu-id="f1e94-237">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-237">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="f1e94-238">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-238">Int32</span></span>|<span data-ttu-id="f1e94-239">ロールバックが有効になっている機能更新後の日数</span><span class="sxs-lookup"><span data-stu-id="f1e94-239">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="f1e94-240">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="f1e94-240">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="f1e94-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-241">Boolean</span></span>|<span data-ttu-id="f1e94-242">次のデバイスチェックで品質更新プログラムをロールバックするかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="f1e94-242">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="f1e94-243">Featureupdateswillberolledbackqualityupdatesrollbackstartdatetime</span><span class="sxs-lookup"><span data-stu-id="f1e94-243">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="f1e94-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-244">Boolean</span></span>|<span data-ttu-id="f1e94-245">次回のデバイスチェックで機能の更新をロールバックするかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="f1e94-245">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="f1e94-246">追加</span><span class="sxs-lookup"><span data-stu-id="f1e94-246">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="f1e94-247">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e94-247">DateTimeOffset</span></span>|<span data-ttu-id="f1e94-248">品質更新プログラムのロールバック開始日時</span><span class="sxs-lookup"><span data-stu-id="f1e94-248">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="f1e94-249">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e94-249">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="f1e94-250">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e94-250">DateTimeOffset</span></span>|<span data-ttu-id="f1e94-251">機能更新プログラムのロールバック開始日時</span><span class="sxs-lookup"><span data-stu-id="f1e94-251">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="f1e94-252">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-252">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="f1e94-253">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-253">Int32</span></span>|<span data-ttu-id="f1e94-254">アクティブ時間外に保留中の再起動を自動的にスケジュールして実行するまでの期限 (日数は2から30日)</span><span class="sxs-lookup"><span data-stu-id="f1e94-254">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="f1e94-255">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-255">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="f1e94-256">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-256">Int32</span></span>|<span data-ttu-id="f1e94-257">ユーザーが参加を再開できるリマインダー通知通知の有効期間が 1 ~ 3 日の場合に、再通知できる日数</span><span class="sxs-lookup"><span data-stu-id="f1e94-257">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="f1e94-258">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-258">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="f1e94-259">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-259">Int32</span></span>|<span data-ttu-id="f1e94-260">アクティブ時間外に再起動が行われるようにスケジュールされた自動再起動から移行するまでの日数。0から30日の範囲で有効な範囲で、ユーザーのスケジュールを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1e94-260">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="f1e94-261">deadlineForFeatureUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-261">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="f1e94-262">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-262">Int32</span></span>|<span data-ttu-id="f1e94-263">機能更新プログラムが自動的にインストールされるまでの日数は、2から30日の範囲内です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-263">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="f1e94-264">deadlineForQualityUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-264">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="f1e94-265">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-265">Int32</span></span>|<span data-ttu-id="f1e94-266">品質更新プログラムが自動的にインストールされるまでの日数は、2から30日の範囲内です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-266">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="f1e94-267">deadlineGracePeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f1e94-267">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="f1e94-268">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-268">Int32</span></span>|<span data-ttu-id="f1e94-269">有効範囲が0から7日に設定されると、再起動が自動的に実行されるまでの日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-269">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="f1e94-270">postponeRebootUntilAfterDeadline</span><span class="sxs-lookup"><span data-stu-id="f1e94-270">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="f1e94-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e94-271">Boolean</span></span>|<span data-ttu-id="f1e94-272">デバイスがアクティブ時間外の再起動の期限まで待機するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-272">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="f1e94-273">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="f1e94-273">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="f1e94-274">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="f1e94-274">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="f1e94-275">自動再起動必須通知を閉じる方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-275">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="f1e94-276">可能な値は、`notConfigured`、`automatic`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-276">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="f1e94-277">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="f1e94-277">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="f1e94-278">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-278">Int32</span></span>|<span data-ttu-id="f1e94-279">自動再起動警告リマインダー通知の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-279">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="f1e94-280">サポートされている値: 2、4、8、12、または 24 (時間)。</span><span class="sxs-lookup"><span data-stu-id="f1e94-280">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="f1e94-281">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="f1e94-281">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="f1e94-282">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e94-282">Int32</span></span>|<span data-ttu-id="f1e94-283">差し迫った自動再起動警告通知の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-283">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="f1e94-284">サポートされている値:15、30または 60 (分)。</span><span class="sxs-lookup"><span data-stu-id="f1e94-284">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="f1e94-285">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="f1e94-285">userPauseAccess</span></span>|[<span data-ttu-id="f1e94-286">購入</span><span class="sxs-lookup"><span data-stu-id="f1e94-286">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1e94-287">エンドユーザーのアクセスを有効にして、ソフトウェアの更新を一時停止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-287">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="f1e94-288">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-288">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1e94-289">Userwindowsupの Canaccess</span><span class="sxs-lookup"><span data-stu-id="f1e94-289">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="f1e94-290">購入</span><span class="sxs-lookup"><span data-stu-id="f1e94-290">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1e94-291">Windows Update をスキャンするためにユーザーのアクセスを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-291">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="f1e94-292">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-292">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1e94-293">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="f1e94-293">updateNotificationLevel</span></span>|[<span data-ttu-id="f1e94-294">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="f1e94-294">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="f1e94-295">ユーザーに表示する Windows Update 通知を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-295">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="f1e94-296">可能な値は、`notConfigured`、`defaultNotifications`、`restartWarningsOnly`、`disableAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-296">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="f1e94-297">応答</span><span class="sxs-lookup"><span data-stu-id="f1e94-297">Response</span></span>
<span data-ttu-id="f1e94-298">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f1e94-298">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1e94-299">例</span><span class="sxs-lookup"><span data-stu-id="f1e94-299">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1e94-300">要求</span><span class="sxs-lookup"><span data-stu-id="f1e94-300">Request</span></span>
<span data-ttu-id="f1e94-301">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1e94-301">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2840

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
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="f1e94-302">応答</span><span class="sxs-lookup"><span data-stu-id="f1e94-302">Response</span></span>
<span data-ttu-id="f1e94-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1e94-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3012

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
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```






