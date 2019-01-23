---
title: AndroidDeviceOwnerGeneralDeviceConfiguration を作成します。
description: 新しい androidDeviceOwnerGeneralDeviceConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93df53db7c19df9134370f9dbd703d99f631b688
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421222"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="062df-103">AndroidDeviceOwnerGeneralDeviceConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="062df-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="062df-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="062df-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="062df-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="062df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="062df-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="062df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="062df-107">新しい[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="062df-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="062df-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="062df-108">Prerequisites</span></span>
<span data-ttu-id="062df-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="062df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="062df-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="062df-111">Permission type</span></span>|<span data-ttu-id="062df-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="062df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="062df-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="062df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="062df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="062df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="062df-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="062df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="062df-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="062df-116">Not supported.</span></span>|
|<span data-ttu-id="062df-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="062df-117">Application</span></span>|<span data-ttu-id="062df-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="062df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="062df-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="062df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="062df-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="062df-120">Request headers</span></span>
|<span data-ttu-id="062df-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="062df-121">Header</span></span>|<span data-ttu-id="062df-122">値</span><span class="sxs-lookup"><span data-stu-id="062df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="062df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="062df-123">Authorization</span></span>|<span data-ttu-id="062df-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="062df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="062df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="062df-125">Accept</span></span>|<span data-ttu-id="062df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="062df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="062df-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="062df-127">Request body</span></span>
<span data-ttu-id="062df-128">要求の本文に androidDeviceOwnerGeneralDeviceConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="062df-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="062df-129">次の表は、androidDeviceOwnerGeneralDeviceConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="062df-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="062df-130">Property</span></span>|<span data-ttu-id="062df-131">型</span><span class="sxs-lookup"><span data-stu-id="062df-131">Type</span></span>|<span data-ttu-id="062df-132">説明</span><span class="sxs-lookup"><span data-stu-id="062df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="062df-133">id</span><span class="sxs-lookup"><span data-stu-id="062df-133">id</span></span>|<span data-ttu-id="062df-134">String</span><span class="sxs-lookup"><span data-stu-id="062df-134">String</span></span>|<span data-ttu-id="062df-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="062df-135">Key of the entity.</span></span> <span data-ttu-id="062df-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="062df-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="062df-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="062df-137">lastModifiedDateTime</span></span>|<span data-ttu-id="062df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="062df-138">DateTimeOffset</span></span>|<span data-ttu-id="062df-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="062df-139">DateTime the object was last modified.</span></span> <span data-ttu-id="062df-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="062df-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="062df-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="062df-141">roleScopeTagIds</span></span>|<span data-ttu-id="062df-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="062df-142">String collection</span></span>|<span data-ttu-id="062df-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="062df-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="062df-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="062df-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="062df-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="062df-145">supportsScopeTags</span></span>|<span data-ttu-id="062df-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-146">Boolean</span></span>|<span data-ttu-id="062df-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="062df-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="062df-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="062df-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="062df-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="062df-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="062df-150">This property is read-only.</span></span> <span data-ttu-id="062df-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="062df-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="062df-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="062df-152">createdDateTime</span></span>|<span data-ttu-id="062df-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="062df-153">DateTimeOffset</span></span>|<span data-ttu-id="062df-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="062df-154">DateTime the object was created.</span></span> <span data-ttu-id="062df-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="062df-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="062df-156">説明</span><span class="sxs-lookup"><span data-stu-id="062df-156">description</span></span>|<span data-ttu-id="062df-157">String</span><span class="sxs-lookup"><span data-stu-id="062df-157">String</span></span>|<span data-ttu-id="062df-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="062df-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="062df-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="062df-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="062df-160">displayName</span><span class="sxs-lookup"><span data-stu-id="062df-160">displayName</span></span>|<span data-ttu-id="062df-161">String</span><span class="sxs-lookup"><span data-stu-id="062df-161">String</span></span>|<span data-ttu-id="062df-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="062df-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="062df-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="062df-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="062df-164">version</span><span class="sxs-lookup"><span data-stu-id="062df-164">version</span></span>|<span data-ttu-id="062df-165">Int32</span><span class="sxs-lookup"><span data-stu-id="062df-165">Int32</span></span>|<span data-ttu-id="062df-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="062df-166">Version of the device configuration.</span></span> <span data-ttu-id="062df-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="062df-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="062df-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="062df-168">accountsBlockModification</span></span>|<span data-ttu-id="062df-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-169">Boolean</span></span>|<span data-ttu-id="062df-170">追加または削除、アカウントが無効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="062df-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="062df-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="062df-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-172">Boolean</span></span>|<span data-ttu-id="062df-173">不明なソースの設定を有効にするユーザーを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="062df-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="062df-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="062df-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="062df-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="062df-176">アプリケーションの自動更新ポリシーの値を示します。</span><span class="sxs-lookup"><span data-stu-id="062df-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="062df-177">可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。</span><span class="sxs-lookup"><span data-stu-id="062df-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="062df-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="062df-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="062df-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="062df-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="062df-180">いずれかが定義されていない場合、アプリケーションの具体的には、実行時のアクセス許可の要求のアクセス許可ポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="062df-181">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="062df-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="062df-182">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="062df-182">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="062df-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-183">Boolean</span></span>|<span data-ttu-id="062df-184">すべてのアプリケーションをお勧めするかどうかは、追加可能性があります、最初の時間の使用のヒントをスキップします。</span><span class="sxs-lookup"><span data-stu-id="062df-184">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="062df-185">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="062df-185">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="062df-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-186">Boolean</span></span>|<span data-ttu-id="062df-187">Bluetooth の構成からユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-187">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="062df-188">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="062df-188">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="062df-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-189">Boolean</span></span>|<span data-ttu-id="062df-190">Bluetooth を使用して連絡先の共有からユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-190">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="062df-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="062df-191">cameraBlocked</span></span>|<span data-ttu-id="062df-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-192">Boolean</span></span>|<span data-ttu-id="062df-193">カメラの使用を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-193">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="062df-194">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="062df-194">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="062df-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-195">Boolean</span></span>|<span data-ttu-id="062df-196">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-196">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="062df-197">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="062df-197">dataRoamingBlocked</span></span>|<span data-ttu-id="062df-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-198">Boolean</span></span>|<span data-ttu-id="062df-199">ユーザーによるデータの移動を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-199">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="062df-200">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="062df-200">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="062df-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-201">Boolean</span></span>|<span data-ttu-id="062df-202">日付またはデバイス上の時刻を手動で変更するからユーザーをブロックするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="062df-202">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="062df-203">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="062df-203">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="062df-204">String コレクション</span><span class="sxs-lookup"><span data-stu-id="062df-204">String collection</span></span>|<span data-ttu-id="062df-205">デバイスは、工場出荷時を設定する前にリセットした後に認証する必要があります Google アカウントのメールのリストです。</span><span class="sxs-lookup"><span data-stu-id="062df-205">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="062df-206">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="062df-206">factoryResetBlocked</span></span>|<span data-ttu-id="062df-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-207">Boolean</span></span>|<span data-ttu-id="062df-208">設定の工場出荷時リセット ・ オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-208">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="062df-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="062df-209">kioskModeApps</span></span>|<span data-ttu-id="062df-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="062df-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="062df-211">キオスク モードでは、デバイスに表示される管理対象のアプリケーションの一覧です。</span><span class="sxs-lookup"><span data-stu-id="062df-211">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="062df-212">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="062df-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="062df-213">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="062df-213">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="062df-214">String</span><span class="sxs-lookup"><span data-stu-id="062df-214">String</span></span>|<span data-ttu-id="062df-215">キオスク モードでは、デバイスとは、壁紙に使用するパブリックにアクセス可能なイメージの URL。</span><span class="sxs-lookup"><span data-stu-id="062df-215">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="062df-216">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="062df-216">kioskModeExitCode</span></span>|<span data-ttu-id="062df-217">String</span><span class="sxs-lookup"><span data-stu-id="062df-217">String</span></span>|<span data-ttu-id="062df-218">ユーザーがキオスク モードでは、デバイスとは、キオスク モードからエスケープできるようにするためのコードを終了します。</span><span class="sxs-lookup"><span data-stu-id="062df-218">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="062df-219">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="062df-219">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="062df-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-220">Boolean</span></span>|<span data-ttu-id="062df-221">キオスク モードでは、デバイスと仮想のホーム ボタンを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="062df-221">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="062df-222">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="062df-222">microphoneForceMute</span></span>|<span data-ttu-id="062df-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-223">Boolean</span></span>|<span data-ttu-id="062df-224">Unmuting デバイスのマイクをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-224">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="062df-225">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="062df-225">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="062df-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-226">Boolean</span></span>|<span data-ttu-id="062df-227">デバイスがブート時に一時的なネットワーク接続への接続を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-227">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="062df-228">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="062df-228">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="062df-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-229">Boolean</span></span>|<span data-ttu-id="062df-230">NFC 送信ビームをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-230">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="062df-231">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="062df-231">passwordBlockKeyguard</span></span>|<span data-ttu-id="062df-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-232">Boolean</span></span>|<span data-ttu-id="062df-233">Keyguard が無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-233">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="062df-234">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="062df-234">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="062df-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="062df-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="062df-236">ブロックするデバイスの keyguard の機能の一覧です。</span><span class="sxs-lookup"><span data-stu-id="062df-236">List of device keyguard features to block.</span></span> <span data-ttu-id="062df-237">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="062df-237">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="062df-238">可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。</span><span class="sxs-lookup"><span data-stu-id="062df-238">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="062df-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="062df-239">passwordExpirationDays</span></span>|<span data-ttu-id="062df-240">Int32</span><span class="sxs-lookup"><span data-stu-id="062df-240">Int32</span></span>|<span data-ttu-id="062df-241">期限が切れるし、新しいパスワードが必要になる前のパスワードを設定できる時間 (秒) の量を示します。</span><span class="sxs-lookup"><span data-stu-id="062df-241">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="062df-242">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="062df-242">Valid values 1 to 365</span></span>|
|<span data-ttu-id="062df-243">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="062df-243">passwordMinimumLength</span></span>|<span data-ttu-id="062df-244">Int32</span><span class="sxs-lookup"><span data-stu-id="062df-244">Int32</span></span>|<span data-ttu-id="062df-245">デバイスに必要なパスワードの最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-245">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="062df-246">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="062df-246">Valid values 4 to 16</span></span>|
|<span data-ttu-id="062df-247">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="062df-247">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="062df-248">Int32</span><span class="sxs-lookup"><span data-stu-id="062df-248">Int32</span></span>|<span data-ttu-id="062df-249">画面がタイムアウトするまで非アクティブのミリ秒です。</span><span class="sxs-lookup"><span data-stu-id="062df-249">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="062df-250">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="062df-250">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="062df-251">Int32</span><span class="sxs-lookup"><span data-stu-id="062df-251">Int32</span></span>|<span data-ttu-id="062df-252">場所ユーザーことはできませんが、履歴内の任意のパスワードと同じパスワードを入力するのには、パスワードの履歴の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-252">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="062df-253">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="062df-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="062df-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="062df-254">passwordRequiredType</span></span>|[<span data-ttu-id="062df-255">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="062df-255">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="062df-256">デバイスに必要なパスワードの最小の品質を示します。</span><span class="sxs-lookup"><span data-stu-id="062df-256">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="062df-257">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="062df-257">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="062df-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="062df-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="062df-259">Int32</span><span class="sxs-lookup"><span data-stu-id="062df-259">Int32</span></span>|<span data-ttu-id="062df-260">デバイスをワイプする前に、ユーザーが誤ったパスワードを入力できる回数を示します。</span><span class="sxs-lookup"><span data-stu-id="062df-260">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="062df-261">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="062df-261">Valid values 4 to 11</span></span>|
|<span data-ttu-id="062df-262">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="062df-262">safeBootBlocked</span></span>|<span data-ttu-id="062df-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-263">Boolean</span></span>|<span data-ttu-id="062df-264">セーフ ブート デバイスが無効になってを再起動するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-264">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="062df-265">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="062df-265">screenCaptureBlocked</span></span>|<span data-ttu-id="062df-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-266">Boolean</span></span>|<span data-ttu-id="062df-267">スクリーン ショットを実行する機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-267">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="062df-268">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="062df-268">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="062df-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-269">Boolean</span></span>|<span data-ttu-id="062df-270">デバイスのデバッグ機能を有効にすることからユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-270">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="062df-271">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="062df-271">securityRequireVerifyApps</span></span>|<span data-ttu-id="062df-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-272">Boolean</span></span>|<span data-ttu-id="062df-273">示しているかどうかのアプリケーションが必要なことを確認します。</span><span class="sxs-lookup"><span data-stu-id="062df-273">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="062df-274">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="062df-274">statusBarBlocked</span></span>|<span data-ttu-id="062df-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-275">Boolean</span></span>|<span data-ttu-id="062df-276">示すかどうか、またはステータス バーを無効に、通知、すばやく設定およびその他の画面のオーバーレイを含みます。</span><span class="sxs-lookup"><span data-stu-id="062df-276">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="062df-277">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="062df-277">stayOnModes</span></span>|<span data-ttu-id="062df-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="062df-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="062df-279">デバイスの表示が残ります電源モードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="062df-279">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="062df-280">このコレクションには、最大 4 つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="062df-280">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="062df-281">可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。</span><span class="sxs-lookup"><span data-stu-id="062df-281">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="062df-282">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="062df-282">storageAllowUsb</span></span>|<span data-ttu-id="062df-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-283">Boolean</span></span>|<span data-ttu-id="062df-284">USB 大容量記憶装置を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-284">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="062df-285">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="062df-285">storageBlockExternalMedia</span></span>|<span data-ttu-id="062df-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-286">Boolean</span></span>|<span data-ttu-id="062df-287">外部メディアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-287">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="062df-288">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="062df-288">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="062df-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-289">Boolean</span></span>|<span data-ttu-id="062df-290">USB ファイル転送をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-290">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="062df-291">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="062df-291">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="062df-292">Int32</span><span class="sxs-lookup"><span data-stu-id="062df-292">Int32</span></span>|<span data-ttu-id="062df-293">システム更新プログラムの開始を午前 0 時以降後の分単位の数を示します。</span><span class="sxs-lookup"><span data-stu-id="062df-293">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="062df-294">有効な値の 0 から 1440</span><span class="sxs-lookup"><span data-stu-id="062df-294">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="062df-295">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="062df-295">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="062df-296">Int32</span><span class="sxs-lookup"><span data-stu-id="062df-296">Int32</span></span>|<span data-ttu-id="062df-297">システムの更新] ウィンドウを終了する午前 0 時以降後の分単位の数を示します。</span><span class="sxs-lookup"><span data-stu-id="062df-297">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="062df-298">有効な値の 0 から 1440</span><span class="sxs-lookup"><span data-stu-id="062df-298">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="062df-299">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="062df-299">systemUpdateInstallType</span></span>|[<span data-ttu-id="062df-300">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="062df-300">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="062df-301">システム更新の構成の型。</span><span class="sxs-lookup"><span data-stu-id="062df-301">The type of system update configuration.</span></span> <span data-ttu-id="062df-302">可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="062df-302">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="062df-303">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="062df-303">systemWindowsBlocked</span></span>|<span data-ttu-id="062df-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-304">Boolean</span></span>|<span data-ttu-id="062df-305">Android システムをブロックするかどうかは、toasts、電話活動、およびシステムの警告のように、windows を確認します。</span><span class="sxs-lookup"><span data-stu-id="062df-305">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="062df-306">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="062df-306">usersBlockAdd</span></span>|<span data-ttu-id="062df-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-307">Boolean</span></span>|<span data-ttu-id="062df-308">ユーザーとプロファイルを追加することが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-308">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="062df-309">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="062df-309">usersBlockRemove</span></span>|<span data-ttu-id="062df-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-310">Boolean</span></span>|<span data-ttu-id="062df-311">デバイスから他のユーザーを削除するを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-311">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="062df-312">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="062df-312">volumeBlockAdjustment</span></span>|<span data-ttu-id="062df-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-313">Boolean</span></span>|<span data-ttu-id="062df-314">マスター ボリュームが無効になっているを調整するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-314">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="062df-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="062df-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="062df-316">String</span><span class="sxs-lookup"><span data-stu-id="062df-316">String</span></span>|<span data-ttu-id="062df-317">常時接続で VPN 接続を処理するアプリケーションの android アプリのパッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="062df-317">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="062df-318">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="062df-318">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="062df-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-319">Boolean</span></span>|<span data-ttu-id="062df-320">常にオンの VPN は、パッケージの名前は指定、かどうか、その VPN が切断されたときに、ネットワーク トラフィックをロックされます。</span><span class="sxs-lookup"><span data-stu-id="062df-320">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="062df-321">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="062df-321">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="062df-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-322">Boolean</span></span>|<span data-ttu-id="062df-323">Wifi 接続の設定を編集することからユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-323">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="062df-324">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="062df-324">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="062df-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="062df-325">Boolean</span></span>|<span data-ttu-id="062df-326">ポリシーで定義されているネットワークだけを編集するユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="062df-326">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="062df-327">応答</span><span class="sxs-lookup"><span data-stu-id="062df-327">Response</span></span>
<span data-ttu-id="062df-328">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="062df-328">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="062df-329">例</span><span class="sxs-lookup"><span data-stu-id="062df-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="062df-330">要求</span><span class="sxs-lookup"><span data-stu-id="062df-330">Request</span></span>
<span data-ttu-id="062df-331">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="062df-331">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="062df-332">応答</span><span class="sxs-lookup"><span data-stu-id="062df-332">Response</span></span>
<span data-ttu-id="062df-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="062df-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




