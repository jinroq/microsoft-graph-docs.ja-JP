---
title: androiddeviceowner一般の devic/デバイスの更新
description: androiddeviceownerのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fad142a5ec0f069c40185a40865e29ddee894789
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32480472"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="1748a-103">androiddeviceowner一般の devic/デバイスの更新</span><span class="sxs-lookup"><span data-stu-id="1748a-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1748a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1748a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1748a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1748a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1748a-106">[androiddeviceownerの](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1748a-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1748a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1748a-107">Prerequisites</span></span>
<span data-ttu-id="1748a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1748a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1748a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1748a-110">Permission type</span></span>|<span data-ttu-id="1748a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1748a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1748a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1748a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1748a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1748a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1748a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1748a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1748a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1748a-115">Not supported.</span></span>|
|<span data-ttu-id="1748a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1748a-116">Application</span></span>|<span data-ttu-id="1748a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1748a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1748a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1748a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1748a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1748a-119">Request headers</span></span>
|<span data-ttu-id="1748a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1748a-120">Header</span></span>|<span data-ttu-id="1748a-121">値</span><span class="sxs-lookup"><span data-stu-id="1748a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1748a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1748a-122">Authorization</span></span>|<span data-ttu-id="1748a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1748a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1748a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1748a-124">Accept</span></span>|<span data-ttu-id="1748a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1748a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1748a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1748a-126">Request body</span></span>
<span data-ttu-id="1748a-127">要求本文で、 [androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devic/devicオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1748a-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="1748a-128">次の表に、 [androiddeviceowner[devic]](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="1748a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1748a-129">Property</span></span>|<span data-ttu-id="1748a-130">型</span><span class="sxs-lookup"><span data-stu-id="1748a-130">Type</span></span>|<span data-ttu-id="1748a-131">説明</span><span class="sxs-lookup"><span data-stu-id="1748a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1748a-132">id</span><span class="sxs-lookup"><span data-stu-id="1748a-132">id</span></span>|<span data-ttu-id="1748a-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1748a-133">String</span></span>|<span data-ttu-id="1748a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1748a-134">Key of the entity.</span></span> <span data-ttu-id="1748a-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1748a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1748a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1748a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1748a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1748a-137">DateTimeOffset</span></span>|<span data-ttu-id="1748a-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1748a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1748a-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1748a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1748a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1748a-140">roleScopeTagIds</span></span>|<span data-ttu-id="1748a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1748a-141">String collection</span></span>|<span data-ttu-id="1748a-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="1748a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1748a-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1748a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1748a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1748a-144">supportsScopeTags</span></span>|<span data-ttu-id="1748a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-145">Boolean</span></span>|<span data-ttu-id="1748a-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1748a-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="1748a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1748a-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="1748a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1748a-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="1748a-149">This property is read-only.</span></span> <span data-ttu-id="1748a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1748a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1748a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1748a-151">createdDateTime</span></span>|<span data-ttu-id="1748a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1748a-152">DateTimeOffset</span></span>|<span data-ttu-id="1748a-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1748a-153">DateTime the object was created.</span></span> <span data-ttu-id="1748a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1748a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1748a-155">説明</span><span class="sxs-lookup"><span data-stu-id="1748a-155">description</span></span>|<span data-ttu-id="1748a-156">String</span><span class="sxs-lookup"><span data-stu-id="1748a-156">String</span></span>|<span data-ttu-id="1748a-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="1748a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1748a-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1748a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1748a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1748a-159">displayName</span></span>|<span data-ttu-id="1748a-160">String</span><span class="sxs-lookup"><span data-stu-id="1748a-160">String</span></span>|<span data-ttu-id="1748a-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="1748a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1748a-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1748a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1748a-163">version</span><span class="sxs-lookup"><span data-stu-id="1748a-163">version</span></span>|<span data-ttu-id="1748a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-164">Int32</span></span>|<span data-ttu-id="1748a-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1748a-165">Version of the device configuration.</span></span> <span data-ttu-id="1748a-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1748a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1748a-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="1748a-167">accountsBlockModification</span></span>|<span data-ttu-id="1748a-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-168">Boolean</span></span>|<span data-ttu-id="1748a-169">アカウントの追加または削除が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="1748a-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1748a-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="1748a-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-171">Boolean</span></span>|<span data-ttu-id="1748a-172">ユーザーが不明なソースを有効にできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="1748a-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="1748a-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="1748a-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="1748a-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="1748a-175">アプリの自動更新ポリシーの値を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="1748a-176">可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。</span><span class="sxs-lookup"><span data-stu-id="1748a-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="1748a-177">appsdefaultpermissionpolicy</span><span class="sxs-lookup"><span data-stu-id="1748a-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="1748a-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="1748a-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="1748a-179">アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="1748a-180">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="1748a-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="1748a-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="1748a-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="1748a-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-182">Boolean</span></span>|<span data-ttu-id="1748a-183">すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1748a-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="1748a-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="1748a-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="1748a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-185">Boolean</span></span>|<span data-ttu-id="1748a-186">ユーザーが bluetooth を構成することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="1748a-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="1748a-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="1748a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-188">Boolean</span></span>|<span data-ttu-id="1748a-189">ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="1748a-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1748a-190">cameraBlocked</span></span>|<span data-ttu-id="1748a-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-191">Boolean</span></span>|<span data-ttu-id="1748a-192">カメラの使用を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="1748a-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="1748a-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="1748a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-194">Boolean</span></span>|<span data-ttu-id="1748a-195">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="1748a-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="1748a-196">dataRoamingBlocked</span></span>|<span data-ttu-id="1748a-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-197">Boolean</span></span>|<span data-ttu-id="1748a-198">ユーザーのデータ移動を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="1748a-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="1748a-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="1748a-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-200">Boolean</span></span>|<span data-ttu-id="1748a-201">ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="1748a-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="1748a-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="1748a-203">String collection</span><span class="sxs-lookup"><span data-stu-id="1748a-203">String collection</span></span>|<span data-ttu-id="1748a-204">デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。</span><span class="sxs-lookup"><span data-stu-id="1748a-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="1748a-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="1748a-205">factoryResetBlocked</span></span>|<span data-ttu-id="1748a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-206">Boolean</span></span>|<span data-ttu-id="1748a-207">設定の出荷時のリセットオプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="1748a-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="1748a-208">kioskModeApps</span></span>|<span data-ttu-id="1748a-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1748a-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1748a-210">デバイスがキオスクモードのときに表示される管理対象アプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="1748a-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="1748a-211">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1748a-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1748a-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="1748a-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="1748a-213">String</span><span class="sxs-lookup"><span data-stu-id="1748a-213">String</span></span>|<span data-ttu-id="1748a-214">デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。</span><span class="sxs-lookup"><span data-stu-id="1748a-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1748a-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="1748a-215">kioskModeExitCode</span></span>|<span data-ttu-id="1748a-216">String</span><span class="sxs-lookup"><span data-stu-id="1748a-216">String</span></span>|<span data-ttu-id="1748a-217">デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。</span><span class="sxs-lookup"><span data-stu-id="1748a-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1748a-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="1748a-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="1748a-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-219">Boolean</span></span>|<span data-ttu-id="1748a-220">デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1748a-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1748a-221">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="1748a-221">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="1748a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-222">Boolean</span></span>|<span data-ttu-id="1748a-223">ユーザーがキオスクモードで Bluetooth 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1748a-223">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="1748a-224">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="1748a-224">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="1748a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-225">Boolean</span></span>|<span data-ttu-id="1748a-226">ユーザーがキオスクモードで wi-fi 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1748a-226">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="1748a-227">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="1748a-227">microphoneForceMute</span></span>|<span data-ttu-id="1748a-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-228">Boolean</span></span>|<span data-ttu-id="1748a-229">デバイス上でのマイクのミュートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-229">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="1748a-230">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="1748a-230">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="1748a-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-231">Boolean</span></span>|<span data-ttu-id="1748a-232">ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-232">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="1748a-233">nfcblockoutgoingbeam</span><span class="sxs-lookup"><span data-stu-id="1748a-233">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="1748a-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-234">Boolean</span></span>|<span data-ttu-id="1748a-235">NFC の送信ビームをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-235">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="1748a-236">passwordblockkeyguard</span><span class="sxs-lookup"><span data-stu-id="1748a-236">passwordBlockKeyguard</span></span>|<span data-ttu-id="1748a-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-237">Boolean</span></span>|<span data-ttu-id="1748a-238">keyguard が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-238">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="1748a-239">passwordblockkeygu/機能</span><span class="sxs-lookup"><span data-stu-id="1748a-239">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="1748a-240">[androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1748a-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="1748a-241">ブロックする device keyguard 機能のリストです。</span><span class="sxs-lookup"><span data-stu-id="1748a-241">List of device keyguard features to block.</span></span> <span data-ttu-id="1748a-242">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1748a-242">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="1748a-243">可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。</span><span class="sxs-lookup"><span data-stu-id="1748a-243">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="1748a-244">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1748a-244">passwordExpirationDays</span></span>|<span data-ttu-id="1748a-245">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-245">Int32</span></span>|<span data-ttu-id="1748a-246">パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1748a-246">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="1748a-247">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="1748a-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1748a-248">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1748a-248">passwordMinimumLength</span></span>|<span data-ttu-id="1748a-249">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-249">Int32</span></span>|<span data-ttu-id="1748a-250">デバイスで必要なパスワードの最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-250">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="1748a-251">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="1748a-251">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1748a-252">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1748a-252">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="1748a-253">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-253">Int32</span></span>|<span data-ttu-id="1748a-254">デバイスパスワードに必要な文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-254">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="1748a-255">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="1748a-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1748a-256">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1748a-256">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="1748a-257">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-257">Int32</span></span>|<span data-ttu-id="1748a-258">デバイスパスワードに必要な小文字の最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-258">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="1748a-259">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="1748a-259">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1748a-260">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1748a-260">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="1748a-261">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-261">Int32</span></span>|<span data-ttu-id="1748a-262">デバイスパスワードに必要な文字以外の文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-262">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="1748a-263">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="1748a-263">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1748a-264">passwordminimumnumericcharacters</span><span class="sxs-lookup"><span data-stu-id="1748a-264">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="1748a-265">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-265">Int32</span></span>|<span data-ttu-id="1748a-266">デバイスパスワードに必要な最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-266">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="1748a-267">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="1748a-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1748a-268">passwordminimumシンボル文字</span><span class="sxs-lookup"><span data-stu-id="1748a-268">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="1748a-269">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-269">Int32</span></span>|<span data-ttu-id="1748a-270">デバイスパスワードに必要な最小記号文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-270">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="1748a-271">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="1748a-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1748a-272">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1748a-272">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="1748a-273">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-273">Int32</span></span>|<span data-ttu-id="1748a-274">デバイスのパスワードに必要な上位 caseletter 文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-274">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="1748a-275">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="1748a-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1748a-276">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1748a-276">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1748a-277">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-277">Int32</span></span>|<span data-ttu-id="1748a-278">画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。</span><span class="sxs-lookup"><span data-stu-id="1748a-278">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1748a-279">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="1748a-279">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="1748a-280">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-280">Int32</span></span>|<span data-ttu-id="1748a-281">パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。</span><span class="sxs-lookup"><span data-stu-id="1748a-281">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="1748a-282">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="1748a-282">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1748a-283">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1748a-283">passwordRequiredType</span></span>|[<span data-ttu-id="1748a-284">androiddeviceownerrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="1748a-284">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="1748a-285">デバイスで必要なパスワードの最小品質を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-285">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="1748a-286">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。</span><span class="sxs-lookup"><span data-stu-id="1748a-286">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="1748a-287">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1748a-287">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1748a-288">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-288">Int32</span></span>|<span data-ttu-id="1748a-289">ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-289">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="1748a-290">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="1748a-290">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1748a-291">playstoremode</span><span class="sxs-lookup"><span data-stu-id="1748a-291">playStoreMode</span></span>|[<span data-ttu-id="1748a-292">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="1748a-292">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="1748a-293">デバイスの再生ストアモードを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-293">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="1748a-294">使用可能な値は、`notConfigured`、`allowList`、`blockList` です。</span><span class="sxs-lookup"><span data-stu-id="1748a-294">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="1748a-295">safebootblocked</span><span class="sxs-lookup"><span data-stu-id="1748a-295">safeBootBlocked</span></span>|<span data-ttu-id="1748a-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-296">Boolean</span></span>|<span data-ttu-id="1748a-297">セーフブートでのデバイスの再起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-297">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="1748a-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1748a-298">screenCaptureBlocked</span></span>|<span data-ttu-id="1748a-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-299">Boolean</span></span>|<span data-ttu-id="1748a-300">スクリーンショットを撮影する機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-300">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="1748a-301">securityallowデバッグ機能</span><span class="sxs-lookup"><span data-stu-id="1748a-301">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="1748a-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-302">Boolean</span></span>|<span data-ttu-id="1748a-303">ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-303">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="1748a-304">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1748a-304">securityRequireVerifyApps</span></span>|<span data-ttu-id="1748a-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-305">Boolean</span></span>|<span data-ttu-id="1748a-306">アプリを確認する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-306">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="1748a-307">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="1748a-307">statusBarBlocked</span></span>|<span data-ttu-id="1748a-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-308">Boolean</span></span>|<span data-ttu-id="1748a-309">通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-309">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="1748a-310">stayonmodes</span><span class="sxs-lookup"><span data-stu-id="1748a-310">stayOnModes</span></span>|<span data-ttu-id="1748a-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1748a-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="1748a-312">デバイスの表示がオンのままになるモードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="1748a-312">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="1748a-313">このコレクションには、最大4つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1748a-313">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="1748a-314">可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。</span><span class="sxs-lookup"><span data-stu-id="1748a-314">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="1748a-315">storageallowusb</span><span class="sxs-lookup"><span data-stu-id="1748a-315">storageAllowUsb</span></span>|<span data-ttu-id="1748a-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-316">Boolean</span></span>|<span data-ttu-id="1748a-317">USB 大容量ストレージを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-317">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="1748a-318">storageblockexternalmedia</span><span class="sxs-lookup"><span data-stu-id="1748a-318">storageBlockExternalMedia</span></span>|<span data-ttu-id="1748a-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-319">Boolean</span></span>|<span data-ttu-id="1748a-320">外部メディアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-320">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="1748a-321">storageblockusbfiletransfer</span><span class="sxs-lookup"><span data-stu-id="1748a-321">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="1748a-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-322">Boolean</span></span>|<span data-ttu-id="1748a-323">USB ファイル転送をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-323">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="1748a-324">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="1748a-324">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="1748a-325">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-325">Int32</span></span>|<span data-ttu-id="1748a-326">[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-326">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="1748a-327">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="1748a-327">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1748a-328">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="1748a-328">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="1748a-329">Int32</span><span class="sxs-lookup"><span data-stu-id="1748a-329">Int32</span></span>|<span data-ttu-id="1748a-330">[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-330">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="1748a-331">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="1748a-331">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1748a-332">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1748a-332">systemUpdateInstallType</span></span>|[<span data-ttu-id="1748a-333">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1748a-333">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="1748a-334">システム更新構成の種類。</span><span class="sxs-lookup"><span data-stu-id="1748a-334">The type of system update configuration.</span></span> <span data-ttu-id="1748a-335">可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="1748a-335">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="1748a-336">systemwindowsblocked ブロック</span><span class="sxs-lookup"><span data-stu-id="1748a-336">systemWindowsBlocked</span></span>|<span data-ttu-id="1748a-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-337">Boolean</span></span>|<span data-ttu-id="1748a-338">Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1748a-338">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="1748a-339">ユーザー blockadd</span><span class="sxs-lookup"><span data-stu-id="1748a-339">usersBlockAdd</span></span>|<span data-ttu-id="1748a-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-340">Boolean</span></span>|<span data-ttu-id="1748a-341">ユーザーおよびプロファイルの追加を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-341">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="1748a-342">ユーザー blockremove</span><span class="sxs-lookup"><span data-stu-id="1748a-342">usersBlockRemove</span></span>|<span data-ttu-id="1748a-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-343">Boolean</span></span>|<span data-ttu-id="1748a-344">他のユーザーのデバイスからの削除を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-344">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="1748a-345">volumeblockadjustment</span><span class="sxs-lookup"><span data-stu-id="1748a-345">volumeBlockAdjustment</span></span>|<span data-ttu-id="1748a-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-346">Boolean</span></span>|<span data-ttu-id="1748a-347">マスターボリュームを調整するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-347">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="1748a-348">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="1748a-348">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="1748a-349">String</span><span class="sxs-lookup"><span data-stu-id="1748a-349">String</span></span>|<span data-ttu-id="1748a-350">always on VPN 接続を処理するアプリの Android アプリパッケージ名。</span><span class="sxs-lookup"><span data-stu-id="1748a-350">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="1748a-351">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="1748a-351">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="1748a-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-352">Boolean</span></span>|<span data-ttu-id="1748a-353">always on vpn パッケージ名が指定されている場合は、vpn が切断されたときにネットワークトラフィックをロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1748a-353">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="1748a-354">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="1748a-354">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="1748a-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-355">Boolean</span></span>|<span data-ttu-id="1748a-356">ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-356">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="1748a-357">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="1748a-357">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="1748a-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="1748a-358">Boolean</span></span>|<span data-ttu-id="1748a-359">ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1748a-359">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1748a-360">応答</span><span class="sxs-lookup"><span data-stu-id="1748a-360">Response</span></span>
<span data-ttu-id="1748a-361">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devic/オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1748a-361">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1748a-362">例</span><span class="sxs-lookup"><span data-stu-id="1748a-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="1748a-363">要求</span><span class="sxs-lookup"><span data-stu-id="1748a-363">Request</span></span>
<span data-ttu-id="1748a-364">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1748a-364">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2905

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="1748a-365">応答</span><span class="sxs-lookup"><span data-stu-id="1748a-365">Response</span></span>
<span data-ttu-id="1748a-p130">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1748a-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3077

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





