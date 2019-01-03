---
title: AndroidDeviceOwnerGeneralDeviceConfiguration を作成します。
description: 新しい androidDeviceOwnerGeneralDeviceConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 404233f1c9eba62021b5ba019a9f3bb049c272c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333259"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="86f17-103">AndroidDeviceOwnerGeneralDeviceConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="86f17-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="86f17-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86f17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86f17-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86f17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86f17-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="86f17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86f17-107">新しい[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="86f17-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86f17-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="86f17-108">Prerequisites</span></span>
<span data-ttu-id="86f17-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86f17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86f17-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86f17-111">Permission type</span></span>|<span data-ttu-id="86f17-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="86f17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86f17-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86f17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86f17-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86f17-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86f17-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86f17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86f17-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86f17-116">Not supported.</span></span>|
|<span data-ttu-id="86f17-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86f17-117">Application</span></span>|<span data-ttu-id="86f17-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86f17-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86f17-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86f17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86f17-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86f17-120">Request headers</span></span>
|<span data-ttu-id="86f17-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86f17-121">Header</span></span>|<span data-ttu-id="86f17-122">値</span><span class="sxs-lookup"><span data-stu-id="86f17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86f17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86f17-123">Authorization</span></span>|<span data-ttu-id="86f17-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="86f17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86f17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86f17-125">Accept</span></span>|<span data-ttu-id="86f17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86f17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86f17-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="86f17-127">Request body</span></span>
<span data-ttu-id="86f17-128">要求の本文に androidDeviceOwnerGeneralDeviceConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="86f17-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="86f17-129">次の表は、androidDeviceOwnerGeneralDeviceConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="86f17-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86f17-130">Property</span></span>|<span data-ttu-id="86f17-131">種類</span><span class="sxs-lookup"><span data-stu-id="86f17-131">Type</span></span>|<span data-ttu-id="86f17-132">説明</span><span class="sxs-lookup"><span data-stu-id="86f17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86f17-133">ID</span><span class="sxs-lookup"><span data-stu-id="86f17-133">id</span></span>|<span data-ttu-id="86f17-134">String</span><span class="sxs-lookup"><span data-stu-id="86f17-134">String</span></span>|<span data-ttu-id="86f17-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="86f17-135">Key of the entity.</span></span> <span data-ttu-id="86f17-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86f17-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f17-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86f17-137">lastModifiedDateTime</span></span>|<span data-ttu-id="86f17-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86f17-138">DateTimeOffset</span></span>|<span data-ttu-id="86f17-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="86f17-139">DateTime the object was last modified.</span></span> <span data-ttu-id="86f17-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86f17-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f17-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86f17-141">roleScopeTagIds</span></span>|<span data-ttu-id="86f17-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="86f17-142">String collection</span></span>|<span data-ttu-id="86f17-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="86f17-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86f17-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86f17-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f17-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86f17-145">supportsScopeTags</span></span>|<span data-ttu-id="86f17-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-146">Boolean</span></span>|<span data-ttu-id="86f17-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86f17-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="86f17-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86f17-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="86f17-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86f17-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="86f17-150">This property is read-only.</span></span> <span data-ttu-id="86f17-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86f17-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f17-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86f17-152">createdDateTime</span></span>|<span data-ttu-id="86f17-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86f17-153">DateTimeOffset</span></span>|<span data-ttu-id="86f17-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="86f17-154">DateTime the object was created.</span></span> <span data-ttu-id="86f17-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86f17-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f17-156">説明</span><span class="sxs-lookup"><span data-stu-id="86f17-156">description</span></span>|<span data-ttu-id="86f17-157">String</span><span class="sxs-lookup"><span data-stu-id="86f17-157">String</span></span>|<span data-ttu-id="86f17-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="86f17-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86f17-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86f17-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f17-160">displayName</span><span class="sxs-lookup"><span data-stu-id="86f17-160">displayName</span></span>|<span data-ttu-id="86f17-161">String</span><span class="sxs-lookup"><span data-stu-id="86f17-161">String</span></span>|<span data-ttu-id="86f17-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="86f17-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86f17-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86f17-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f17-164">version</span><span class="sxs-lookup"><span data-stu-id="86f17-164">version</span></span>|<span data-ttu-id="86f17-165">Int32</span><span class="sxs-lookup"><span data-stu-id="86f17-165">Int32</span></span>|<span data-ttu-id="86f17-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="86f17-166">Version of the device configuration.</span></span> <span data-ttu-id="86f17-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="86f17-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f17-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="86f17-168">accountsBlockModification</span></span>|<span data-ttu-id="86f17-169">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-169">Boolean</span></span>|<span data-ttu-id="86f17-170">追加または削除、アカウントが無効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="86f17-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="86f17-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="86f17-172">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-172">Boolean</span></span>|<span data-ttu-id="86f17-173">不明なソースの設定を有効にするユーザーを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="86f17-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="86f17-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="86f17-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="86f17-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="86f17-176">アプリケーションの自動更新ポリシーの値を示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="86f17-177">可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。</span><span class="sxs-lookup"><span data-stu-id="86f17-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="86f17-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="86f17-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="86f17-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="86f17-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="86f17-180">いずれかが定義されていない場合、アプリケーションの具体的には、実行時のアクセス許可の要求のアクセス許可ポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="86f17-181">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="86f17-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="86f17-182">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="86f17-182">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="86f17-183">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-183">Boolean</span></span>|<span data-ttu-id="86f17-184">Bluetooth の構成からユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-184">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="86f17-185">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="86f17-185">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="86f17-186">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-186">Boolean</span></span>|<span data-ttu-id="86f17-187">Bluetooth を使用して連絡先の共有からユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-187">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="86f17-188">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="86f17-188">cameraBlocked</span></span>|<span data-ttu-id="86f17-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="86f17-189">Boolean</span></span>|<span data-ttu-id="86f17-190">カメラの使用を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-190">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="86f17-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="86f17-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="86f17-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="86f17-192">Boolean</span></span>|<span data-ttu-id="86f17-193">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-193">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="86f17-194">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="86f17-194">dataRoamingBlocked</span></span>|<span data-ttu-id="86f17-195">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-195">Boolean</span></span>|<span data-ttu-id="86f17-196">ユーザーによるデータの移動を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-196">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="86f17-197">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="86f17-197">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="86f17-198">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-198">Boolean</span></span>|<span data-ttu-id="86f17-199">日付またはデバイス上の時刻を手動で変更するからユーザーをブロックするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="86f17-199">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="86f17-200">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="86f17-200">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="86f17-201">String コレクション</span><span class="sxs-lookup"><span data-stu-id="86f17-201">String collection</span></span>|<span data-ttu-id="86f17-202">デバイスは、工場出荷時を設定する前にリセットした後に認証する必要があります Google アカウントのメールのリストです。</span><span class="sxs-lookup"><span data-stu-id="86f17-202">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="86f17-203">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="86f17-203">factoryResetBlocked</span></span>|<span data-ttu-id="86f17-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="86f17-204">Boolean</span></span>|<span data-ttu-id="86f17-205">設定の工場出荷時リセット ・ オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-205">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="86f17-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="86f17-206">kioskModeApps</span></span>|<span data-ttu-id="86f17-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="86f17-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="86f17-208">キオスク モードでは、デバイスに表示される管理対象のアプリケーションの一覧です。</span><span class="sxs-lookup"><span data-stu-id="86f17-208">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="86f17-209">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="86f17-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="86f17-210">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="86f17-210">microphoneForceMute</span></span>|<span data-ttu-id="86f17-211">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-211">Boolean</span></span>|<span data-ttu-id="86f17-212">Unmuting デバイスのマイクをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-212">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="86f17-213">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="86f17-213">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="86f17-214">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-214">Boolean</span></span>|<span data-ttu-id="86f17-215">デバイスがブート時に一時的なネットワーク接続への接続を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-215">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="86f17-216">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="86f17-216">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="86f17-217">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-217">Boolean</span></span>|<span data-ttu-id="86f17-218">NFC 送信ビームをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-218">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="86f17-219">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="86f17-219">passwordBlockKeyguard</span></span>|<span data-ttu-id="86f17-220">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-220">Boolean</span></span>|<span data-ttu-id="86f17-221">Keyguard が無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-221">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="86f17-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="86f17-222">passwordExpirationDays</span></span>|<span data-ttu-id="86f17-223">Int32</span><span class="sxs-lookup"><span data-stu-id="86f17-223">Int32</span></span>|<span data-ttu-id="86f17-224">期限が切れるし、新しいパスワードが必要になる前のパスワードを設定できる時間 (秒) の量を示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-224">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="86f17-225">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="86f17-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="86f17-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="86f17-226">passwordMinimumLength</span></span>|<span data-ttu-id="86f17-227">Int32</span><span class="sxs-lookup"><span data-stu-id="86f17-227">Int32</span></span>|<span data-ttu-id="86f17-228">デバイスに必要なパスワードの最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-228">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="86f17-229">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="86f17-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="86f17-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="86f17-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="86f17-231">Int32</span><span class="sxs-lookup"><span data-stu-id="86f17-231">Int32</span></span>|<span data-ttu-id="86f17-232">画面がタイムアウトするまで非アクティブのミリ秒です。</span><span class="sxs-lookup"><span data-stu-id="86f17-232">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="86f17-233">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="86f17-233">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="86f17-234">Int32</span><span class="sxs-lookup"><span data-stu-id="86f17-234">Int32</span></span>|<span data-ttu-id="86f17-235">場所ユーザーことはできませんが、履歴内の任意のパスワードと同じパスワードを入力するのには、パスワードの履歴の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-235">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="86f17-236">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="86f17-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="86f17-237">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="86f17-237">passwordRequiredType</span></span>|[<span data-ttu-id="86f17-238">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="86f17-238">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="86f17-239">デバイスに必要なパスワードの最小の品質を示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-239">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="86f17-240">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="86f17-240">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="86f17-241">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="86f17-241">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="86f17-242">Int32</span><span class="sxs-lookup"><span data-stu-id="86f17-242">Int32</span></span>|<span data-ttu-id="86f17-243">デバイスをワイプする前に、ユーザーが誤ったパスワードを入力できる回数を示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-243">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="86f17-244">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="86f17-244">Valid values 4 to 11</span></span>|
|<span data-ttu-id="86f17-245">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="86f17-245">safeBootBlocked</span></span>|<span data-ttu-id="86f17-246">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-246">Boolean</span></span>|<span data-ttu-id="86f17-247">セーフ ブート デバイスが無効になってを再起動するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-247">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="86f17-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="86f17-248">screenCaptureBlocked</span></span>|<span data-ttu-id="86f17-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="86f17-249">Boolean</span></span>|<span data-ttu-id="86f17-250">スクリーン ショットを実行する機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-250">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="86f17-251">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="86f17-251">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="86f17-252">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-252">Boolean</span></span>|<span data-ttu-id="86f17-253">デバイスのデバッグ機能を有効にすることからユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-253">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="86f17-254">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="86f17-254">securityRequireVerifyApps</span></span>|<span data-ttu-id="86f17-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="86f17-255">Boolean</span></span>|<span data-ttu-id="86f17-256">示しているかどうかのアプリケーションが必要なことを確認します。</span><span class="sxs-lookup"><span data-stu-id="86f17-256">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="86f17-257">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="86f17-257">statusBarBlocked</span></span>|<span data-ttu-id="86f17-258">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-258">Boolean</span></span>|<span data-ttu-id="86f17-259">示すかどうか、またはステータス バーを無効に、通知、すばやく設定およびその他の画面のオーバーレイを含みます。</span><span class="sxs-lookup"><span data-stu-id="86f17-259">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="86f17-260">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="86f17-260">stayOnModes</span></span>|<span data-ttu-id="86f17-261">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="86f17-261">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="86f17-262">デバイスの表示が残ります電源モードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="86f17-262">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="86f17-263">このコレクションには、最大 4 つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="86f17-263">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="86f17-264">可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。</span><span class="sxs-lookup"><span data-stu-id="86f17-264">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="86f17-265">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="86f17-265">storageAllowUsb</span></span>|<span data-ttu-id="86f17-266">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-266">Boolean</span></span>|<span data-ttu-id="86f17-267">USB 大容量記憶装置を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-267">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="86f17-268">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="86f17-268">storageBlockExternalMedia</span></span>|<span data-ttu-id="86f17-269">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-269">Boolean</span></span>|<span data-ttu-id="86f17-270">外部メディアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-270">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="86f17-271">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="86f17-271">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="86f17-272">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-272">Boolean</span></span>|<span data-ttu-id="86f17-273">USB ファイル転送をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-273">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="86f17-274">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="86f17-274">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="86f17-275">Int32</span><span class="sxs-lookup"><span data-stu-id="86f17-275">Int32</span></span>|<span data-ttu-id="86f17-276">システム更新プログラムの開始を午前 0 時以降後の分単位の数を示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-276">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="86f17-277">有効な値の 0 から 1440</span><span class="sxs-lookup"><span data-stu-id="86f17-277">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="86f17-278">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="86f17-278">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="86f17-279">Int32</span><span class="sxs-lookup"><span data-stu-id="86f17-279">Int32</span></span>|<span data-ttu-id="86f17-280">システムの更新] ウィンドウを終了する午前 0 時以降後の分単位の数を示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-280">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="86f17-281">有効な値の 0 から 1440</span><span class="sxs-lookup"><span data-stu-id="86f17-281">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="86f17-282">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="86f17-282">systemUpdateInstallType</span></span>|[<span data-ttu-id="86f17-283">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="86f17-283">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="86f17-284">システム更新の構成の型。</span><span class="sxs-lookup"><span data-stu-id="86f17-284">The type of system update configuration.</span></span> <span data-ttu-id="86f17-285">可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="86f17-285">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="86f17-286">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="86f17-286">usersBlockAdd</span></span>|<span data-ttu-id="86f17-287">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-287">Boolean</span></span>|<span data-ttu-id="86f17-288">ユーザーとプロファイルを追加することが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-288">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="86f17-289">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="86f17-289">usersBlockRemove</span></span>|<span data-ttu-id="86f17-290">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-290">Boolean</span></span>|<span data-ttu-id="86f17-291">デバイスから他のユーザーを削除するを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-291">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="86f17-292">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="86f17-292">volumeBlockAdjustment</span></span>|<span data-ttu-id="86f17-293">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-293">Boolean</span></span>|<span data-ttu-id="86f17-294">マスター ボリュームが無効になっているを調整するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-294">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="86f17-295">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="86f17-295">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="86f17-296">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-296">Boolean</span></span>|<span data-ttu-id="86f17-297">Wifi 接続の設定を編集することからユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-297">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="86f17-298">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="86f17-298">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="86f17-299">ブール型</span><span class="sxs-lookup"><span data-stu-id="86f17-299">Boolean</span></span>|<span data-ttu-id="86f17-300">ポリシーで定義されているネットワークだけを編集するユーザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="86f17-300">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="86f17-301">応答</span><span class="sxs-lookup"><span data-stu-id="86f17-301">Response</span></span>
<span data-ttu-id="86f17-302">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="86f17-302">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86f17-303">例</span><span class="sxs-lookup"><span data-stu-id="86f17-303">Example</span></span>
### <a name="request"></a><span data-ttu-id="86f17-304">要求</span><span class="sxs-lookup"><span data-stu-id="86f17-304">Request</span></span>
<span data-ttu-id="86f17-305">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86f17-305">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2156

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="86f17-306">応答</span><span class="sxs-lookup"><span data-stu-id="86f17-306">Response</span></span>
<span data-ttu-id="86f17-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86f17-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2264

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




