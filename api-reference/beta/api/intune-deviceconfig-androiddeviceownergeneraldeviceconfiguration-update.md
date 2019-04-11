---
title: androiddeviceowner一般の devic/デバイスの更新
description: androiddeviceownerのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fad142a5ec0f069c40185a40865e29ddee894789
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792371"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="62ba3-103">androiddeviceowner一般の devic/デバイスの更新</span><span class="sxs-lookup"><span data-stu-id="62ba3-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="62ba3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62ba3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62ba3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62ba3-106">[androiddeviceownerの](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62ba3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="62ba3-107">Prerequisites</span></span>
<span data-ttu-id="62ba3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62ba3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62ba3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62ba3-110">Permission type</span></span>|<span data-ttu-id="62ba3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="62ba3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62ba3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62ba3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62ba3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62ba3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62ba3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62ba3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62ba3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62ba3-115">Not supported.</span></span>|
|<span data-ttu-id="62ba3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62ba3-116">Application</span></span>|<span data-ttu-id="62ba3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62ba3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62ba3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62ba3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="62ba3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62ba3-119">Request headers</span></span>
|<span data-ttu-id="62ba3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62ba3-120">Header</span></span>|<span data-ttu-id="62ba3-121">値</span><span class="sxs-lookup"><span data-stu-id="62ba3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62ba3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62ba3-122">Authorization</span></span>|<span data-ttu-id="62ba3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62ba3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="62ba3-124">Accept</span></span>|<span data-ttu-id="62ba3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62ba3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62ba3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="62ba3-126">Request body</span></span>
<span data-ttu-id="62ba3-127">要求本文で、 [androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devic/devicオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="62ba3-128">次の表に、 [androiddeviceowner[devic]](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="62ba3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62ba3-129">Property</span></span>|<span data-ttu-id="62ba3-130">型</span><span class="sxs-lookup"><span data-stu-id="62ba3-130">Type</span></span>|<span data-ttu-id="62ba3-131">説明</span><span class="sxs-lookup"><span data-stu-id="62ba3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62ba3-132">id</span><span class="sxs-lookup"><span data-stu-id="62ba3-132">id</span></span>|<span data-ttu-id="62ba3-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="62ba3-133">String</span></span>|<span data-ttu-id="62ba3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="62ba3-134">Key of the entity.</span></span> <span data-ttu-id="62ba3-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62ba3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ba3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62ba3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="62ba3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62ba3-137">DateTimeOffset</span></span>|<span data-ttu-id="62ba3-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="62ba3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="62ba3-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62ba3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ba3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62ba3-140">roleScopeTagIds</span></span>|<span data-ttu-id="62ba3-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="62ba3-141">String collection</span></span>|<span data-ttu-id="62ba3-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="62ba3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62ba3-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62ba3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ba3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62ba3-144">supportsScopeTags</span></span>|<span data-ttu-id="62ba3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-145">Boolean</span></span>|<span data-ttu-id="62ba3-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62ba3-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="62ba3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62ba3-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="62ba3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62ba3-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-149">This property is read-only.</span></span> <span data-ttu-id="62ba3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62ba3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ba3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62ba3-151">createdDateTime</span></span>|<span data-ttu-id="62ba3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62ba3-152">DateTimeOffset</span></span>|<span data-ttu-id="62ba3-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="62ba3-153">DateTime the object was created.</span></span> <span data-ttu-id="62ba3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62ba3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ba3-155">説明</span><span class="sxs-lookup"><span data-stu-id="62ba3-155">description</span></span>|<span data-ttu-id="62ba3-156">String</span><span class="sxs-lookup"><span data-stu-id="62ba3-156">String</span></span>|<span data-ttu-id="62ba3-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="62ba3-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62ba3-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62ba3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ba3-159">displayName</span><span class="sxs-lookup"><span data-stu-id="62ba3-159">displayName</span></span>|<span data-ttu-id="62ba3-160">String</span><span class="sxs-lookup"><span data-stu-id="62ba3-160">String</span></span>|<span data-ttu-id="62ba3-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="62ba3-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62ba3-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62ba3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ba3-163">version</span><span class="sxs-lookup"><span data-stu-id="62ba3-163">version</span></span>|<span data-ttu-id="62ba3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-164">Int32</span></span>|<span data-ttu-id="62ba3-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="62ba3-165">Version of the device configuration.</span></span> <span data-ttu-id="62ba3-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62ba3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ba3-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="62ba3-167">accountsBlockModification</span></span>|<span data-ttu-id="62ba3-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-168">Boolean</span></span>|<span data-ttu-id="62ba3-169">アカウントの追加または削除が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="62ba3-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="62ba3-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="62ba3-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-171">Boolean</span></span>|<span data-ttu-id="62ba3-172">ユーザーが不明なソースを有効にできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="62ba3-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="62ba3-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="62ba3-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="62ba3-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="62ba3-175">アプリの自動更新ポリシーの値を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="62ba3-176">可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="62ba3-177">appsdefaultpermissionpolicy</span><span class="sxs-lookup"><span data-stu-id="62ba3-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="62ba3-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="62ba3-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="62ba3-179">アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="62ba3-180">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="62ba3-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="62ba3-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="62ba3-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-182">Boolean</span></span>|<span data-ttu-id="62ba3-183">すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="62ba3-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="62ba3-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="62ba3-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-185">Boolean</span></span>|<span data-ttu-id="62ba3-186">ユーザーが bluetooth を構成することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="62ba3-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="62ba3-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="62ba3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-188">Boolean</span></span>|<span data-ttu-id="62ba3-189">ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="62ba3-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="62ba3-190">cameraBlocked</span></span>|<span data-ttu-id="62ba3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-191">Boolean</span></span>|<span data-ttu-id="62ba3-192">カメラの使用を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="62ba3-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="62ba3-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="62ba3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-194">Boolean</span></span>|<span data-ttu-id="62ba3-195">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="62ba3-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="62ba3-196">dataRoamingBlocked</span></span>|<span data-ttu-id="62ba3-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-197">Boolean</span></span>|<span data-ttu-id="62ba3-198">ユーザーのデータ移動を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="62ba3-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="62ba3-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="62ba3-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-200">Boolean</span></span>|<span data-ttu-id="62ba3-201">ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="62ba3-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="62ba3-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="62ba3-203">String コレクション</span><span class="sxs-lookup"><span data-stu-id="62ba3-203">String collection</span></span>|<span data-ttu-id="62ba3-204">デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。</span><span class="sxs-lookup"><span data-stu-id="62ba3-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="62ba3-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="62ba3-205">factoryResetBlocked</span></span>|<span data-ttu-id="62ba3-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-206">Boolean</span></span>|<span data-ttu-id="62ba3-207">設定の出荷時のリセットオプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="62ba3-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="62ba3-208">kioskModeApps</span></span>|<span data-ttu-id="62ba3-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62ba3-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="62ba3-210">デバイスがキオスクモードのときに表示される管理対象アプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="62ba3-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="62ba3-211">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="62ba3-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="62ba3-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="62ba3-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="62ba3-213">文字列</span><span class="sxs-lookup"><span data-stu-id="62ba3-213">String</span></span>|<span data-ttu-id="62ba3-214">デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。</span><span class="sxs-lookup"><span data-stu-id="62ba3-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="62ba3-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="62ba3-215">kioskModeExitCode</span></span>|<span data-ttu-id="62ba3-216">文字列</span><span class="sxs-lookup"><span data-stu-id="62ba3-216">String</span></span>|<span data-ttu-id="62ba3-217">デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。</span><span class="sxs-lookup"><span data-stu-id="62ba3-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="62ba3-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="62ba3-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="62ba3-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-219">Boolean</span></span>|<span data-ttu-id="62ba3-220">デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="62ba3-221">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="62ba3-221">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="62ba3-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-222">Boolean</span></span>|<span data-ttu-id="62ba3-223">ユーザーがキオスクモードで Bluetooth 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-223">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="62ba3-224">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="62ba3-224">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="62ba3-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-225">Boolean</span></span>|<span data-ttu-id="62ba3-226">ユーザーがキオスクモードで wi-fi 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-226">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="62ba3-227">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="62ba3-227">microphoneForceMute</span></span>|<span data-ttu-id="62ba3-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-228">Boolean</span></span>|<span data-ttu-id="62ba3-229">デバイス上でのマイクのミュートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-229">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="62ba3-230">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="62ba3-230">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="62ba3-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-231">Boolean</span></span>|<span data-ttu-id="62ba3-232">ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-232">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="62ba3-233">nfcblockoutgoingbeam</span><span class="sxs-lookup"><span data-stu-id="62ba3-233">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="62ba3-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-234">Boolean</span></span>|<span data-ttu-id="62ba3-235">NFC の送信ビームをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-235">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="62ba3-236">passwordblockkeyguard</span><span class="sxs-lookup"><span data-stu-id="62ba3-236">passwordBlockKeyguard</span></span>|<span data-ttu-id="62ba3-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-237">Boolean</span></span>|<span data-ttu-id="62ba3-238">keyguard が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-238">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="62ba3-239">passwordblockkeygu/機能</span><span class="sxs-lookup"><span data-stu-id="62ba3-239">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="62ba3-240">[androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62ba3-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="62ba3-241">ブロックする device keyguard 機能のリストです。</span><span class="sxs-lookup"><span data-stu-id="62ba3-241">List of device keyguard features to block.</span></span> <span data-ttu-id="62ba3-242">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="62ba3-242">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="62ba3-243">可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-243">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="62ba3-244">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="62ba3-244">passwordExpirationDays</span></span>|<span data-ttu-id="62ba3-245">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-245">Int32</span></span>|<span data-ttu-id="62ba3-246">パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="62ba3-246">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="62ba3-247">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="62ba3-248">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="62ba3-248">passwordMinimumLength</span></span>|<span data-ttu-id="62ba3-249">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-249">Int32</span></span>|<span data-ttu-id="62ba3-250">デバイスで必要なパスワードの最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-250">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="62ba3-251">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-251">Valid values 4 to 16</span></span>|
|<span data-ttu-id="62ba3-252">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="62ba3-252">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="62ba3-253">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-253">Int32</span></span>|<span data-ttu-id="62ba3-254">デバイスパスワードに必要な文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-254">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="62ba3-255">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="62ba3-256">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="62ba3-256">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="62ba3-257">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-257">Int32</span></span>|<span data-ttu-id="62ba3-258">デバイスパスワードに必要な小文字の最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-258">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="62ba3-259">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-259">Valid values 1 to 16</span></span>|
|<span data-ttu-id="62ba3-260">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="62ba3-260">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="62ba3-261">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-261">Int32</span></span>|<span data-ttu-id="62ba3-262">デバイスパスワードに必要な文字以外の文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-262">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="62ba3-263">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-263">Valid values 1 to 16</span></span>|
|<span data-ttu-id="62ba3-264">passwordminimumnumericcharacters</span><span class="sxs-lookup"><span data-stu-id="62ba3-264">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="62ba3-265">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-265">Int32</span></span>|<span data-ttu-id="62ba3-266">デバイスパスワードに必要な最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-266">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="62ba3-267">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="62ba3-268">passwordminimumシンボル文字</span><span class="sxs-lookup"><span data-stu-id="62ba3-268">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="62ba3-269">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-269">Int32</span></span>|<span data-ttu-id="62ba3-270">デバイスパスワードに必要な最小記号文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-270">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="62ba3-271">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="62ba3-272">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="62ba3-272">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="62ba3-273">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-273">Int32</span></span>|<span data-ttu-id="62ba3-274">デバイスのパスワードに必要な上位 caseletter 文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-274">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="62ba3-275">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="62ba3-276">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="62ba3-276">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="62ba3-277">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-277">Int32</span></span>|<span data-ttu-id="62ba3-278">画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。</span><span class="sxs-lookup"><span data-stu-id="62ba3-278">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="62ba3-279">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="62ba3-279">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="62ba3-280">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-280">Int32</span></span>|<span data-ttu-id="62ba3-281">パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。</span><span class="sxs-lookup"><span data-stu-id="62ba3-281">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="62ba3-282">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-282">Valid values 0 to 24</span></span>|
|<span data-ttu-id="62ba3-283">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="62ba3-283">passwordRequiredType</span></span>|[<span data-ttu-id="62ba3-284">androiddeviceownerrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="62ba3-284">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="62ba3-285">デバイスで必要なパスワードの最小品質を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-285">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="62ba3-286">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-286">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="62ba3-287">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="62ba3-287">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="62ba3-288">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-288">Int32</span></span>|<span data-ttu-id="62ba3-289">ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-289">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="62ba3-290">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="62ba3-290">Valid values 4 to 11</span></span>|
|<span data-ttu-id="62ba3-291">playstoremode</span><span class="sxs-lookup"><span data-stu-id="62ba3-291">playStoreMode</span></span>|[<span data-ttu-id="62ba3-292">androiddeviceownerplaystoremode</span><span class="sxs-lookup"><span data-stu-id="62ba3-292">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="62ba3-293">デバイスの再生ストアモードを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-293">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="62ba3-294">使用可能な値は、`notConfigured`、`allowList`、`blockList` です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-294">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="62ba3-295">safebootblocked</span><span class="sxs-lookup"><span data-stu-id="62ba3-295">safeBootBlocked</span></span>|<span data-ttu-id="62ba3-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-296">Boolean</span></span>|<span data-ttu-id="62ba3-297">セーフブートでのデバイスの再起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-297">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="62ba3-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="62ba3-298">screenCaptureBlocked</span></span>|<span data-ttu-id="62ba3-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-299">Boolean</span></span>|<span data-ttu-id="62ba3-300">スクリーンショットを撮影する機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-300">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="62ba3-301">securityallowデバッグ機能</span><span class="sxs-lookup"><span data-stu-id="62ba3-301">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="62ba3-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-302">Boolean</span></span>|<span data-ttu-id="62ba3-303">ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-303">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="62ba3-304">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="62ba3-304">securityRequireVerifyApps</span></span>|<span data-ttu-id="62ba3-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-305">Boolean</span></span>|<span data-ttu-id="62ba3-306">アプリを確認する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-306">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="62ba3-307">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="62ba3-307">statusBarBlocked</span></span>|<span data-ttu-id="62ba3-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-308">Boolean</span></span>|<span data-ttu-id="62ba3-309">通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-309">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="62ba3-310">stayonmodes</span><span class="sxs-lookup"><span data-stu-id="62ba3-310">stayOnModes</span></span>|<span data-ttu-id="62ba3-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62ba3-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="62ba3-312">デバイスの表示がオンのままになるモードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-312">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="62ba3-313">このコレクションには、最大4つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="62ba3-313">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="62ba3-314">可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-314">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="62ba3-315">storageallowusb</span><span class="sxs-lookup"><span data-stu-id="62ba3-315">storageAllowUsb</span></span>|<span data-ttu-id="62ba3-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-316">Boolean</span></span>|<span data-ttu-id="62ba3-317">USB 大容量ストレージを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-317">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="62ba3-318">storageblockexternalmedia</span><span class="sxs-lookup"><span data-stu-id="62ba3-318">storageBlockExternalMedia</span></span>|<span data-ttu-id="62ba3-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-319">Boolean</span></span>|<span data-ttu-id="62ba3-320">外部メディアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-320">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="62ba3-321">storageblockusbfiletransfer</span><span class="sxs-lookup"><span data-stu-id="62ba3-321">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="62ba3-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-322">Boolean</span></span>|<span data-ttu-id="62ba3-323">USB ファイル転送をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-323">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="62ba3-324">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="62ba3-324">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="62ba3-325">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-325">Int32</span></span>|<span data-ttu-id="62ba3-326">[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-326">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="62ba3-327">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="62ba3-327">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="62ba3-328">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="62ba3-328">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="62ba3-329">Int32</span><span class="sxs-lookup"><span data-stu-id="62ba3-329">Int32</span></span>|<span data-ttu-id="62ba3-330">[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-330">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="62ba3-331">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="62ba3-331">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="62ba3-332">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="62ba3-332">systemUpdateInstallType</span></span>|[<span data-ttu-id="62ba3-333">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="62ba3-333">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="62ba3-334">システム更新構成の種類。</span><span class="sxs-lookup"><span data-stu-id="62ba3-334">The type of system update configuration.</span></span> <span data-ttu-id="62ba3-335">可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-335">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="62ba3-336">systemwindowsblocked ブロック</span><span class="sxs-lookup"><span data-stu-id="62ba3-336">systemWindowsBlocked</span></span>|<span data-ttu-id="62ba3-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-337">Boolean</span></span>|<span data-ttu-id="62ba3-338">Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-338">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="62ba3-339">ユーザー blockadd</span><span class="sxs-lookup"><span data-stu-id="62ba3-339">usersBlockAdd</span></span>|<span data-ttu-id="62ba3-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-340">Boolean</span></span>|<span data-ttu-id="62ba3-341">ユーザーおよびプロファイルの追加を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-341">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="62ba3-342">ユーザー blockremove</span><span class="sxs-lookup"><span data-stu-id="62ba3-342">usersBlockRemove</span></span>|<span data-ttu-id="62ba3-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-343">Boolean</span></span>|<span data-ttu-id="62ba3-344">他のユーザーのデバイスからの削除を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-344">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="62ba3-345">volumeblockadjustment</span><span class="sxs-lookup"><span data-stu-id="62ba3-345">volumeBlockAdjustment</span></span>|<span data-ttu-id="62ba3-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-346">Boolean</span></span>|<span data-ttu-id="62ba3-347">マスターボリュームを調整するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-347">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="62ba3-348">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="62ba3-348">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="62ba3-349">文字列</span><span class="sxs-lookup"><span data-stu-id="62ba3-349">String</span></span>|<span data-ttu-id="62ba3-350">always on VPN 接続を処理するアプリの Android アプリパッケージ名。</span><span class="sxs-lookup"><span data-stu-id="62ba3-350">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="62ba3-351">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="62ba3-351">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="62ba3-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-352">Boolean</span></span>|<span data-ttu-id="62ba3-353">always on vpn パッケージ名が指定されている場合は、vpn が切断されたときにネットワークトラフィックをロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-353">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="62ba3-354">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="62ba3-354">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="62ba3-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-355">Boolean</span></span>|<span data-ttu-id="62ba3-356">ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-356">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="62ba3-357">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="62ba3-357">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="62ba3-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="62ba3-358">Boolean</span></span>|<span data-ttu-id="62ba3-359">ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-359">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="62ba3-360">応答</span><span class="sxs-lookup"><span data-stu-id="62ba3-360">Response</span></span>
<span data-ttu-id="62ba3-361">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devic/オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62ba3-361">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62ba3-362">例</span><span class="sxs-lookup"><span data-stu-id="62ba3-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="62ba3-363">要求</span><span class="sxs-lookup"><span data-stu-id="62ba3-363">Request</span></span>
<span data-ttu-id="62ba3-364">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62ba3-364">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62ba3-365">応答</span><span class="sxs-lookup"><span data-stu-id="62ba3-365">Response</span></span>
<span data-ttu-id="62ba3-p130">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62ba3-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





