---
title: androiddeviceowner一般の devic/デバイスの作成
description: 新しい androiddeviceowner一般の devic/デバイスオブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa5f2ac532e4b8e912b47a50be755ab0ceb495fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32481025"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="e968f-103">androiddeviceowner一般の devic/デバイスの作成</span><span class="sxs-lookup"><span data-stu-id="e968f-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e968f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e968f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e968f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e968f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e968f-106">新しい[androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e968f-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e968f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e968f-107">Prerequisites</span></span>
<span data-ttu-id="e968f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e968f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e968f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e968f-110">Permission type</span></span>|<span data-ttu-id="e968f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e968f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e968f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e968f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e968f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e968f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e968f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e968f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e968f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e968f-115">Not supported.</span></span>|
|<span data-ttu-id="e968f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e968f-116">Application</span></span>|<span data-ttu-id="e968f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e968f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e968f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e968f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e968f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e968f-119">Request headers</span></span>
|<span data-ttu-id="e968f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e968f-120">Header</span></span>|<span data-ttu-id="e968f-121">値</span><span class="sxs-lookup"><span data-stu-id="e968f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e968f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e968f-122">Authorization</span></span>|<span data-ttu-id="e968f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e968f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e968f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e968f-124">Accept</span></span>|<span data-ttu-id="e968f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e968f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e968f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e968f-126">Request body</span></span>
<span data-ttu-id="e968f-127">要求本文で、androiddeviceowner一般の devic/devicオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e968f-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="e968f-128">次の表に、androiddeviceowner[devic] の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="e968f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e968f-129">Property</span></span>|<span data-ttu-id="e968f-130">型</span><span class="sxs-lookup"><span data-stu-id="e968f-130">Type</span></span>|<span data-ttu-id="e968f-131">説明</span><span class="sxs-lookup"><span data-stu-id="e968f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e968f-132">id</span><span class="sxs-lookup"><span data-stu-id="e968f-132">id</span></span>|<span data-ttu-id="e968f-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e968f-133">String</span></span>|<span data-ttu-id="e968f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e968f-134">Key of the entity.</span></span> <span data-ttu-id="e968f-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e968f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e968f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e968f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e968f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e968f-137">DateTimeOffset</span></span>|<span data-ttu-id="e968f-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e968f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e968f-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e968f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e968f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e968f-140">roleScopeTagIds</span></span>|<span data-ttu-id="e968f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e968f-141">String collection</span></span>|<span data-ttu-id="e968f-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e968f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e968f-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e968f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e968f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e968f-144">supportsScopeTags</span></span>|<span data-ttu-id="e968f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-145">Boolean</span></span>|<span data-ttu-id="e968f-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e968f-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e968f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e968f-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e968f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e968f-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e968f-149">This property is read-only.</span></span> <span data-ttu-id="e968f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e968f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e968f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e968f-151">createdDateTime</span></span>|<span data-ttu-id="e968f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e968f-152">DateTimeOffset</span></span>|<span data-ttu-id="e968f-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e968f-153">DateTime the object was created.</span></span> <span data-ttu-id="e968f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e968f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e968f-155">説明</span><span class="sxs-lookup"><span data-stu-id="e968f-155">description</span></span>|<span data-ttu-id="e968f-156">String</span><span class="sxs-lookup"><span data-stu-id="e968f-156">String</span></span>|<span data-ttu-id="e968f-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e968f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e968f-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e968f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e968f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e968f-159">displayName</span></span>|<span data-ttu-id="e968f-160">String</span><span class="sxs-lookup"><span data-stu-id="e968f-160">String</span></span>|<span data-ttu-id="e968f-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e968f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e968f-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e968f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e968f-163">version</span><span class="sxs-lookup"><span data-stu-id="e968f-163">version</span></span>|<span data-ttu-id="e968f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-164">Int32</span></span>|<span data-ttu-id="e968f-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e968f-165">Version of the device configuration.</span></span> <span data-ttu-id="e968f-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e968f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e968f-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="e968f-167">accountsBlockModification</span></span>|<span data-ttu-id="e968f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-168">Boolean</span></span>|<span data-ttu-id="e968f-169">アカウントの追加または削除が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="e968f-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="e968f-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="e968f-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-171">Boolean</span></span>|<span data-ttu-id="e968f-172">ユーザーが不明なソースを有効にできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="e968f-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="e968f-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="e968f-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="e968f-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="e968f-175">アプリの自動更新ポリシーの値を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="e968f-176">可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。</span><span class="sxs-lookup"><span data-stu-id="e968f-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="e968f-177">appsdefaultpermissionpolicy</span><span class="sxs-lookup"><span data-stu-id="e968f-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="e968f-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e968f-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="e968f-179">アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="e968f-180">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="e968f-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e968f-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="e968f-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="e968f-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-182">Boolean</span></span>|<span data-ttu-id="e968f-183">すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e968f-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="e968f-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="e968f-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="e968f-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-185">Boolean</span></span>|<span data-ttu-id="e968f-186">ユーザーが bluetooth を構成することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="e968f-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="e968f-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="e968f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-188">Boolean</span></span>|<span data-ttu-id="e968f-189">ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="e968f-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e968f-190">cameraBlocked</span></span>|<span data-ttu-id="e968f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-191">Boolean</span></span>|<span data-ttu-id="e968f-192">カメラの使用を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="e968f-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="e968f-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="e968f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-194">Boolean</span></span>|<span data-ttu-id="e968f-195">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="e968f-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="e968f-196">dataRoamingBlocked</span></span>|<span data-ttu-id="e968f-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-197">Boolean</span></span>|<span data-ttu-id="e968f-198">ユーザーのデータ移動を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="e968f-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="e968f-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="e968f-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-200">Boolean</span></span>|<span data-ttu-id="e968f-201">ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="e968f-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="e968f-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="e968f-203">String collection</span><span class="sxs-lookup"><span data-stu-id="e968f-203">String collection</span></span>|<span data-ttu-id="e968f-204">デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。</span><span class="sxs-lookup"><span data-stu-id="e968f-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="e968f-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="e968f-205">factoryResetBlocked</span></span>|<span data-ttu-id="e968f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-206">Boolean</span></span>|<span data-ttu-id="e968f-207">設定の出荷時のリセットオプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="e968f-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="e968f-208">kioskModeApps</span></span>|<span data-ttu-id="e968f-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e968f-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e968f-210">デバイスがキオスクモードのときに表示される管理対象アプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="e968f-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="e968f-211">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e968f-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e968f-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="e968f-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="e968f-213">String</span><span class="sxs-lookup"><span data-stu-id="e968f-213">String</span></span>|<span data-ttu-id="e968f-214">デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。</span><span class="sxs-lookup"><span data-stu-id="e968f-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e968f-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="e968f-215">kioskModeExitCode</span></span>|<span data-ttu-id="e968f-216">String</span><span class="sxs-lookup"><span data-stu-id="e968f-216">String</span></span>|<span data-ttu-id="e968f-217">デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。</span><span class="sxs-lookup"><span data-stu-id="e968f-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e968f-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="e968f-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="e968f-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-219">Boolean</span></span>|<span data-ttu-id="e968f-220">デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e968f-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e968f-221">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="e968f-221">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="e968f-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-222">Boolean</span></span>|<span data-ttu-id="e968f-223">ユーザーがキオスクモードで Bluetooth 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e968f-223">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="e968f-224">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="e968f-224">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="e968f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-225">Boolean</span></span>|<span data-ttu-id="e968f-226">ユーザーがキオスクモードで wi-fi 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e968f-226">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="e968f-227">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="e968f-227">microphoneForceMute</span></span>|<span data-ttu-id="e968f-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-228">Boolean</span></span>|<span data-ttu-id="e968f-229">デバイス上でのマイクのミュートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-229">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="e968f-230">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="e968f-230">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="e968f-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-231">Boolean</span></span>|<span data-ttu-id="e968f-232">ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-232">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="e968f-233">nfcblockoutgoingbeam</span><span class="sxs-lookup"><span data-stu-id="e968f-233">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="e968f-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-234">Boolean</span></span>|<span data-ttu-id="e968f-235">NFC の送信ビームをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-235">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="e968f-236">passwordblockkeyguard</span><span class="sxs-lookup"><span data-stu-id="e968f-236">passwordBlockKeyguard</span></span>|<span data-ttu-id="e968f-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-237">Boolean</span></span>|<span data-ttu-id="e968f-238">keyguard が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-238">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="e968f-239">passwordblockkeygu/機能</span><span class="sxs-lookup"><span data-stu-id="e968f-239">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="e968f-240">[androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e968f-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="e968f-241">ブロックする device keyguard 機能のリストです。</span><span class="sxs-lookup"><span data-stu-id="e968f-241">List of device keyguard features to block.</span></span> <span data-ttu-id="e968f-242">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e968f-242">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="e968f-243">可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。</span><span class="sxs-lookup"><span data-stu-id="e968f-243">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="e968f-244">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e968f-244">passwordExpirationDays</span></span>|<span data-ttu-id="e968f-245">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-245">Int32</span></span>|<span data-ttu-id="e968f-246">パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e968f-246">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="e968f-247">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="e968f-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e968f-248">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e968f-248">passwordMinimumLength</span></span>|<span data-ttu-id="e968f-249">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-249">Int32</span></span>|<span data-ttu-id="e968f-250">デバイスで必要なパスワードの最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-250">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="e968f-251">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="e968f-251">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e968f-252">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e968f-252">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="e968f-253">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-253">Int32</span></span>|<span data-ttu-id="e968f-254">デバイスパスワードに必要な文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-254">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="e968f-255">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e968f-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e968f-256">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e968f-256">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="e968f-257">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-257">Int32</span></span>|<span data-ttu-id="e968f-258">デバイスパスワードに必要な小文字の最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-258">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="e968f-259">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e968f-259">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e968f-260">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e968f-260">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="e968f-261">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-261">Int32</span></span>|<span data-ttu-id="e968f-262">デバイスパスワードに必要な文字以外の文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-262">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="e968f-263">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e968f-263">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e968f-264">passwordminimumnumericcharacters</span><span class="sxs-lookup"><span data-stu-id="e968f-264">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="e968f-265">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-265">Int32</span></span>|<span data-ttu-id="e968f-266">デバイスパスワードに必要な最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-266">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="e968f-267">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e968f-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e968f-268">passwordminimumシンボル文字</span><span class="sxs-lookup"><span data-stu-id="e968f-268">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="e968f-269">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-269">Int32</span></span>|<span data-ttu-id="e968f-270">デバイスパスワードに必要な最小記号文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-270">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="e968f-271">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e968f-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e968f-272">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e968f-272">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="e968f-273">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-273">Int32</span></span>|<span data-ttu-id="e968f-274">デバイスのパスワードに必要な上位 caseletter 文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-274">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="e968f-275">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e968f-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e968f-276">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e968f-276">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e968f-277">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-277">Int32</span></span>|<span data-ttu-id="e968f-278">画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。</span><span class="sxs-lookup"><span data-stu-id="e968f-278">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e968f-279">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="e968f-279">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="e968f-280">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-280">Int32</span></span>|<span data-ttu-id="e968f-281">パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。</span><span class="sxs-lookup"><span data-stu-id="e968f-281">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="e968f-282">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="e968f-282">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e968f-283">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e968f-283">passwordRequiredType</span></span>|[<span data-ttu-id="e968f-284">androiddeviceownerrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="e968f-284">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="e968f-285">デバイスで必要なパスワードの最小品質を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-285">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="e968f-286">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。</span><span class="sxs-lookup"><span data-stu-id="e968f-286">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="e968f-287">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e968f-287">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e968f-288">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-288">Int32</span></span>|<span data-ttu-id="e968f-289">ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-289">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="e968f-290">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="e968f-290">Valid values 4 to 11</span></span>|
|<span data-ttu-id="e968f-291">playstoremode</span><span class="sxs-lookup"><span data-stu-id="e968f-291">playStoreMode</span></span>|[<span data-ttu-id="e968f-292">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="e968f-292">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="e968f-293">デバイスの再生ストアモードを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-293">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="e968f-294">使用可能な値は、`notConfigured`、`allowList`、`blockList` です。</span><span class="sxs-lookup"><span data-stu-id="e968f-294">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="e968f-295">safebootblocked</span><span class="sxs-lookup"><span data-stu-id="e968f-295">safeBootBlocked</span></span>|<span data-ttu-id="e968f-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-296">Boolean</span></span>|<span data-ttu-id="e968f-297">セーフブートでのデバイスの再起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-297">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="e968f-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e968f-298">screenCaptureBlocked</span></span>|<span data-ttu-id="e968f-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-299">Boolean</span></span>|<span data-ttu-id="e968f-300">スクリーンショットを撮影する機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-300">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="e968f-301">securityallowデバッグ機能</span><span class="sxs-lookup"><span data-stu-id="e968f-301">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="e968f-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-302">Boolean</span></span>|<span data-ttu-id="e968f-303">ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-303">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="e968f-304">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e968f-304">securityRequireVerifyApps</span></span>|<span data-ttu-id="e968f-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-305">Boolean</span></span>|<span data-ttu-id="e968f-306">アプリを確認する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-306">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="e968f-307">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="e968f-307">statusBarBlocked</span></span>|<span data-ttu-id="e968f-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-308">Boolean</span></span>|<span data-ttu-id="e968f-309">通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-309">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="e968f-310">stayonmodes</span><span class="sxs-lookup"><span data-stu-id="e968f-310">stayOnModes</span></span>|<span data-ttu-id="e968f-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e968f-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="e968f-312">デバイスの表示がオンのままになるモードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="e968f-312">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="e968f-313">このコレクションには、最大4つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e968f-313">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="e968f-314">可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。</span><span class="sxs-lookup"><span data-stu-id="e968f-314">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="e968f-315">storageallowusb</span><span class="sxs-lookup"><span data-stu-id="e968f-315">storageAllowUsb</span></span>|<span data-ttu-id="e968f-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-316">Boolean</span></span>|<span data-ttu-id="e968f-317">USB 大容量ストレージを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-317">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="e968f-318">storageblockexternalmedia</span><span class="sxs-lookup"><span data-stu-id="e968f-318">storageBlockExternalMedia</span></span>|<span data-ttu-id="e968f-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-319">Boolean</span></span>|<span data-ttu-id="e968f-320">外部メディアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-320">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="e968f-321">storageblockusbfiletransfer</span><span class="sxs-lookup"><span data-stu-id="e968f-321">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="e968f-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-322">Boolean</span></span>|<span data-ttu-id="e968f-323">USB ファイル転送をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-323">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="e968f-324">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="e968f-324">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="e968f-325">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-325">Int32</span></span>|<span data-ttu-id="e968f-326">[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-326">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="e968f-327">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="e968f-327">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="e968f-328">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="e968f-328">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="e968f-329">Int32</span><span class="sxs-lookup"><span data-stu-id="e968f-329">Int32</span></span>|<span data-ttu-id="e968f-330">[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-330">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="e968f-331">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="e968f-331">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="e968f-332">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="e968f-332">systemUpdateInstallType</span></span>|[<span data-ttu-id="e968f-333">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="e968f-333">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="e968f-334">システム更新構成の種類。</span><span class="sxs-lookup"><span data-stu-id="e968f-334">The type of system update configuration.</span></span> <span data-ttu-id="e968f-335">可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="e968f-335">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="e968f-336">systemwindowsblocked ブロック</span><span class="sxs-lookup"><span data-stu-id="e968f-336">systemWindowsBlocked</span></span>|<span data-ttu-id="e968f-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-337">Boolean</span></span>|<span data-ttu-id="e968f-338">Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e968f-338">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="e968f-339">ユーザー blockadd</span><span class="sxs-lookup"><span data-stu-id="e968f-339">usersBlockAdd</span></span>|<span data-ttu-id="e968f-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-340">Boolean</span></span>|<span data-ttu-id="e968f-341">ユーザーおよびプロファイルの追加を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-341">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="e968f-342">ユーザー blockremove</span><span class="sxs-lookup"><span data-stu-id="e968f-342">usersBlockRemove</span></span>|<span data-ttu-id="e968f-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-343">Boolean</span></span>|<span data-ttu-id="e968f-344">他のユーザーのデバイスからの削除を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-344">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="e968f-345">volumeblockadjustment</span><span class="sxs-lookup"><span data-stu-id="e968f-345">volumeBlockAdjustment</span></span>|<span data-ttu-id="e968f-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-346">Boolean</span></span>|<span data-ttu-id="e968f-347">マスターボリュームを調整するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-347">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="e968f-348">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="e968f-348">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="e968f-349">String</span><span class="sxs-lookup"><span data-stu-id="e968f-349">String</span></span>|<span data-ttu-id="e968f-350">always on VPN 接続を処理するアプリの Android アプリパッケージ名。</span><span class="sxs-lookup"><span data-stu-id="e968f-350">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="e968f-351">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="e968f-351">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="e968f-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-352">Boolean</span></span>|<span data-ttu-id="e968f-353">always on vpn パッケージ名が指定されている場合は、vpn が切断されたときにネットワークトラフィックをロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e968f-353">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="e968f-354">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="e968f-354">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="e968f-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-355">Boolean</span></span>|<span data-ttu-id="e968f-356">ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-356">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="e968f-357">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="e968f-357">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="e968f-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="e968f-358">Boolean</span></span>|<span data-ttu-id="e968f-359">ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e968f-359">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="e968f-360">応答</span><span class="sxs-lookup"><span data-stu-id="e968f-360">Response</span></span>
<span data-ttu-id="e968f-361">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e968f-361">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e968f-362">例</span><span class="sxs-lookup"><span data-stu-id="e968f-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="e968f-363">要求</span><span class="sxs-lookup"><span data-stu-id="e968f-363">Request</span></span>
<span data-ttu-id="e968f-364">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e968f-364">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="e968f-365">応答</span><span class="sxs-lookup"><span data-stu-id="e968f-365">Response</span></span>
<span data-ttu-id="e968f-p130">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e968f-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





