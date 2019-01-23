---
title: Create windowsUpdateForBusinessConfiguration
description: 新しい windowsUpdateForBusinessConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dade72412a64b5703fa253eda0a40829f2475549
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406193"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="7d5e3-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d5e3-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="7d5e3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7d5e3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d5e3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d5e3-107">新しい [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-107">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d5e3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7d5e3-108">Prerequisites</span></span>
<span data-ttu-id="7d5e3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7d5e3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d5e3-111">Permission type</span></span>|<span data-ttu-id="7d5e3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d5e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d5e3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d5e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d5e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d5e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d5e3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d5e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d5e3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-116">Not supported.</span></span>|
|<span data-ttu-id="7d5e3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d5e3-117">Application</span></span>|<span data-ttu-id="7d5e3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d5e3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d5e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7d5e3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d5e3-120">Request headers</span></span>
|<span data-ttu-id="7d5e3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d5e3-121">Header</span></span>|<span data-ttu-id="7d5e3-122">値</span><span class="sxs-lookup"><span data-stu-id="7d5e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d5e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d5e3-123">Authorization</span></span>|<span data-ttu-id="7d5e3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d5e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d5e3-125">Accept</span></span>|<span data-ttu-id="7d5e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d5e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d5e3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d5e3-127">Request body</span></span>
<span data-ttu-id="7d5e3-128">要求本文で、windowsUpdateForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-128">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="7d5e3-129">次の表に、windowsUpdateForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-129">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="7d5e3-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d5e3-130">Property</span></span>|<span data-ttu-id="7d5e3-131">型</span><span class="sxs-lookup"><span data-stu-id="7d5e3-131">Type</span></span>|<span data-ttu-id="7d5e3-132">説明</span><span class="sxs-lookup"><span data-stu-id="7d5e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d5e3-133">id</span><span class="sxs-lookup"><span data-stu-id="7d5e3-133">id</span></span>|<span data-ttu-id="7d5e3-134">String</span><span class="sxs-lookup"><span data-stu-id="7d5e3-134">String</span></span>|<span data-ttu-id="7d5e3-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-135">Key of the entity.</span></span> <span data-ttu-id="7d5e3-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d5e3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d5e3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7d5e3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d5e3-138">DateTimeOffset</span></span>|<span data-ttu-id="7d5e3-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7d5e3-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d5e3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d5e3-141">roleScopeTagIds</span></span>|<span data-ttu-id="7d5e3-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7d5e3-142">String collection</span></span>|<span data-ttu-id="7d5e3-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d5e3-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d5e3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7d5e3-145">supportsScopeTags</span></span>|<span data-ttu-id="7d5e3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d5e3-146">Boolean</span></span>|<span data-ttu-id="7d5e3-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7d5e3-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7d5e3-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7d5e3-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-150">This property is read-only.</span></span> <span data-ttu-id="7d5e3-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d5e3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d5e3-152">createdDateTime</span></span>|<span data-ttu-id="7d5e3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d5e3-153">DateTimeOffset</span></span>|<span data-ttu-id="7d5e3-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-154">DateTime the object was created.</span></span> <span data-ttu-id="7d5e3-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d5e3-156">説明</span><span class="sxs-lookup"><span data-stu-id="7d5e3-156">description</span></span>|<span data-ttu-id="7d5e3-157">String</span><span class="sxs-lookup"><span data-stu-id="7d5e3-157">String</span></span>|<span data-ttu-id="7d5e3-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d5e3-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d5e3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7d5e3-160">displayName</span></span>|<span data-ttu-id="7d5e3-161">String</span><span class="sxs-lookup"><span data-stu-id="7d5e3-161">String</span></span>|<span data-ttu-id="7d5e3-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d5e3-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d5e3-164">version</span><span class="sxs-lookup"><span data-stu-id="7d5e3-164">version</span></span>|<span data-ttu-id="7d5e3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-165">Int32</span></span>|<span data-ttu-id="7d5e3-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-166">Version of the device configuration.</span></span> <span data-ttu-id="7d5e3-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d5e3-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="7d5e3-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="7d5e3-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="7d5e3-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="7d5e3-170">配信の最適化モードです。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-170">Delivery Optimization Mode.</span></span> <span data-ttu-id="7d5e3-171">可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="7d5e3-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="7d5e3-172">prereleaseFeatures</span></span>|[<span data-ttu-id="7d5e3-173">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="7d5e3-173">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="7d5e3-174">プレリリース機能です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-174">The pre-release features.</span></span> <span data-ttu-id="7d5e3-175">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-175">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="7d5e3-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="7d5e3-176">automaticUpdateMode</span></span>|[<span data-ttu-id="7d5e3-177">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="7d5e3-177">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="7d5e3-178">自動更新モードです。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-178">Automatic update mode.</span></span> <span data-ttu-id="7d5e3-179">可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`、`windowsDefault` です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-179">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="7d5e3-180">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="7d5e3-180">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="7d5e3-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d5e3-181">Boolean</span></span>|<span data-ttu-id="7d5e3-182">Microsoft の更新サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-182">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="7d5e3-183">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="7d5e3-183">driversExcluded</span></span>|<span data-ttu-id="7d5e3-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d5e3-184">Boolean</span></span>|<span data-ttu-id="7d5e3-185">Windows 更新ドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-185">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="7d5e3-186">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="7d5e3-186">installationSchedule</span></span>|[<span data-ttu-id="7d5e3-187">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="7d5e3-187">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="7d5e3-188">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="7d5e3-188">Installation schedule</span></span>|
|<span data-ttu-id="7d5e3-189">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="7d5e3-189">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="7d5e3-190">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-190">Int32</span></span>|<span data-ttu-id="7d5e3-191">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-191">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="7d5e3-192">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="7d5e3-192">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="7d5e3-193">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-193">Int32</span></span>|<span data-ttu-id="7d5e3-194">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-194">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="7d5e3-195">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="7d5e3-195">qualityUpdatesPaused</span></span>|<span data-ttu-id="7d5e3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d5e3-196">Boolean</span></span>|<span data-ttu-id="7d5e3-197">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-197">Pause Quality Updates</span></span>|
|<span data-ttu-id="7d5e3-198">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="7d5e3-198">featureUpdatesPaused</span></span>|<span data-ttu-id="7d5e3-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d5e3-199">Boolean</span></span>|<span data-ttu-id="7d5e3-200">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="7d5e3-200">Pause Feature Updates</span></span>|
|<span data-ttu-id="7d5e3-201">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="7d5e3-201">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="7d5e3-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d5e3-202">DateTimeOffset</span></span>|<span data-ttu-id="7d5e3-203">品質更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="7d5e3-203">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="7d5e3-204">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="7d5e3-204">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="7d5e3-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d5e3-205">DateTimeOffset</span></span>|<span data-ttu-id="7d5e3-206">機能更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="7d5e3-206">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="7d5e3-207">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="7d5e3-207">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="7d5e3-208">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="7d5e3-208">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="7d5e3-209">更新を受信できるの分岐デバイスを決定します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-209">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="7d5e3-210">使用可能な値: `userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-210">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="7d5e3-211">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="7d5e3-211">skipChecksBeforeRestart</span></span>|<span data-ttu-id="7d5e3-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d5e3-212">Boolean</span></span>|<span data-ttu-id="7d5e3-213">再起動する前にすべてのチェックをスキップする設定: バッテリ レベル = 40%、ユーザーのプレゼンス、プレゼンテーション モード、全画面表示モード、電話の呼び出しの状態、ゲームのモードなど、表示が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-213">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="7d5e3-214">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="7d5e3-214">updateWeeks</span></span>|[<span data-ttu-id="7d5e3-215">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="7d5e3-215">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="7d5e3-216">月の週に更新プログラムのインストールをスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-216">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="7d5e3-217">使用可能な値: `userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-217">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="7d5e3-218">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="7d5e3-218">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="7d5e3-219">日付</span><span class="sxs-lookup"><span data-stu-id="7d5e3-219">Date</span></span>|<span data-ttu-id="7d5e3-220">品質の更新プログラムの一時停止の開始日です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-220">Quality Updates Pause start date.</span></span> <span data-ttu-id="7d5e3-221">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-221">This property is read-only.</span></span>|
|<span data-ttu-id="7d5e3-222">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="7d5e3-222">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="7d5e3-223">日付</span><span class="sxs-lookup"><span data-stu-id="7d5e3-223">Date</span></span>|<span data-ttu-id="7d5e3-224">機能の更新の一時停止の開始日。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-224">Feature Updates Pause start date.</span></span> <span data-ttu-id="7d5e3-225">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-225">This property is read-only.</span></span>|
|<span data-ttu-id="7d5e3-226">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="7d5e3-226">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="7d5e3-227">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-227">Int32</span></span>|<span data-ttu-id="7d5e3-228">機能の更新プログラムのロールバックの有効期限後の日数</span><span class="sxs-lookup"><span data-stu-id="7d5e3-228">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="7d5e3-229">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="7d5e3-229">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="7d5e3-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d5e3-230">Boolean</span></span>|<span data-ttu-id="7d5e3-231">に次のデバイス上の品質の更新プログラムをチェック ロールバックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-231">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="7d5e3-232">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="7d5e3-232">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="7d5e3-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d5e3-233">Boolean</span></span>|<span data-ttu-id="7d5e3-234">に次のデバイスの機能の更新をチェックをロールバックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-234">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="7d5e3-235">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="7d5e3-235">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="7d5e3-236">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d5e3-236">DateTimeOffset</span></span>|<span data-ttu-id="7d5e3-237">品質の更新プログラムのロールバックの開始日時</span><span class="sxs-lookup"><span data-stu-id="7d5e3-237">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="7d5e3-238">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="7d5e3-238">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="7d5e3-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d5e3-239">DateTimeOffset</span></span>|<span data-ttu-id="7d5e3-240">機能の更新プログラムのロールバックの開始日時</span><span class="sxs-lookup"><span data-stu-id="7d5e3-240">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="7d5e3-241">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="7d5e3-241">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="7d5e3-242">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-242">Int32</span></span>|<span data-ttu-id="7d5e3-243">期限日に自動的にスケジュール設定とアクティブな時間で、2 から 30 日間の有効な範囲外で保留中の再起動を実行する前に</span><span class="sxs-lookup"><span data-stu-id="7d5e3-243">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="7d5e3-244">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="7d5e3-244">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="7d5e3-245">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-245">Int32</span></span>|<span data-ttu-id="7d5e3-246">ユーザーの有効な範囲は 1 から 3 日間での事前通知の関与を再起動できます再通知する日数です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-246">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="7d5e3-247">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="7d5e3-247">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="7d5e3-248">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-248">Int32</span></span>|<span data-ttu-id="7d5e3-249">自動再起動が掛かり状態を再起動する、ユーザーが有効な範囲は 0 から 30 日間で、スケジュールを必要とするアクティブな時間をスケジュールから移行するまでの日数</span><span class="sxs-lookup"><span data-stu-id="7d5e3-249">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="7d5e3-250">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="7d5e3-250">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="7d5e3-251">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="7d5e3-251">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="7d5e3-252">通知は消されますを自動的に再起動が必要するメソッドを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-252">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="7d5e3-253">可能な値は、`notConfigured`、`automatic`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-253">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="7d5e3-254">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="7d5e3-254">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="7d5e3-255">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-255">Int32</span></span>|<span data-ttu-id="7d5e3-256">自動再起動警告アラームの通知の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-256">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="7d5e3-257">サポートされる値: 2、4、8、12、または 24 (時間) です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-257">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="7d5e3-258">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="7d5e3-258">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="7d5e3-259">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5e3-259">Int32</span></span>|<span data-ttu-id="7d5e3-260">緊急の警告通知を自動的に再起動の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-260">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="7d5e3-261">サポートされる値: 15、30 または 60 (分) です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-261">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="7d5e3-262">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="7d5e3-262">userPauseAccess</span></span>|<span data-ttu-id="7d5e3-263">[有効化](../resources/intune-shared-enablement</span><span class="sxs-lookup"><span data-stu-id="7d5e3-263">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="7d5e3-264">.md)</span><span class="sxs-lookup"><span data-stu-id="7d5e3-264">.md)</span></span>|<span data-ttu-id="7d5e3-265">ソフトウェア更新を一時停止するのには、エンド ・ ユーザーのアクセスを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-265">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="7d5e3-266">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-266">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="7d5e3-267">応答</span><span class="sxs-lookup"><span data-stu-id="7d5e3-267">Response</span></span>
<span data-ttu-id="7d5e3-268">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-268">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d5e3-269">例</span><span class="sxs-lookup"><span data-stu-id="7d5e3-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d5e3-270">要求</span><span class="sxs-lookup"><span data-stu-id="7d5e3-270">Request</span></span>
<span data-ttu-id="7d5e3-271">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-271">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d5e3-272">応答</span><span class="sxs-lookup"><span data-stu-id="7d5e3-272">Response</span></span>
<span data-ttu-id="7d5e3-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




