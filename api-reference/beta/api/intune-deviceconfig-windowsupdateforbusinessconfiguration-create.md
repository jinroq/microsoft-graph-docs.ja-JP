---
title: Create windowsUpdateForBusinessConfiguration
description: 新しい windowsUpdateForBusinessConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e857437e78e647e6762ffa8914ffbc0efc011785
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171961"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="f3256-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3256-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="f3256-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3256-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3256-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3256-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3256-106">新しい [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f3256-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3256-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3256-107">Prerequisites</span></span>
<span data-ttu-id="f3256-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3256-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f3256-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3256-110">Permission type</span></span>|<span data-ttu-id="f3256-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3256-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3256-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3256-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3256-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3256-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3256-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3256-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3256-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3256-115">Not supported.</span></span>|
|<span data-ttu-id="f3256-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3256-116">Application</span></span>|<span data-ttu-id="f3256-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3256-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3256-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3256-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f3256-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3256-119">Request headers</span></span>
|<span data-ttu-id="f3256-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3256-120">Header</span></span>|<span data-ttu-id="f3256-121">値</span><span class="sxs-lookup"><span data-stu-id="f3256-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3256-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3256-122">Authorization</span></span>|<span data-ttu-id="f3256-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f3256-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3256-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f3256-124">Accept</span></span>|<span data-ttu-id="f3256-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3256-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3256-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3256-126">Request body</span></span>
<span data-ttu-id="f3256-127">要求本文で、windowsUpdateForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3256-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="f3256-128">次の表に、windowsUpdateForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3256-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="f3256-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3256-129">Property</span></span>|<span data-ttu-id="f3256-130">型</span><span class="sxs-lookup"><span data-stu-id="f3256-130">Type</span></span>|<span data-ttu-id="f3256-131">説明</span><span class="sxs-lookup"><span data-stu-id="f3256-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3256-132">id</span><span class="sxs-lookup"><span data-stu-id="f3256-132">id</span></span>|<span data-ttu-id="f3256-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f3256-133">String</span></span>|<span data-ttu-id="f3256-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f3256-134">Key of the entity.</span></span> <span data-ttu-id="f3256-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3256-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3256-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3256-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f3256-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3256-137">DateTimeOffset</span></span>|<span data-ttu-id="f3256-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f3256-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f3256-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3256-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3256-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3256-140">roleScopeTagIds</span></span>|<span data-ttu-id="f3256-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f3256-141">String collection</span></span>|<span data-ttu-id="f3256-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f3256-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f3256-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3256-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3256-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f3256-144">supportsScopeTags</span></span>|<span data-ttu-id="f3256-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="f3256-145">Boolean</span></span>|<span data-ttu-id="f3256-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3256-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f3256-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f3256-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f3256-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f3256-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f3256-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f3256-149">This property is read-only.</span></span> <span data-ttu-id="f3256-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3256-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3256-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3256-151">createdDateTime</span></span>|<span data-ttu-id="f3256-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3256-152">DateTimeOffset</span></span>|<span data-ttu-id="f3256-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f3256-153">DateTime the object was created.</span></span> <span data-ttu-id="f3256-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3256-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3256-155">説明</span><span class="sxs-lookup"><span data-stu-id="f3256-155">description</span></span>|<span data-ttu-id="f3256-156">String</span><span class="sxs-lookup"><span data-stu-id="f3256-156">String</span></span>|<span data-ttu-id="f3256-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f3256-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3256-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3256-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3256-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f3256-159">displayName</span></span>|<span data-ttu-id="f3256-160">String</span><span class="sxs-lookup"><span data-stu-id="f3256-160">String</span></span>|<span data-ttu-id="f3256-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f3256-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3256-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3256-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3256-163">version</span><span class="sxs-lookup"><span data-stu-id="f3256-163">version</span></span>|<span data-ttu-id="f3256-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-164">Int32</span></span>|<span data-ttu-id="f3256-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f3256-165">Version of the device configuration.</span></span> <span data-ttu-id="f3256-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3256-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3256-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f3256-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="f3256-168">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f3256-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="f3256-169">配信最適化モード。</span><span class="sxs-lookup"><span data-stu-id="f3256-169">Delivery Optimization Mode.</span></span> <span data-ttu-id="f3256-170">可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="f3256-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="f3256-171">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f3256-171">prereleaseFeatures</span></span>|[<span data-ttu-id="f3256-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f3256-172">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="f3256-173">プレリリース機能です。</span><span class="sxs-lookup"><span data-stu-id="f3256-173">The pre-release features.</span></span> <span data-ttu-id="f3256-174">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="f3256-174">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="f3256-175">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f3256-175">automaticUpdateMode</span></span>|[<span data-ttu-id="f3256-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f3256-176">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="f3256-177">自動更新モードです。</span><span class="sxs-lookup"><span data-stu-id="f3256-177">Automatic update mode.</span></span> <span data-ttu-id="f3256-178">可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`、`windowsDefault` です。</span><span class="sxs-lookup"><span data-stu-id="f3256-178">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="f3256-179">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="f3256-179">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="f3256-180">ブール値</span><span class="sxs-lookup"><span data-stu-id="f3256-180">Boolean</span></span>|<span data-ttu-id="f3256-181">Microsoft の更新サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="f3256-181">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="f3256-182">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="f3256-182">driversExcluded</span></span>|<span data-ttu-id="f3256-183">ブール値</span><span class="sxs-lookup"><span data-stu-id="f3256-183">Boolean</span></span>|<span data-ttu-id="f3256-184">Windows 更新ドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="f3256-184">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="f3256-185">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="f3256-185">installationSchedule</span></span>|[<span data-ttu-id="f3256-186">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="f3256-186">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="f3256-187">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="f3256-187">Installation schedule</span></span>|
|<span data-ttu-id="f3256-188">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f3256-188">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f3256-189">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-189">Int32</span></span>|<span data-ttu-id="f3256-190">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="f3256-190">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="f3256-191">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f3256-191">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f3256-192">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-192">Int32</span></span>|<span data-ttu-id="f3256-193">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="f3256-193">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="f3256-194">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f3256-194">qualityUpdatesPaused</span></span>|<span data-ttu-id="f3256-195">ブール値</span><span class="sxs-lookup"><span data-stu-id="f3256-195">Boolean</span></span>|<span data-ttu-id="f3256-196">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="f3256-196">Pause Quality Updates</span></span>|
|<span data-ttu-id="f3256-197">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f3256-197">featureUpdatesPaused</span></span>|<span data-ttu-id="f3256-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3256-198">Boolean</span></span>|<span data-ttu-id="f3256-199">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="f3256-199">Pause Feature Updates</span></span>|
|<span data-ttu-id="f3256-200">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f3256-200">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f3256-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3256-201">DateTimeOffset</span></span>|<span data-ttu-id="f3256-202">品質更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="f3256-202">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f3256-203">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f3256-203">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f3256-204">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3256-204">DateTimeOffset</span></span>|<span data-ttu-id="f3256-205">機能更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="f3256-205">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f3256-206">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="f3256-206">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="f3256-207">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="f3256-207">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="f3256-208">更新プログラムを受信するブランチデバイスを決定します。</span><span class="sxs-lookup"><span data-stu-id="f3256-208">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="f3256-209">使用可能な値: `userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="f3256-209">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="f3256-210">skipchecksbeforerestart</span><span class="sxs-lookup"><span data-stu-id="f3256-210">skipChecksBeforeRestart</span></span>|<span data-ttu-id="f3256-211">ブール値</span><span class="sxs-lookup"><span data-stu-id="f3256-211">Boolean</span></span>|<span data-ttu-id="f3256-212">再起動前にすべてのチェックをスキップするように設定: バッテリーレベル = 40%、ユーザープレゼンス、表示が必要、プレゼンテーションモード、全画面表示モード、電話呼び出しの状態、ゲームモードなど。</span><span class="sxs-lookup"><span data-stu-id="f3256-212">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="f3256-213">updateweeks</span><span class="sxs-lookup"><span data-stu-id="f3256-213">updateWeeks</span></span>|[<span data-ttu-id="f3256-214">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="f3256-214">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="f3256-215">月の週に更新プログラムのインストールをスケジュールしました。</span><span class="sxs-lookup"><span data-stu-id="f3256-215">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="f3256-216">使用可能な値: `userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="f3256-216">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="f3256-217">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="f3256-217">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="f3256-218">日付</span><span class="sxs-lookup"><span data-stu-id="f3256-218">Date</span></span>|<span data-ttu-id="f3256-219">品質更新の一時停止の開始日。</span><span class="sxs-lookup"><span data-stu-id="f3256-219">Quality Updates Pause start date.</span></span> <span data-ttu-id="f3256-220">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f3256-220">This property is read-only.</span></span>|
|<span data-ttu-id="f3256-221">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="f3256-221">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="f3256-222">日付</span><span class="sxs-lookup"><span data-stu-id="f3256-222">Date</span></span>|<span data-ttu-id="f3256-223">機能の更新の開始日が一時停止します。</span><span class="sxs-lookup"><span data-stu-id="f3256-223">Feature Updates Pause start date.</span></span> <span data-ttu-id="f3256-224">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f3256-224">This property is read-only.</span></span>|
|<span data-ttu-id="f3256-225">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="f3256-225">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="f3256-226">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-226">Int32</span></span>|<span data-ttu-id="f3256-227">ロールバックが有効になっている機能更新後の日数</span><span class="sxs-lookup"><span data-stu-id="f3256-227">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="f3256-228">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="f3256-228">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="f3256-229">ブール値</span><span class="sxs-lookup"><span data-stu-id="f3256-229">Boolean</span></span>|<span data-ttu-id="f3256-230">次のデバイスチェックで品質更新プログラムをロールバックするかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="f3256-230">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="f3256-231">featureupdateswillberolledbackqualityupdatesrollbackstartdatetime</span><span class="sxs-lookup"><span data-stu-id="f3256-231">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="f3256-232">ブール値</span><span class="sxs-lookup"><span data-stu-id="f3256-232">Boolean</span></span>|<span data-ttu-id="f3256-233">次回のデバイスチェックで機能の更新をロールバックするかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="f3256-233">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="f3256-234">追加</span><span class="sxs-lookup"><span data-stu-id="f3256-234">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="f3256-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3256-235">DateTimeOffset</span></span>|<span data-ttu-id="f3256-236">品質更新プログラムのロールバック開始日時</span><span class="sxs-lookup"><span data-stu-id="f3256-236">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="f3256-237">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="f3256-237">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="f3256-238">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3256-238">DateTimeOffset</span></span>|<span data-ttu-id="f3256-239">機能更新プログラムのロールバック開始日時</span><span class="sxs-lookup"><span data-stu-id="f3256-239">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="f3256-240">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="f3256-240">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="f3256-241">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-241">Int32</span></span>|<span data-ttu-id="f3256-242">アクティブ時間外に保留中の再起動を自動的にスケジュールして実行するまでの期限 (日数は2から30日)</span><span class="sxs-lookup"><span data-stu-id="f3256-242">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="f3256-243">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="f3256-243">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="f3256-244">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-244">Int32</span></span>|<span data-ttu-id="f3256-245">ユーザーが参加を再開できるリマインダー通知通知の有効期間が 1 ~ 3 日の場合に、再通知できる日数</span><span class="sxs-lookup"><span data-stu-id="f3256-245">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="f3256-246">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="f3256-246">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="f3256-247">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-247">Int32</span></span>|<span data-ttu-id="f3256-248">アクティブ時間外に再起動が行われるようにスケジュールされた自動再起動から移行するまでの日数。0から30日の範囲で有効な範囲で、ユーザーのスケジュールを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3256-248">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="f3256-249">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="f3256-249">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="f3256-250">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="f3256-250">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="f3256-251">自動再起動必須通知を閉じる方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3256-251">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="f3256-252">可能な値は `notConfigured`、`automatic`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="f3256-252">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="f3256-253">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="f3256-253">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="f3256-254">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-254">Int32</span></span>|<span data-ttu-id="f3256-255">自動再起動警告リマインダー通知の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3256-255">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="f3256-256">サポートされている値: 2、4、8、12、または 24 (時間)。</span><span class="sxs-lookup"><span data-stu-id="f3256-256">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="f3256-257">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="f3256-257">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="f3256-258">Int32</span><span class="sxs-lookup"><span data-stu-id="f3256-258">Int32</span></span>|<span data-ttu-id="f3256-259">差し迫った自動再起動警告通知の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3256-259">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="f3256-260">サポートされている値:15、30または 60 (分)。</span><span class="sxs-lookup"><span data-stu-id="f3256-260">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="f3256-261">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="f3256-261">userPauseAccess</span></span>|[<span data-ttu-id="f3256-262">購入</span><span class="sxs-lookup"><span data-stu-id="f3256-262">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f3256-263">エンドユーザーのアクセスを有効にして、ソフトウェアの更新を一時停止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3256-263">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="f3256-264">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f3256-264">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="f3256-265">応答</span><span class="sxs-lookup"><span data-stu-id="f3256-265">Response</span></span>
<span data-ttu-id="f3256-266">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3256-266">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3256-267">例</span><span class="sxs-lookup"><span data-stu-id="f3256-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3256-268">要求</span><span class="sxs-lookup"><span data-stu-id="f3256-268">Request</span></span>
<span data-ttu-id="f3256-269">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3256-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1804

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "userPauseAccess": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="f3256-270">応答</span><span class="sxs-lookup"><span data-stu-id="f3256-270">Response</span></span>
<span data-ttu-id="f3256-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3256-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1976

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "userPauseAccess": "enabled"
}
```




