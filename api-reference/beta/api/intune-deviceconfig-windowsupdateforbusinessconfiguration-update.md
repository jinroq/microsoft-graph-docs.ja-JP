---
title: windowsUpdateForBusinessConfiguration の更新
description: windowsUpdateForBusinessConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: 5df5f1fdece80d502a12f196ee67db39eb81c5cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069748"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="d90a6-103">windowsUpdateForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d90a6-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="d90a6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d90a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d90a6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d90a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d90a6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d90a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d90a6-107">[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-107">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d90a6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d90a6-108">Prerequisites</span></span>
<span data-ttu-id="d90a6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d90a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d90a6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d90a6-111">Permission type</span></span>|<span data-ttu-id="d90a6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d90a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d90a6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d90a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d90a6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d90a6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d90a6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d90a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d90a6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d90a6-116">Not supported.</span></span>|
|<span data-ttu-id="d90a6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d90a6-117">Application</span></span>|<span data-ttu-id="d90a6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d90a6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d90a6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d90a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d90a6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d90a6-120">Request headers</span></span>
|<span data-ttu-id="d90a6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d90a6-121">Header</span></span>|<span data-ttu-id="d90a6-122">値</span><span class="sxs-lookup"><span data-stu-id="d90a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d90a6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d90a6-123">Authorization</span></span>|<span data-ttu-id="d90a6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d90a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d90a6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d90a6-125">Accept</span></span>|<span data-ttu-id="d90a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d90a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d90a6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d90a6-127">Request body</span></span>
<span data-ttu-id="d90a6-128">要求本文では、[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-128">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="d90a6-129">次の表に、[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-129">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="d90a6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d90a6-130">Property</span></span>|<span data-ttu-id="d90a6-131">型</span><span class="sxs-lookup"><span data-stu-id="d90a6-131">Type</span></span>|<span data-ttu-id="d90a6-132">説明</span><span class="sxs-lookup"><span data-stu-id="d90a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d90a6-133">id</span><span class="sxs-lookup"><span data-stu-id="d90a6-133">id</span></span>|<span data-ttu-id="d90a6-134">String</span><span class="sxs-lookup"><span data-stu-id="d90a6-134">String</span></span>|<span data-ttu-id="d90a6-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d90a6-135">Key of the entity.</span></span> <span data-ttu-id="d90a6-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d90a6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d90a6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d90a6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d90a6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90a6-138">DateTimeOffset</span></span>|<span data-ttu-id="d90a6-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d90a6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d90a6-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d90a6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d90a6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d90a6-141">roleScopeTagIds</span></span>|<span data-ttu-id="d90a6-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d90a6-142">String collection</span></span>|<span data-ttu-id="d90a6-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="d90a6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d90a6-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d90a6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d90a6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d90a6-145">supportsScopeTags</span></span>|<span data-ttu-id="d90a6-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="d90a6-146">Boolean</span></span>|<span data-ttu-id="d90a6-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d90a6-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="d90a6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d90a6-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="d90a6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d90a6-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-150">This property is read-only.</span></span> <span data-ttu-id="d90a6-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d90a6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d90a6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d90a6-152">createdDateTime</span></span>|<span data-ttu-id="d90a6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90a6-153">DateTimeOffset</span></span>|<span data-ttu-id="d90a6-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d90a6-154">DateTime the object was created.</span></span> <span data-ttu-id="d90a6-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d90a6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d90a6-156">説明</span><span class="sxs-lookup"><span data-stu-id="d90a6-156">description</span></span>|<span data-ttu-id="d90a6-157">String</span><span class="sxs-lookup"><span data-stu-id="d90a6-157">String</span></span>|<span data-ttu-id="d90a6-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d90a6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d90a6-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d90a6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d90a6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d90a6-160">displayName</span></span>|<span data-ttu-id="d90a6-161">String</span><span class="sxs-lookup"><span data-stu-id="d90a6-161">String</span></span>|<span data-ttu-id="d90a6-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d90a6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d90a6-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d90a6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d90a6-164">version</span><span class="sxs-lookup"><span data-stu-id="d90a6-164">version</span></span>|<span data-ttu-id="d90a6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-165">Int32</span></span>|<span data-ttu-id="d90a6-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d90a6-166">Version of the device configuration.</span></span> <span data-ttu-id="d90a6-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d90a6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d90a6-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="d90a6-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="d90a6-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="d90a6-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="d90a6-170">配信の最適化モードです。</span><span class="sxs-lookup"><span data-stu-id="d90a6-170">Delivery Optimization Mode.</span></span> <span data-ttu-id="d90a6-171">可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="d90a6-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="d90a6-172">prereleaseFeatures</span></span>|[<span data-ttu-id="d90a6-173">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="d90a6-173">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="d90a6-174">プレリリース機能です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-174">The pre-release features.</span></span> <span data-ttu-id="d90a6-175">可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-175">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="d90a6-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="d90a6-176">automaticUpdateMode</span></span>|[<span data-ttu-id="d90a6-177">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="d90a6-177">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="d90a6-178">自動更新モードです。</span><span class="sxs-lookup"><span data-stu-id="d90a6-178">Automatic update mode.</span></span> <span data-ttu-id="d90a6-179">可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-179">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="d90a6-180">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="d90a6-180">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="d90a6-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d90a6-181">Boolean</span></span>|<span data-ttu-id="d90a6-182">Microsoft の更新サービスを許可します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-182">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="d90a6-183">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="d90a6-183">driversExcluded</span></span>|<span data-ttu-id="d90a6-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="d90a6-184">Boolean</span></span>|<span data-ttu-id="d90a6-185">Windows 更新ドライバーを除外します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-185">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="d90a6-186">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="d90a6-186">installationSchedule</span></span>|[<span data-ttu-id="d90a6-187">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="d90a6-187">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="d90a6-188">インストールのスケジュールです</span><span class="sxs-lookup"><span data-stu-id="d90a6-188">Installation schedule</span></span>|
|<span data-ttu-id="d90a6-189">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="d90a6-189">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="d90a6-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-190">Int32</span></span>|<span data-ttu-id="d90a6-191">品質更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="d90a6-191">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="d90a6-192">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="d90a6-192">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="d90a6-193">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-193">Int32</span></span>|<span data-ttu-id="d90a6-194">機能更新プログラムの実行をこの日数分延期します</span><span class="sxs-lookup"><span data-stu-id="d90a6-194">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="d90a6-195">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="d90a6-195">qualityUpdatesPaused</span></span>|<span data-ttu-id="d90a6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d90a6-196">Boolean</span></span>|<span data-ttu-id="d90a6-197">品質更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="d90a6-197">Pause Quality Updates</span></span>|
|<span data-ttu-id="d90a6-198">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="d90a6-198">featureUpdatesPaused</span></span>|<span data-ttu-id="d90a6-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d90a6-199">Boolean</span></span>|<span data-ttu-id="d90a6-200">機能更新プログラムの実行を一時停止します</span><span class="sxs-lookup"><span data-stu-id="d90a6-200">Pause Feature Updates</span></span>|
|<span data-ttu-id="d90a6-201">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="d90a6-201">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="d90a6-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90a6-202">DateTimeOffset</span></span>|<span data-ttu-id="d90a6-203">品質更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="d90a6-203">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="d90a6-204">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="d90a6-204">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="d90a6-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90a6-205">DateTimeOffset</span></span>|<span data-ttu-id="d90a6-206">機能更新プログラム実行一時停止の有効期限が切れる日時です</span><span class="sxs-lookup"><span data-stu-id="d90a6-206">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="d90a6-207">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="d90a6-207">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="d90a6-208">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="d90a6-208">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="d90a6-209">更新を受信できるの分岐デバイスを決定します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-209">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="d90a6-210">使用可能な値: `userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="d90a6-210">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="d90a6-211">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="d90a6-211">skipChecksBeforeRestart</span></span>|<span data-ttu-id="d90a6-212">ブール値</span><span class="sxs-lookup"><span data-stu-id="d90a6-212">Boolean</span></span>|<span data-ttu-id="d90a6-213">再起動する前にすべてのチェックをスキップする設定: バッテリ レベル = 40%、ユーザーのプレゼンス、プレゼンテーション モード、全画面表示モード、電話の呼び出しの状態、ゲームのモードなど、表示が必要です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-213">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="d90a6-214">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="d90a6-214">updateWeeks</span></span>|[<span data-ttu-id="d90a6-215">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="d90a6-215">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="d90a6-216">月の週に更新プログラムのインストールをスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="d90a6-216">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="d90a6-217">使用可能な値: `userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="d90a6-217">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="d90a6-218">qualityUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d90a6-218">qualityUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="d90a6-219">String</span><span class="sxs-lookup"><span data-stu-id="d90a6-219">String</span></span>|<span data-ttu-id="d90a6-220">品質の更新プログラムの一時停止の開始日時</span><span class="sxs-lookup"><span data-stu-id="d90a6-220">Quality Updates Pause Start datetime</span></span>|
|<span data-ttu-id="d90a6-221">featureUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d90a6-221">featureUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="d90a6-222">String</span><span class="sxs-lookup"><span data-stu-id="d90a6-222">String</span></span>|<span data-ttu-id="d90a6-223">機能の更新の一時停止の開始日時</span><span class="sxs-lookup"><span data-stu-id="d90a6-223">Feature Updates Pause Start datetime</span></span>|
|<span data-ttu-id="d90a6-224">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="d90a6-224">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="d90a6-225">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-225">Int32</span></span>|<span data-ttu-id="d90a6-226">機能の更新プログラムのロールバックの有効期限後の日数</span><span class="sxs-lookup"><span data-stu-id="d90a6-226">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="d90a6-227">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="d90a6-227">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="d90a6-228">ブール値</span><span class="sxs-lookup"><span data-stu-id="d90a6-228">Boolean</span></span>|<span data-ttu-id="d90a6-229">に次のデバイス上の品質の更新プログラムをチェック ロールバックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-229">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="d90a6-230">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="d90a6-230">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="d90a6-231">ブール値</span><span class="sxs-lookup"><span data-stu-id="d90a6-231">Boolean</span></span>|<span data-ttu-id="d90a6-232">に次のデバイスの機能の更新をチェックをロールバックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-232">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="d90a6-233">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d90a6-233">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="d90a6-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90a6-234">DateTimeOffset</span></span>|<span data-ttu-id="d90a6-235">品質の更新プログラムのロールバックの開始日時</span><span class="sxs-lookup"><span data-stu-id="d90a6-235">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="d90a6-236">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d90a6-236">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="d90a6-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90a6-237">DateTimeOffset</span></span>|<span data-ttu-id="d90a6-238">機能の更新プログラムのロールバックの開始日時</span><span class="sxs-lookup"><span data-stu-id="d90a6-238">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="d90a6-239">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="d90a6-239">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="d90a6-240">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-240">Int32</span></span>|<span data-ttu-id="d90a6-241">期限日に自動的にスケジュール設定とアクティブな時間で、2 から 30 日間の有効な範囲外で保留中の再起動を実行する前に</span><span class="sxs-lookup"><span data-stu-id="d90a6-241">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="d90a6-242">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="d90a6-242">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="d90a6-243">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-243">Int32</span></span>|<span data-ttu-id="d90a6-244">ユーザーの有効な範囲は 1 から 3 日間での事前通知の関与を再起動できます再通知する日数です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-244">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="d90a6-245">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="d90a6-245">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="d90a6-246">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-246">Int32</span></span>|<span data-ttu-id="d90a6-247">自動再起動が掛かり状態を再起動する、ユーザーが有効な範囲は 0 から 30 日間で、スケジュールを必要とするアクティブな時間をスケジュールから移行するまでの日数</span><span class="sxs-lookup"><span data-stu-id="d90a6-247">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="d90a6-248">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="d90a6-248">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="d90a6-249">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="d90a6-249">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="d90a6-250">通知は消されますを自動的に再起動が必要するメソッドを指定します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-250">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="d90a6-251">可能な値は、`notConfigured`、`automatic`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-251">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="d90a6-252">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="d90a6-252">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="d90a6-253">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-253">Int32</span></span>|<span data-ttu-id="d90a6-254">自動再起動警告アラームの通知の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-254">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="d90a6-255">サポートされる値: 2、4、8、12、または 24 (時間) です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-255">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="d90a6-256">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="d90a6-256">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="d90a6-257">Int32</span><span class="sxs-lookup"><span data-stu-id="d90a6-257">Int32</span></span>|<span data-ttu-id="d90a6-258">緊急の警告通知を自動的に再起動の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-258">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="d90a6-259">サポートされる値: 15、30 または 60 (分) です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-259">Supported values: 15, 30 or 60 (minutes).</span></span>|



## <a name="response"></a><span data-ttu-id="d90a6-260">応答</span><span class="sxs-lookup"><span data-stu-id="d90a6-260">Response</span></span>
<span data-ttu-id="d90a6-261">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d90a6-261">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d90a6-262">例</span><span class="sxs-lookup"><span data-stu-id="d90a6-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="d90a6-263">要求</span><span class="sxs-lookup"><span data-stu-id="d90a6-263">Request</span></span>
<span data-ttu-id="d90a6-264">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d90a6-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1787

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
  "scheduleImminentRestartWarningInMinutes": 7
}
```

### <a name="response"></a><span data-ttu-id="d90a6-265">応答</span><span class="sxs-lookup"><span data-stu-id="d90a6-265">Response</span></span>
<span data-ttu-id="d90a6-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d90a6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1971

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
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
  "scheduleImminentRestartWarningInMinutes": 7
}
```





