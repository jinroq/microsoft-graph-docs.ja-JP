---
title: Create windowsUpdateForBusinessConfiguration
description: 新しい windowsUpdateForBusinessConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 4fa7cc29e439d4c160d752869ef2a877ef0a0e4a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315667"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="50656-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="50656-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="50656-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="50656-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50656-105">新しい [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="50656-105">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50656-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="50656-106">Prerequisites</span></span>
<span data-ttu-id="50656-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50656-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50656-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50656-109">Permission type</span></span>|<span data-ttu-id="50656-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="50656-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50656-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50656-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50656-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50656-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50656-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50656-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50656-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50656-114">Not supported.</span></span>|
|<span data-ttu-id="50656-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50656-115">Application</span></span>|<span data-ttu-id="50656-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50656-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50656-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50656-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="50656-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50656-118">Request headers</span></span>
|<span data-ttu-id="50656-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50656-119">Header</span></span>|<span data-ttu-id="50656-120">値</span><span class="sxs-lookup"><span data-stu-id="50656-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50656-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50656-121">Authorization</span></span>|<span data-ttu-id="50656-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="50656-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50656-123">Accept</span><span class="sxs-lookup"><span data-stu-id="50656-123">Accept</span></span>|<span data-ttu-id="50656-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50656-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50656-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="50656-125">Request body</span></span>
<span data-ttu-id="50656-126">要求本文で、windowsUpdateForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="50656-126">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="50656-127">次の表に、windowsUpdateForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="50656-127">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="50656-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50656-128">Property</span></span>|<span data-ttu-id="50656-129">種類</span><span class="sxs-lookup"><span data-stu-id="50656-129">Type</span></span>|<span data-ttu-id="50656-130">説明</span><span class="sxs-lookup"><span data-stu-id="50656-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50656-131">ID</span><span class="sxs-lookup"><span data-stu-id="50656-131">id</span></span>|<span data-ttu-id="50656-132">String</span><span class="sxs-lookup"><span data-stu-id="50656-132">String</span></span>|<span data-ttu-id="50656-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="50656-133">Key of the entity.</span></span> <span data-ttu-id="50656-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50656-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50656-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50656-135">lastModifiedDateTime</span></span>|<span data-ttu-id="50656-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50656-136">DateTimeOffset</span></span>|<span data-ttu-id="50656-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="50656-137">DateTime the object was last modified.</span></span> <span data-ttu-id="50656-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50656-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50656-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50656-139">createdDateTime</span></span>|<span data-ttu-id="50656-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50656-140">DateTimeOffset</span></span>|<span data-ttu-id="50656-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="50656-141">DateTime the object was created.</span></span> <span data-ttu-id="50656-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50656-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50656-143">説明</span><span class="sxs-lookup"><span data-stu-id="50656-143">description</span></span>|<span data-ttu-id="50656-144">String</span><span class="sxs-lookup"><span data-stu-id="50656-144">String</span></span>|<span data-ttu-id="50656-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="50656-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50656-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50656-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50656-147">displayName</span><span class="sxs-lookup"><span data-stu-id="50656-147">displayName</span></span>|<span data-ttu-id="50656-148">String</span><span class="sxs-lookup"><span data-stu-id="50656-148">String</span></span>|<span data-ttu-id="50656-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="50656-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50656-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50656-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50656-151">version</span><span class="sxs-lookup"><span data-stu-id="50656-151">version</span></span>|<span data-ttu-id="50656-152">Int32</span><span class="sxs-lookup"><span data-stu-id="50656-152">Int32</span></span>|<span data-ttu-id="50656-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="50656-153">Version of the device configuration.</span></span> <span data-ttu-id="50656-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50656-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50656-155">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="50656-155">deliveryOptimizationMode</span></span>|[<span data-ttu-id="50656-156">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="50656-156">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="50656-157">配信の最適化モードです。</span><span class="sxs-lookup"><span data-stu-id="50656-157">Delivery Optimization Mode.</span></span> <span data-ttu-id="50656-158">可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="50656-158">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="50656-159">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="50656-159">prereleaseFeatures</span></span>|[<span data-ttu-id="50656-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="50656-160">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="50656-161">プレリリース機能です。</span><span class="sxs-lookup"><span data-stu-id="50656-161">The pre-release features.</span></span> <span data-ttu-id="50656-162">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="50656-162">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="50656-163">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="50656-163">automaticUpdateMode</span></span>|[<span data-ttu-id="50656-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="50656-164">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="50656-165">自動更新モードです。</span><span class="sxs-lookup"><span data-stu-id="50656-165">Automatic update mode.</span></span> <span data-ttu-id="50656-166">可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` です。</span><span class="sxs-lookup"><span data-stu-id="50656-166">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="50656-167">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="50656-167">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="50656-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="50656-168">Boolean</span></span>|<span data-ttu-id="50656-169">Microsoft の更新サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="50656-169">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="50656-170">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="50656-170">driversExcluded</span></span>|<span data-ttu-id="50656-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="50656-171">Boolean</span></span>|<span data-ttu-id="50656-172">Windows 更新ドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="50656-172">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="50656-173">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="50656-173">installationSchedule</span></span>|[<span data-ttu-id="50656-174">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="50656-174">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="50656-175">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="50656-175">Installation schedule</span></span>|
|<span data-ttu-id="50656-176">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="50656-176">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="50656-177">Int32</span><span class="sxs-lookup"><span data-stu-id="50656-177">Int32</span></span>|<span data-ttu-id="50656-178">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="50656-178">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="50656-179">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="50656-179">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="50656-180">Int32</span><span class="sxs-lookup"><span data-stu-id="50656-180">Int32</span></span>|<span data-ttu-id="50656-181">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="50656-181">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="50656-182">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="50656-182">qualityUpdatesPaused</span></span>|<span data-ttu-id="50656-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="50656-183">Boolean</span></span>|<span data-ttu-id="50656-184">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="50656-184">Pause Quality Updates</span></span>|
|<span data-ttu-id="50656-185">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="50656-185">featureUpdatesPaused</span></span>|<span data-ttu-id="50656-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="50656-186">Boolean</span></span>|<span data-ttu-id="50656-187">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="50656-187">Pause Feature Updates</span></span>|
|<span data-ttu-id="50656-188">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="50656-188">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="50656-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50656-189">DateTimeOffset</span></span>|<span data-ttu-id="50656-190">品質更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="50656-190">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="50656-191">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="50656-191">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="50656-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50656-192">DateTimeOffset</span></span>|<span data-ttu-id="50656-193">機能更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="50656-193">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="50656-194">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="50656-194">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="50656-195">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="50656-195">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="50656-196">更新を受信できるの分岐デバイスを決定します。</span><span class="sxs-lookup"><span data-stu-id="50656-196">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="50656-197">使用可能な値: `userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="50656-197">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="50656-198">応答</span><span class="sxs-lookup"><span data-stu-id="50656-198">Response</span></span>
<span data-ttu-id="50656-199">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="50656-199">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50656-200">例</span><span class="sxs-lookup"><span data-stu-id="50656-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="50656-201">要求</span><span class="sxs-lookup"><span data-stu-id="50656-201">Request</span></span>
<span data-ttu-id="50656-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50656-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 910

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "businessReadyUpdatesOnly": "all"
}
```

### <a name="response"></a><span data-ttu-id="50656-203">応答</span><span class="sxs-lookup"><span data-stu-id="50656-203">Response</span></span>
<span data-ttu-id="50656-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="50656-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "businessReadyUpdatesOnly": "all"
}
```


