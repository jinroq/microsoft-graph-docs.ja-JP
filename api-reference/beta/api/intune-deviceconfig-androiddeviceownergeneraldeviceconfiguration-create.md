---
title: Androiddeviceowner一般の Devic/デバイスの作成
description: 新しい Androiddeviceowner一般の Devic/デバイスオブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16ba295955cc32f932612c5d2d4007ffedca46af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971431"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="b6861-103">Androiddeviceowner一般の Devic/デバイスの作成</span><span class="sxs-lookup"><span data-stu-id="b6861-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b6861-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6861-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6861-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6861-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6861-106">新しい[Androiddeviceowner一般の Devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b6861-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6861-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6861-107">Prerequisites</span></span>
<span data-ttu-id="b6861-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6861-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6861-110">Permission type</span></span>|<span data-ttu-id="b6861-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6861-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6861-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6861-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6861-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6861-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6861-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6861-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6861-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6861-115">Not supported.</span></span>|
|<span data-ttu-id="b6861-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6861-116">Application</span></span>|<span data-ttu-id="b6861-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6861-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6861-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6861-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b6861-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6861-119">Request headers</span></span>
|<span data-ttu-id="b6861-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6861-120">Header</span></span>|<span data-ttu-id="b6861-121">値</span><span class="sxs-lookup"><span data-stu-id="b6861-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6861-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6861-122">Authorization</span></span>|<span data-ttu-id="b6861-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6861-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6861-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b6861-124">Accept</span></span>|<span data-ttu-id="b6861-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6861-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6861-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6861-126">Request body</span></span>
<span data-ttu-id="b6861-127">要求本文で、Androiddeviceowner一般の Devic/devicオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6861-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="b6861-128">次の表に、Androiddeviceowner[Devic] の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="b6861-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6861-129">Property</span></span>|<span data-ttu-id="b6861-130">型</span><span class="sxs-lookup"><span data-stu-id="b6861-130">Type</span></span>|<span data-ttu-id="b6861-131">説明</span><span class="sxs-lookup"><span data-stu-id="b6861-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6861-132">id</span><span class="sxs-lookup"><span data-stu-id="b6861-132">id</span></span>|<span data-ttu-id="b6861-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b6861-133">String</span></span>|<span data-ttu-id="b6861-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b6861-134">Key of the entity.</span></span> <span data-ttu-id="b6861-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6861-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b6861-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6861-137">DateTimeOffset</span></span>|<span data-ttu-id="b6861-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b6861-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b6861-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6861-140">roleScopeTagIds</span></span>|<span data-ttu-id="b6861-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b6861-141">String collection</span></span>|<span data-ttu-id="b6861-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b6861-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6861-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b6861-144">supportsScopeTags</span></span>|<span data-ttu-id="b6861-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-145">Boolean</span></span>|<span data-ttu-id="b6861-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b6861-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="b6861-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b6861-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="b6861-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b6861-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="b6861-149">This property is read-only.</span></span> <span data-ttu-id="b6861-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b6861-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b6861-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b6861-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b6861-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="b6861-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b6861-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b6861-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b6861-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b6861-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b6861-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b6861-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b6861-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b6861-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b6861-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b6861-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b6861-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b6861-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b6861-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6861-163">createdDateTime</span></span>|<span data-ttu-id="b6861-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6861-164">DateTimeOffset</span></span>|<span data-ttu-id="b6861-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b6861-165">DateTime the object was created.</span></span> <span data-ttu-id="b6861-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-167">description</span><span class="sxs-lookup"><span data-stu-id="b6861-167">description</span></span>|<span data-ttu-id="b6861-168">String</span><span class="sxs-lookup"><span data-stu-id="b6861-168">String</span></span>|<span data-ttu-id="b6861-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b6861-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6861-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b6861-171">displayName</span></span>|<span data-ttu-id="b6861-172">String</span><span class="sxs-lookup"><span data-stu-id="b6861-172">String</span></span>|<span data-ttu-id="b6861-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b6861-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6861-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-175">version</span><span class="sxs-lookup"><span data-stu-id="b6861-175">version</span></span>|<span data-ttu-id="b6861-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-176">Int32</span></span>|<span data-ttu-id="b6861-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b6861-177">Version of the device configuration.</span></span> <span data-ttu-id="b6861-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6861-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6861-179">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="b6861-179">accountsBlockModification</span></span>|<span data-ttu-id="b6861-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-180">Boolean</span></span>|<span data-ttu-id="b6861-181">アカウントの追加または削除が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="b6861-182">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b6861-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="b6861-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-183">Boolean</span></span>|<span data-ttu-id="b6861-184">ユーザーが不明なソースを有効にできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="b6861-185">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="b6861-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="b6861-186">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="b6861-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="b6861-187">アプリの自動更新ポリシーの値を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="b6861-188">可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。</span><span class="sxs-lookup"><span data-stu-id="b6861-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="b6861-189">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="b6861-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="b6861-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="b6861-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="b6861-191">アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="b6861-192">使用可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="b6861-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="b6861-193">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="b6861-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="b6861-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-194">Boolean</span></span>|<span data-ttu-id="b6861-195">すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6861-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="b6861-196">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6861-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="b6861-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-197">Boolean</span></span>|<span data-ttu-id="b6861-198">ユーザーが bluetooth を構成することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="b6861-199">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="b6861-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="b6861-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-200">Boolean</span></span>|<span data-ttu-id="b6861-201">ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="b6861-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b6861-202">cameraBlocked</span></span>|<span data-ttu-id="b6861-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-203">Boolean</span></span>|<span data-ttu-id="b6861-204">カメラの使用を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="b6861-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="b6861-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="b6861-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-206">Boolean</span></span>|<span data-ttu-id="b6861-207">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="b6861-208">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="b6861-208">dataRoamingBlocked</span></span>|<span data-ttu-id="b6861-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-209">Boolean</span></span>|<span data-ttu-id="b6861-210">ユーザーのデータ移動を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-210">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="b6861-211">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="b6861-211">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="b6861-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-212">Boolean</span></span>|<span data-ttu-id="b6861-213">ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-213">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="b6861-214">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="b6861-214">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="b6861-215">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b6861-215">String collection</span></span>|<span data-ttu-id="b6861-216">デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。</span><span class="sxs-lookup"><span data-stu-id="b6861-216">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="b6861-217">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="b6861-217">factoryResetBlocked</span></span>|<span data-ttu-id="b6861-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-218">Boolean</span></span>|<span data-ttu-id="b6861-219">設定の出荷時のリセットオプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-219">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="b6861-220">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="b6861-220">kioskModeApps</span></span>|<span data-ttu-id="b6861-221">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b6861-221">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b6861-222">デバイスがキオスクモードのときに表示される管理対象アプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="b6861-222">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="b6861-223">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b6861-223">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b6861-224">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="b6861-224">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="b6861-225">String</span><span class="sxs-lookup"><span data-stu-id="b6861-225">String</span></span>|<span data-ttu-id="b6861-226">デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。</span><span class="sxs-lookup"><span data-stu-id="b6861-226">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="b6861-227">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="b6861-227">kioskModeExitCode</span></span>|<span data-ttu-id="b6861-228">String</span><span class="sxs-lookup"><span data-stu-id="b6861-228">String</span></span>|<span data-ttu-id="b6861-229">デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。</span><span class="sxs-lookup"><span data-stu-id="b6861-229">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="b6861-230">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="b6861-230">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="b6861-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-231">Boolean</span></span>|<span data-ttu-id="b6861-232">デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6861-232">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="b6861-233">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="b6861-233">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="b6861-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-234">Boolean</span></span>|<span data-ttu-id="b6861-235">ユーザーがキオスクモードで Bluetooth 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6861-235">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="b6861-236">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="b6861-236">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="b6861-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-237">Boolean</span></span>|<span data-ttu-id="b6861-238">ユーザーがキオスクモードで Wi-fi 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6861-238">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="b6861-239">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="b6861-239">microphoneForceMute</span></span>|<span data-ttu-id="b6861-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-240">Boolean</span></span>|<span data-ttu-id="b6861-241">デバイス上でのマイクのミュートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-241">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="b6861-242">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="b6861-242">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="b6861-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-243">Boolean</span></span>|<span data-ttu-id="b6861-244">ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-244">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="b6861-245">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="b6861-245">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="b6861-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-246">Boolean</span></span>|<span data-ttu-id="b6861-247">NFC の送信ビームをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-247">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="b6861-248">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="b6861-248">passwordBlockKeyguard</span></span>|<span data-ttu-id="b6861-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-249">Boolean</span></span>|<span data-ttu-id="b6861-250">Keyguard が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-250">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="b6861-251">Passwordblockkeygu/機能</span><span class="sxs-lookup"><span data-stu-id="b6861-251">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="b6861-252">[Androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6861-252">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="b6861-253">ブロックする device keyguard 機能のリストです。</span><span class="sxs-lookup"><span data-stu-id="b6861-253">List of device keyguard features to block.</span></span> <span data-ttu-id="b6861-254">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b6861-254">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="b6861-255">可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。</span><span class="sxs-lookup"><span data-stu-id="b6861-255">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="b6861-256">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b6861-256">passwordExpirationDays</span></span>|<span data-ttu-id="b6861-257">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-257">Int32</span></span>|<span data-ttu-id="b6861-258">パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6861-258">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="b6861-259">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="b6861-259">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b6861-260">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b6861-260">passwordMinimumLength</span></span>|<span data-ttu-id="b6861-261">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-261">Int32</span></span>|<span data-ttu-id="b6861-262">デバイスで必要なパスワードの最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-262">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="b6861-263">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="b6861-263">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b6861-264">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="b6861-264">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="b6861-265">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-265">Int32</span></span>|<span data-ttu-id="b6861-266">デバイスパスワードに必要な文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-266">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="b6861-267">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="b6861-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6861-268">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="b6861-268">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="b6861-269">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-269">Int32</span></span>|<span data-ttu-id="b6861-270">デバイスパスワードに必要な小文字の最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-270">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="b6861-271">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="b6861-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6861-272">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="b6861-272">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="b6861-273">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-273">Int32</span></span>|<span data-ttu-id="b6861-274">デバイスパスワードに必要な文字以外の文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-274">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="b6861-275">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="b6861-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6861-276">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="b6861-276">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="b6861-277">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-277">Int32</span></span>|<span data-ttu-id="b6861-278">デバイスパスワードに必要な最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-278">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="b6861-279">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="b6861-279">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6861-280">Passwordminimumシンボル文字</span><span class="sxs-lookup"><span data-stu-id="b6861-280">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="b6861-281">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-281">Int32</span></span>|<span data-ttu-id="b6861-282">デバイスパスワードに必要な最小記号文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-282">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="b6861-283">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="b6861-283">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6861-284">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="b6861-284">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="b6861-285">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-285">Int32</span></span>|<span data-ttu-id="b6861-286">デバイスのパスワードに必要な上位 caseletter 文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-286">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="b6861-287">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="b6861-287">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6861-288">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b6861-288">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b6861-289">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-289">Int32</span></span>|<span data-ttu-id="b6861-290">画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。</span><span class="sxs-lookup"><span data-stu-id="b6861-290">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b6861-291">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="b6861-291">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="b6861-292">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-292">Int32</span></span>|<span data-ttu-id="b6861-293">パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。</span><span class="sxs-lookup"><span data-stu-id="b6861-293">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="b6861-294">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="b6861-294">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b6861-295">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b6861-295">passwordRequiredType</span></span>|[<span data-ttu-id="b6861-296">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b6861-296">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="b6861-297">デバイスで必要なパスワードの最小品質を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-297">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="b6861-298">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。</span><span class="sxs-lookup"><span data-stu-id="b6861-298">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="b6861-299">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b6861-299">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b6861-300">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-300">Int32</span></span>|<span data-ttu-id="b6861-301">ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-301">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="b6861-302">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="b6861-302">Valid values 4 to 11</span></span>|
|<span data-ttu-id="b6861-303">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="b6861-303">playStoreMode</span></span>|[<span data-ttu-id="b6861-304">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="b6861-304">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="b6861-305">デバイスの再生ストアモードを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-305">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="b6861-306">可能な値は、`notConfigured`、`allowList`、`blockList` です。</span><span class="sxs-lookup"><span data-stu-id="b6861-306">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="b6861-307">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="b6861-307">safeBootBlocked</span></span>|<span data-ttu-id="b6861-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-308">Boolean</span></span>|<span data-ttu-id="b6861-309">セーフブートでのデバイスの再起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-309">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="b6861-310">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b6861-310">screenCaptureBlocked</span></span>|<span data-ttu-id="b6861-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-311">Boolean</span></span>|<span data-ttu-id="b6861-312">スクリーンショットを撮影する機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-312">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="b6861-313">Securityallowデバッグ機能</span><span class="sxs-lookup"><span data-stu-id="b6861-313">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="b6861-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-314">Boolean</span></span>|<span data-ttu-id="b6861-315">ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-315">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="b6861-316">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b6861-316">securityRequireVerifyApps</span></span>|<span data-ttu-id="b6861-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-317">Boolean</span></span>|<span data-ttu-id="b6861-318">アプリを確認する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-318">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="b6861-319">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="b6861-319">statusBarBlocked</span></span>|<span data-ttu-id="b6861-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-320">Boolean</span></span>|<span data-ttu-id="b6861-321">通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-321">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="b6861-322">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="b6861-322">stayOnModes</span></span>|<span data-ttu-id="b6861-323">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6861-323">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="b6861-324">デバイスの表示がオンのままになるモードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="b6861-324">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="b6861-325">このコレクションには、最大4つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b6861-325">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="b6861-326">使用可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。</span><span class="sxs-lookup"><span data-stu-id="b6861-326">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="b6861-327">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="b6861-327">storageAllowUsb</span></span>|<span data-ttu-id="b6861-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-328">Boolean</span></span>|<span data-ttu-id="b6861-329">USB 大容量ストレージを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-329">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="b6861-330">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="b6861-330">storageBlockExternalMedia</span></span>|<span data-ttu-id="b6861-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-331">Boolean</span></span>|<span data-ttu-id="b6861-332">外部メディアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-332">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="b6861-333">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="b6861-333">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="b6861-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-334">Boolean</span></span>|<span data-ttu-id="b6861-335">USB ファイル転送をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-335">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="b6861-336">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="b6861-336">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="b6861-337">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-337">Int32</span></span>|<span data-ttu-id="b6861-338">[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-338">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="b6861-339">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="b6861-339">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="b6861-340">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="b6861-340">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="b6861-341">Int32</span><span class="sxs-lookup"><span data-stu-id="b6861-341">Int32</span></span>|<span data-ttu-id="b6861-342">[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-342">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="b6861-343">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="b6861-343">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="b6861-344">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="b6861-344">systemUpdateInstallType</span></span>|[<span data-ttu-id="b6861-345">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="b6861-345">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="b6861-346">システム更新構成の種類。</span><span class="sxs-lookup"><span data-stu-id="b6861-346">The type of system update configuration.</span></span> <span data-ttu-id="b6861-347">使用可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="b6861-347">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="b6861-348">systemWindowsBlocked ブロック</span><span class="sxs-lookup"><span data-stu-id="b6861-348">systemWindowsBlocked</span></span>|<span data-ttu-id="b6861-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-349">Boolean</span></span>|<span data-ttu-id="b6861-350">Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6861-350">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="b6861-351">ユーザー Blockadd</span><span class="sxs-lookup"><span data-stu-id="b6861-351">usersBlockAdd</span></span>|<span data-ttu-id="b6861-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-352">Boolean</span></span>|<span data-ttu-id="b6861-353">ユーザーおよびプロファイルの追加を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-353">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="b6861-354">ユーザー Blockremove</span><span class="sxs-lookup"><span data-stu-id="b6861-354">usersBlockRemove</span></span>|<span data-ttu-id="b6861-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-355">Boolean</span></span>|<span data-ttu-id="b6861-356">他のユーザーのデバイスからの削除を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-356">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="b6861-357">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="b6861-357">volumeBlockAdjustment</span></span>|<span data-ttu-id="b6861-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-358">Boolean</span></span>|<span data-ttu-id="b6861-359">マスターボリュームを調整するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-359">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="b6861-360">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="b6861-360">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="b6861-361">String</span><span class="sxs-lookup"><span data-stu-id="b6861-361">String</span></span>|<span data-ttu-id="b6861-362">Always on VPN 接続を処理するアプリの Android アプリパッケージ名。</span><span class="sxs-lookup"><span data-stu-id="b6861-362">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="b6861-363">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="b6861-363">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="b6861-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-364">Boolean</span></span>|<span data-ttu-id="b6861-365">Always on VPN パッケージ名が指定されている場合は、VPN が切断されたときにネットワークトラフィックをロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6861-365">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="b6861-366">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="b6861-366">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="b6861-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-367">Boolean</span></span>|<span data-ttu-id="b6861-368">ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-368">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="b6861-369">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="b6861-369">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="b6861-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6861-370">Boolean</span></span>|<span data-ttu-id="b6861-371">ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6861-371">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="b6861-372">応答</span><span class="sxs-lookup"><span data-stu-id="b6861-372">Response</span></span>
<span data-ttu-id="b6861-373">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b6861-373">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6861-374">例</span><span class="sxs-lookup"><span data-stu-id="b6861-374">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6861-375">要求</span><span class="sxs-lookup"><span data-stu-id="b6861-375">Request</span></span>
<span data-ttu-id="b6861-376">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6861-376">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3678

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="b6861-377">応答</span><span class="sxs-lookup"><span data-stu-id="b6861-377">Response</span></span>
<span data-ttu-id="b6861-p133">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6861-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3850

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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





