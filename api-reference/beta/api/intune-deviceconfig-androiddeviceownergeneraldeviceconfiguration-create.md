---
title: androiddeviceowner一般の devic/デバイスの作成
description: 新しい androiddeviceowner一般の devic/デバイスオブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cd38922bd7daa8f3e805208fe7c70d6d4abe777
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571943"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="90d06-103">androiddeviceowner一般の devic/デバイスの作成</span><span class="sxs-lookup"><span data-stu-id="90d06-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="90d06-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90d06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90d06-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90d06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90d06-106">新しい[androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="90d06-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90d06-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="90d06-107">Prerequisites</span></span>
<span data-ttu-id="90d06-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="90d06-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90d06-110">Permission type</span></span>|<span data-ttu-id="90d06-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="90d06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90d06-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90d06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90d06-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90d06-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90d06-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90d06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90d06-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90d06-115">Not supported.</span></span>|
|<span data-ttu-id="90d06-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90d06-116">Application</span></span>|<span data-ttu-id="90d06-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90d06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90d06-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90d06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90d06-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90d06-119">Request headers</span></span>
|<span data-ttu-id="90d06-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90d06-120">Header</span></span>|<span data-ttu-id="90d06-121">値</span><span class="sxs-lookup"><span data-stu-id="90d06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90d06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90d06-122">Authorization</span></span>|<span data-ttu-id="90d06-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="90d06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90d06-124">承諾</span><span class="sxs-lookup"><span data-stu-id="90d06-124">Accept</span></span>|<span data-ttu-id="90d06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90d06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90d06-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="90d06-126">Request body</span></span>
<span data-ttu-id="90d06-127">要求本文で、androiddeviceowner一般の devic/devicオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="90d06-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="90d06-128">次の表に、androiddeviceowner[devic] の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="90d06-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90d06-129">Property</span></span>|<span data-ttu-id="90d06-130">型</span><span class="sxs-lookup"><span data-stu-id="90d06-130">Type</span></span>|<span data-ttu-id="90d06-131">説明</span><span class="sxs-lookup"><span data-stu-id="90d06-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90d06-132">id</span><span class="sxs-lookup"><span data-stu-id="90d06-132">id</span></span>|<span data-ttu-id="90d06-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="90d06-133">String</span></span>|<span data-ttu-id="90d06-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="90d06-134">Key of the entity.</span></span> <span data-ttu-id="90d06-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90d06-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90d06-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90d06-136">lastModifiedDateTime</span></span>|<span data-ttu-id="90d06-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90d06-137">DateTimeOffset</span></span>|<span data-ttu-id="90d06-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="90d06-138">DateTime the object was last modified.</span></span> <span data-ttu-id="90d06-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90d06-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90d06-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90d06-140">roleScopeTagIds</span></span>|<span data-ttu-id="90d06-141">String collection</span><span class="sxs-lookup"><span data-stu-id="90d06-141">String collection</span></span>|<span data-ttu-id="90d06-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="90d06-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="90d06-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90d06-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90d06-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="90d06-144">supportsScopeTags</span></span>|<span data-ttu-id="90d06-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-145">Boolean</span></span>|<span data-ttu-id="90d06-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="90d06-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="90d06-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="90d06-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="90d06-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="90d06-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="90d06-149">This property is read-only.</span></span> <span data-ttu-id="90d06-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90d06-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90d06-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90d06-151">createdDateTime</span></span>|<span data-ttu-id="90d06-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90d06-152">DateTimeOffset</span></span>|<span data-ttu-id="90d06-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="90d06-153">DateTime the object was created.</span></span> <span data-ttu-id="90d06-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90d06-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90d06-155">description</span><span class="sxs-lookup"><span data-stu-id="90d06-155">description</span></span>|<span data-ttu-id="90d06-156">String</span><span class="sxs-lookup"><span data-stu-id="90d06-156">String</span></span>|<span data-ttu-id="90d06-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="90d06-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90d06-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90d06-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90d06-159">displayName</span><span class="sxs-lookup"><span data-stu-id="90d06-159">displayName</span></span>|<span data-ttu-id="90d06-160">String</span><span class="sxs-lookup"><span data-stu-id="90d06-160">String</span></span>|<span data-ttu-id="90d06-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="90d06-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90d06-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90d06-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90d06-163">version</span><span class="sxs-lookup"><span data-stu-id="90d06-163">version</span></span>|<span data-ttu-id="90d06-164">Int32</span><span class="sxs-lookup"><span data-stu-id="90d06-164">Int32</span></span>|<span data-ttu-id="90d06-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="90d06-165">Version of the device configuration.</span></span> <span data-ttu-id="90d06-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90d06-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90d06-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="90d06-167">accountsBlockModification</span></span>|<span data-ttu-id="90d06-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-168">Boolean</span></span>|<span data-ttu-id="90d06-169">アカウントの追加または削除が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="90d06-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="90d06-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="90d06-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-171">Boolean</span></span>|<span data-ttu-id="90d06-172">ユーザーが不明なソースを有効にできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="90d06-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="90d06-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="90d06-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="90d06-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="90d06-175">アプリの自動更新ポリシーの値を示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="90d06-176">可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。</span><span class="sxs-lookup"><span data-stu-id="90d06-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="90d06-177">appsdefaultpermissionpolicy</span><span class="sxs-lookup"><span data-stu-id="90d06-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="90d06-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="90d06-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="90d06-179">アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="90d06-180">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="90d06-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="90d06-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="90d06-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="90d06-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-182">Boolean</span></span>|<span data-ttu-id="90d06-183">すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="90d06-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="90d06-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="90d06-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="90d06-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-185">Boolean</span></span>|<span data-ttu-id="90d06-186">ユーザーが bluetooth を構成することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="90d06-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="90d06-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="90d06-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-188">Boolean</span></span>|<span data-ttu-id="90d06-189">ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="90d06-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="90d06-190">cameraBlocked</span></span>|<span data-ttu-id="90d06-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-191">Boolean</span></span>|<span data-ttu-id="90d06-192">カメラの使用を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="90d06-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="90d06-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="90d06-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-194">Boolean</span></span>|<span data-ttu-id="90d06-195">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="90d06-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="90d06-196">dataRoamingBlocked</span></span>|<span data-ttu-id="90d06-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-197">Boolean</span></span>|<span data-ttu-id="90d06-198">ユーザーのデータ移動を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="90d06-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="90d06-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="90d06-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-200">Boolean</span></span>|<span data-ttu-id="90d06-201">ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="90d06-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="90d06-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="90d06-203">String collection</span><span class="sxs-lookup"><span data-stu-id="90d06-203">String collection</span></span>|<span data-ttu-id="90d06-204">デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。</span><span class="sxs-lookup"><span data-stu-id="90d06-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="90d06-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="90d06-205">factoryResetBlocked</span></span>|<span data-ttu-id="90d06-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-206">Boolean</span></span>|<span data-ttu-id="90d06-207">設定の出荷時のリセットオプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="90d06-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="90d06-208">kioskModeApps</span></span>|<span data-ttu-id="90d06-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="90d06-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="90d06-210">デバイスがキオスクモードのときに表示される管理対象アプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="90d06-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="90d06-211">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="90d06-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="90d06-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="90d06-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="90d06-213">String</span><span class="sxs-lookup"><span data-stu-id="90d06-213">String</span></span>|<span data-ttu-id="90d06-214">デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。</span><span class="sxs-lookup"><span data-stu-id="90d06-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="90d06-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="90d06-215">kioskModeExitCode</span></span>|<span data-ttu-id="90d06-216">String</span><span class="sxs-lookup"><span data-stu-id="90d06-216">String</span></span>|<span data-ttu-id="90d06-217">デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。</span><span class="sxs-lookup"><span data-stu-id="90d06-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="90d06-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="90d06-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="90d06-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-219">Boolean</span></span>|<span data-ttu-id="90d06-220">デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="90d06-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="90d06-221">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="90d06-221">microphoneForceMute</span></span>|<span data-ttu-id="90d06-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-222">Boolean</span></span>|<span data-ttu-id="90d06-223">デバイス上でのマイクのミュートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-223">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="90d06-224">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="90d06-224">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="90d06-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-225">Boolean</span></span>|<span data-ttu-id="90d06-226">ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-226">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="90d06-227">nfcblockoutgoingbeam</span><span class="sxs-lookup"><span data-stu-id="90d06-227">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="90d06-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-228">Boolean</span></span>|<span data-ttu-id="90d06-229">NFC の送信ビームをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-229">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="90d06-230">passwordblockkeyguard</span><span class="sxs-lookup"><span data-stu-id="90d06-230">passwordBlockKeyguard</span></span>|<span data-ttu-id="90d06-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-231">Boolean</span></span>|<span data-ttu-id="90d06-232">keyguard が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-232">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="90d06-233">passwordblockkeygu/機能</span><span class="sxs-lookup"><span data-stu-id="90d06-233">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="90d06-234">[androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="90d06-234">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="90d06-235">ブロックする device keyguard 機能のリストです。</span><span class="sxs-lookup"><span data-stu-id="90d06-235">List of device keyguard features to block.</span></span> <span data-ttu-id="90d06-236">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="90d06-236">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="90d06-237">可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。</span><span class="sxs-lookup"><span data-stu-id="90d06-237">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="90d06-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="90d06-238">passwordExpirationDays</span></span>|<span data-ttu-id="90d06-239">Int32</span><span class="sxs-lookup"><span data-stu-id="90d06-239">Int32</span></span>|<span data-ttu-id="90d06-240">パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="90d06-240">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="90d06-241">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="90d06-241">Valid values 1 to 365</span></span>|
|<span data-ttu-id="90d06-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="90d06-242">passwordMinimumLength</span></span>|<span data-ttu-id="90d06-243">Int32</span><span class="sxs-lookup"><span data-stu-id="90d06-243">Int32</span></span>|<span data-ttu-id="90d06-244">デバイスで必要なパスワードの最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-244">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="90d06-245">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="90d06-245">Valid values 4 to 16</span></span>|
|<span data-ttu-id="90d06-246">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="90d06-246">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="90d06-247">Int32</span><span class="sxs-lookup"><span data-stu-id="90d06-247">Int32</span></span>|<span data-ttu-id="90d06-248">画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。</span><span class="sxs-lookup"><span data-stu-id="90d06-248">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="90d06-249">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="90d06-249">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="90d06-250">Int32</span><span class="sxs-lookup"><span data-stu-id="90d06-250">Int32</span></span>|<span data-ttu-id="90d06-251">パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。</span><span class="sxs-lookup"><span data-stu-id="90d06-251">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="90d06-252">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="90d06-252">Valid values 0 to 24</span></span>|
|<span data-ttu-id="90d06-253">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="90d06-253">passwordRequiredType</span></span>|[<span data-ttu-id="90d06-254">androiddeviceownerrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="90d06-254">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="90d06-255">デバイスで必要なパスワードの最小品質を示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-255">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="90d06-256">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。</span><span class="sxs-lookup"><span data-stu-id="90d06-256">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="90d06-257">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="90d06-257">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="90d06-258">Int32</span><span class="sxs-lookup"><span data-stu-id="90d06-258">Int32</span></span>|<span data-ttu-id="90d06-259">ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-259">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="90d06-260">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="90d06-260">Valid values 4 to 11</span></span>|
|<span data-ttu-id="90d06-261">safebootblocked</span><span class="sxs-lookup"><span data-stu-id="90d06-261">safeBootBlocked</span></span>|<span data-ttu-id="90d06-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-262">Boolean</span></span>|<span data-ttu-id="90d06-263">セーフブートでのデバイスの再起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-263">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="90d06-264">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="90d06-264">screenCaptureBlocked</span></span>|<span data-ttu-id="90d06-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-265">Boolean</span></span>|<span data-ttu-id="90d06-266">スクリーンショットを撮影する機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-266">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="90d06-267">securityallowデバッグ機能</span><span class="sxs-lookup"><span data-stu-id="90d06-267">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="90d06-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-268">Boolean</span></span>|<span data-ttu-id="90d06-269">ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-269">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="90d06-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="90d06-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="90d06-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-271">Boolean</span></span>|<span data-ttu-id="90d06-272">アプリを確認する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-272">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="90d06-273">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="90d06-273">statusBarBlocked</span></span>|<span data-ttu-id="90d06-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-274">Boolean</span></span>|<span data-ttu-id="90d06-275">通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-275">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="90d06-276">stayonmodes</span><span class="sxs-lookup"><span data-stu-id="90d06-276">stayOnModes</span></span>|<span data-ttu-id="90d06-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="90d06-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="90d06-278">デバイスの表示がオンのままになるモードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="90d06-278">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="90d06-279">このコレクションには、最大4つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="90d06-279">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="90d06-280">可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。</span><span class="sxs-lookup"><span data-stu-id="90d06-280">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="90d06-281">storageallowusb</span><span class="sxs-lookup"><span data-stu-id="90d06-281">storageAllowUsb</span></span>|<span data-ttu-id="90d06-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-282">Boolean</span></span>|<span data-ttu-id="90d06-283">USB 大容量ストレージを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-283">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="90d06-284">storageblockexternalmedia</span><span class="sxs-lookup"><span data-stu-id="90d06-284">storageBlockExternalMedia</span></span>|<span data-ttu-id="90d06-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-285">Boolean</span></span>|<span data-ttu-id="90d06-286">外部メディアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-286">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="90d06-287">storageblockusbfiletransfer</span><span class="sxs-lookup"><span data-stu-id="90d06-287">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="90d06-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-288">Boolean</span></span>|<span data-ttu-id="90d06-289">USB ファイル転送をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-289">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="90d06-290">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="90d06-290">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="90d06-291">Int32</span><span class="sxs-lookup"><span data-stu-id="90d06-291">Int32</span></span>|<span data-ttu-id="90d06-292">[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-292">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="90d06-293">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="90d06-293">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="90d06-294">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="90d06-294">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="90d06-295">Int32</span><span class="sxs-lookup"><span data-stu-id="90d06-295">Int32</span></span>|<span data-ttu-id="90d06-296">[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-296">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="90d06-297">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="90d06-297">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="90d06-298">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="90d06-298">systemUpdateInstallType</span></span>|[<span data-ttu-id="90d06-299">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="90d06-299">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="90d06-300">システム更新構成の種類。</span><span class="sxs-lookup"><span data-stu-id="90d06-300">The type of system update configuration.</span></span> <span data-ttu-id="90d06-301">可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="90d06-301">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="90d06-302">systemwindowsblocked ブロック</span><span class="sxs-lookup"><span data-stu-id="90d06-302">systemWindowsBlocked</span></span>|<span data-ttu-id="90d06-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-303">Boolean</span></span>|<span data-ttu-id="90d06-304">Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="90d06-304">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="90d06-305">ユーザー blockadd</span><span class="sxs-lookup"><span data-stu-id="90d06-305">usersBlockAdd</span></span>|<span data-ttu-id="90d06-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-306">Boolean</span></span>|<span data-ttu-id="90d06-307">ユーザーおよびプロファイルの追加を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-307">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="90d06-308">ユーザー blockremove</span><span class="sxs-lookup"><span data-stu-id="90d06-308">usersBlockRemove</span></span>|<span data-ttu-id="90d06-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-309">Boolean</span></span>|<span data-ttu-id="90d06-310">他のユーザーのデバイスからの削除を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-310">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="90d06-311">volumeblockadjustment</span><span class="sxs-lookup"><span data-stu-id="90d06-311">volumeBlockAdjustment</span></span>|<span data-ttu-id="90d06-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-312">Boolean</span></span>|<span data-ttu-id="90d06-313">マスターボリュームを調整するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-313">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="90d06-314">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="90d06-314">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="90d06-315">String</span><span class="sxs-lookup"><span data-stu-id="90d06-315">String</span></span>|<span data-ttu-id="90d06-316">always on VPN 接続を処理するアプリの Android アプリパッケージ名。</span><span class="sxs-lookup"><span data-stu-id="90d06-316">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="90d06-317">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="90d06-317">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="90d06-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-318">Boolean</span></span>|<span data-ttu-id="90d06-319">always on vpn パッケージ名が指定されている場合は、vpn が切断されたときにネットワークトラフィックをロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="90d06-319">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="90d06-320">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="90d06-320">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="90d06-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-321">Boolean</span></span>|<span data-ttu-id="90d06-322">ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-322">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="90d06-323">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="90d06-323">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="90d06-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d06-324">Boolean</span></span>|<span data-ttu-id="90d06-325">ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90d06-325">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="90d06-326">応答</span><span class="sxs-lookup"><span data-stu-id="90d06-326">Response</span></span>
<span data-ttu-id="90d06-327">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="90d06-327">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90d06-328">例</span><span class="sxs-lookup"><span data-stu-id="90d06-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="90d06-329">要求</span><span class="sxs-lookup"><span data-stu-id="90d06-329">Request</span></span>
<span data-ttu-id="90d06-330">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90d06-330">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2517

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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

### <a name="response"></a><span data-ttu-id="90d06-331">応答</span><span class="sxs-lookup"><span data-stu-id="90d06-331">Response</span></span>
<span data-ttu-id="90d06-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90d06-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2689

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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




