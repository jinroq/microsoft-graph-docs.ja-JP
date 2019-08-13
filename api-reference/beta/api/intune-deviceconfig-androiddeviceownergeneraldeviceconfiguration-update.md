---
title: Androiddeviceowner一般の Devic/デバイスの更新
description: Androiddeviceownerのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 183a5fe6a9250315bba668671561bc0b402267ca
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36312566"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="6ed09-103">Androiddeviceowner一般の Devic/デバイスの更新</span><span class="sxs-lookup"><span data-stu-id="6ed09-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6ed09-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ed09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ed09-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ed09-106">[Androiddeviceownerの](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ed09-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6ed09-107">Prerequisites</span></span>
<span data-ttu-id="6ed09-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ed09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ed09-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ed09-110">Permission type</span></span>|<span data-ttu-id="6ed09-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ed09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ed09-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ed09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ed09-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ed09-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ed09-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ed09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ed09-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ed09-115">Not supported.</span></span>|
|<span data-ttu-id="6ed09-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ed09-116">Application</span></span>|<span data-ttu-id="6ed09-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ed09-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ed09-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ed09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6ed09-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ed09-119">Request headers</span></span>
|<span data-ttu-id="6ed09-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ed09-120">Header</span></span>|<span data-ttu-id="6ed09-121">値</span><span class="sxs-lookup"><span data-stu-id="6ed09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ed09-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ed09-122">Authorization</span></span>|<span data-ttu-id="6ed09-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ed09-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6ed09-124">Accept</span></span>|<span data-ttu-id="6ed09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ed09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ed09-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ed09-126">Request body</span></span>
<span data-ttu-id="6ed09-127">要求本文で、 [Androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devic/DEVICオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6ed09-128">次の表に、 [Androiddeviceowner[devic]](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="6ed09-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ed09-129">Property</span></span>|<span data-ttu-id="6ed09-130">型</span><span class="sxs-lookup"><span data-stu-id="6ed09-130">Type</span></span>|<span data-ttu-id="6ed09-131">説明</span><span class="sxs-lookup"><span data-stu-id="6ed09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ed09-132">id</span><span class="sxs-lookup"><span data-stu-id="6ed09-132">id</span></span>|<span data-ttu-id="6ed09-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6ed09-133">String</span></span>|<span data-ttu-id="6ed09-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6ed09-134">Key of the entity.</span></span> <span data-ttu-id="6ed09-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ed09-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6ed09-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ed09-137">DateTimeOffset</span></span>|<span data-ttu-id="6ed09-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="6ed09-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6ed09-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ed09-140">roleScopeTagIds</span></span>|<span data-ttu-id="6ed09-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6ed09-141">String collection</span></span>|<span data-ttu-id="6ed09-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="6ed09-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ed09-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6ed09-144">supportsScopeTags</span></span>|<span data-ttu-id="6ed09-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-145">Boolean</span></span>|<span data-ttu-id="6ed09-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ed09-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="6ed09-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ed09-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="6ed09-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ed09-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-149">This property is read-only.</span></span> <span data-ttu-id="6ed09-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ed09-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6ed09-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ed09-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6ed09-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="6ed09-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6ed09-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ed09-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6ed09-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ed09-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6ed09-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="6ed09-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6ed09-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="6ed09-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6ed09-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="6ed09-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6ed09-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="6ed09-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6ed09-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ed09-163">createdDateTime</span></span>|<span data-ttu-id="6ed09-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ed09-164">DateTimeOffset</span></span>|<span data-ttu-id="6ed09-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6ed09-165">DateTime the object was created.</span></span> <span data-ttu-id="6ed09-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-167">description</span><span class="sxs-lookup"><span data-stu-id="6ed09-167">description</span></span>|<span data-ttu-id="6ed09-168">String</span><span class="sxs-lookup"><span data-stu-id="6ed09-168">String</span></span>|<span data-ttu-id="6ed09-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="6ed09-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ed09-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6ed09-171">displayName</span></span>|<span data-ttu-id="6ed09-172">String</span><span class="sxs-lookup"><span data-stu-id="6ed09-172">String</span></span>|<span data-ttu-id="6ed09-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="6ed09-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ed09-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-175">version</span><span class="sxs-lookup"><span data-stu-id="6ed09-175">version</span></span>|<span data-ttu-id="6ed09-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-176">Int32</span></span>|<span data-ttu-id="6ed09-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6ed09-177">Version of the device configuration.</span></span> <span data-ttu-id="6ed09-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ed09-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ed09-179">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="6ed09-179">accountsBlockModification</span></span>|<span data-ttu-id="6ed09-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-180">Boolean</span></span>|<span data-ttu-id="6ed09-181">アカウントの追加または削除が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="6ed09-182">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6ed09-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="6ed09-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-183">Boolean</span></span>|<span data-ttu-id="6ed09-184">ユーザーが不明なソースを有効にできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="6ed09-185">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="6ed09-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="6ed09-186">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="6ed09-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="6ed09-187">アプリの自動更新ポリシーの値を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="6ed09-188">可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="6ed09-189">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="6ed09-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="6ed09-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="6ed09-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="6ed09-191">アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="6ed09-192">使用可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="6ed09-193">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="6ed09-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="6ed09-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-194">Boolean</span></span>|<span data-ttu-id="6ed09-195">すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="6ed09-196">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ed09-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="6ed09-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-197">Boolean</span></span>|<span data-ttu-id="6ed09-198">ユーザーが bluetooth を構成することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="6ed09-199">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="6ed09-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="6ed09-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-200">Boolean</span></span>|<span data-ttu-id="6ed09-201">ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="6ed09-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="6ed09-202">cameraBlocked</span></span>|<span data-ttu-id="6ed09-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-203">Boolean</span></span>|<span data-ttu-id="6ed09-204">カメラの使用を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="6ed09-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="6ed09-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="6ed09-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-206">Boolean</span></span>|<span data-ttu-id="6ed09-207">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="6ed09-208">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="6ed09-208">dataRoamingBlocked</span></span>|<span data-ttu-id="6ed09-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-209">Boolean</span></span>|<span data-ttu-id="6ed09-210">ユーザーのデータ移動を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-210">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="6ed09-211">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="6ed09-211">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="6ed09-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-212">Boolean</span></span>|<span data-ttu-id="6ed09-213">ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-213">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="6ed09-214">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="6ed09-214">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="6ed09-215">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6ed09-215">String collection</span></span>|<span data-ttu-id="6ed09-216">デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。</span><span class="sxs-lookup"><span data-stu-id="6ed09-216">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="6ed09-217">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="6ed09-217">factoryResetBlocked</span></span>|<span data-ttu-id="6ed09-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-218">Boolean</span></span>|<span data-ttu-id="6ed09-219">設定の出荷時のリセットオプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-219">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="6ed09-220">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="6ed09-220">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="6ed09-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-221">Boolean</span></span>|<span data-ttu-id="6ed09-222">スクリーンセーバーモードを有効にするか、キオスクモードにしないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-222">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-223">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="6ed09-223">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="6ed09-224">String</span><span class="sxs-lookup"><span data-stu-id="6ed09-224">String</span></span>|<span data-ttu-id="6ed09-225">キオスクモードでデバイスのスクリーンセーバーになる画像の URL。</span><span class="sxs-lookup"><span data-stu-id="6ed09-225">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-226">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="6ed09-226">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="6ed09-227">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-227">Int32</span></span>|<span data-ttu-id="6ed09-228">キオスクモードの場合にデバイスがスクリーンセーバーを表示する秒数。</span><span class="sxs-lookup"><span data-stu-id="6ed09-228">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="6ed09-229">有効な値は 0 ~ 9999999</span><span class="sxs-lookup"><span data-stu-id="6ed09-229">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="6ed09-230">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="6ed09-230">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="6ed09-231">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-231">Int32</span></span>|<span data-ttu-id="6ed09-232">スクリーンセーバーがキオスクモードで表示されるまでに、デバイスが非アクティブになる必要のある時間 (秒数)。</span><span class="sxs-lookup"><span data-stu-id="6ed09-232">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="6ed09-233">有効な値は 1 ~ 9999999</span><span class="sxs-lookup"><span data-stu-id="6ed09-233">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="6ed09-234">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="6ed09-234">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="6ed09-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-235">Boolean</span></span>|<span data-ttu-id="6ed09-236">音声/ビデオがキオスクモードで再生されている場合に、デバイス画面にスクリーンセーバーを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-236">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-237">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="6ed09-237">kioskModeApps</span></span>|<span data-ttu-id="6ed09-238">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6ed09-238">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6ed09-239">デバイスがキオスクモードのときに表示される管理対象アプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="6ed09-239">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="6ed09-240">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6ed09-240">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ed09-241">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="6ed09-241">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="6ed09-242">String</span><span class="sxs-lookup"><span data-stu-id="6ed09-242">String</span></span>|<span data-ttu-id="6ed09-243">デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。</span><span class="sxs-lookup"><span data-stu-id="6ed09-243">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-244">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="6ed09-244">kioskModeExitCode</span></span>|<span data-ttu-id="6ed09-245">String</span><span class="sxs-lookup"><span data-stu-id="6ed09-245">String</span></span>|<span data-ttu-id="6ed09-246">デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。</span><span class="sxs-lookup"><span data-stu-id="6ed09-246">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-247">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="6ed09-247">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="6ed09-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-248">Boolean</span></span>|<span data-ttu-id="6ed09-249">デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-249">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-250">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="6ed09-250">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="6ed09-251">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="6ed09-251">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="6ed09-252">仮想ホームボタンが [ホームにスワイプ] ボタンか、またはフローティングの [ホーム] ボタンかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-252">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="6ed09-253">可能な値は、`notConfigured`、`swipeUp`、`floating` です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-253">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="6ed09-254">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="6ed09-254">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="6ed09-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-255">Boolean</span></span>|<span data-ttu-id="6ed09-256">ユーザーがキオスクモードで Bluetooth 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-256">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-257">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="6ed09-257">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="6ed09-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-258">Boolean</span></span>|<span data-ttu-id="6ed09-259">ユーザーがキオスクモードで Wi-fi 設定を構成することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-259">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-260">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="6ed09-260">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="6ed09-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-261">Boolean</span></span>|<span data-ttu-id="6ed09-262">ユーザーがキオスクモードで懐中電灯を使用できるようにするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-262">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-263">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="6ed09-263">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="6ed09-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-264">Boolean</span></span>|<span data-ttu-id="6ed09-265">ユーザーがキオスクモードでメディアボリュームを変更することを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-265">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="6ed09-266">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="6ed09-266">microphoneForceMute</span></span>|<span data-ttu-id="6ed09-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-267">Boolean</span></span>|<span data-ttu-id="6ed09-268">デバイス上でのマイクのミュートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-268">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="6ed09-269">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="6ed09-269">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="6ed09-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-270">Boolean</span></span>|<span data-ttu-id="6ed09-271">ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-271">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="6ed09-272">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="6ed09-272">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="6ed09-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-273">Boolean</span></span>|<span data-ttu-id="6ed09-274">NFC の送信ビームをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-274">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="6ed09-275">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="6ed09-275">passwordBlockKeyguard</span></span>|<span data-ttu-id="6ed09-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-276">Boolean</span></span>|<span data-ttu-id="6ed09-277">Keyguard が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-277">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="6ed09-278">Passwordblockkeygu/機能</span><span class="sxs-lookup"><span data-stu-id="6ed09-278">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="6ed09-279">[Androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6ed09-279">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="6ed09-280">ブロックする device keyguard 機能のリストです。</span><span class="sxs-lookup"><span data-stu-id="6ed09-280">List of device keyguard features to block.</span></span> <span data-ttu-id="6ed09-281">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6ed09-281">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="6ed09-282">可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-282">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="6ed09-283">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6ed09-283">passwordExpirationDays</span></span>|<span data-ttu-id="6ed09-284">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-284">Int32</span></span>|<span data-ttu-id="6ed09-285">パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ed09-285">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="6ed09-286">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-286">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6ed09-287">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6ed09-287">passwordMinimumLength</span></span>|<span data-ttu-id="6ed09-288">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-288">Int32</span></span>|<span data-ttu-id="6ed09-289">デバイスで必要なパスワードの最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-289">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="6ed09-290">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-290">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6ed09-291">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6ed09-291">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="6ed09-292">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-292">Int32</span></span>|<span data-ttu-id="6ed09-293">デバイスパスワードに必要な文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-293">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="6ed09-294">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-294">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6ed09-295">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6ed09-295">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="6ed09-296">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-296">Int32</span></span>|<span data-ttu-id="6ed09-297">デバイスパスワードに必要な小文字の最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-297">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="6ed09-298">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-298">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6ed09-299">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6ed09-299">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="6ed09-300">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-300">Int32</span></span>|<span data-ttu-id="6ed09-301">デバイスパスワードに必要な文字以外の文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-301">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="6ed09-302">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-302">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6ed09-303">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="6ed09-303">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="6ed09-304">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-304">Int32</span></span>|<span data-ttu-id="6ed09-305">デバイスパスワードに必要な最小文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-305">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="6ed09-306">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-306">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6ed09-307">Passwordminimumシンボル文字</span><span class="sxs-lookup"><span data-stu-id="6ed09-307">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="6ed09-308">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-308">Int32</span></span>|<span data-ttu-id="6ed09-309">デバイスパスワードに必要な最小記号文字数を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-309">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="6ed09-310">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-310">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6ed09-311">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6ed09-311">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="6ed09-312">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-312">Int32</span></span>|<span data-ttu-id="6ed09-313">デバイスのパスワードに必要な上位 caseletter 文字の最小数を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-313">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="6ed09-314">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-314">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6ed09-315">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6ed09-315">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6ed09-316">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-316">Int32</span></span>|<span data-ttu-id="6ed09-317">画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。</span><span class="sxs-lookup"><span data-stu-id="6ed09-317">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6ed09-318">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="6ed09-318">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="6ed09-319">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-319">Int32</span></span>|<span data-ttu-id="6ed09-320">パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。</span><span class="sxs-lookup"><span data-stu-id="6ed09-320">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="6ed09-321">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-321">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6ed09-322">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6ed09-322">passwordRequiredType</span></span>|[<span data-ttu-id="6ed09-323">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6ed09-323">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="6ed09-324">デバイスで必要なパスワードの最小品質を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-324">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="6ed09-325">可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-325">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="6ed09-326">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6ed09-326">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6ed09-327">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-327">Int32</span></span>|<span data-ttu-id="6ed09-328">ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-328">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="6ed09-329">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="6ed09-329">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6ed09-330">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="6ed09-330">playStoreMode</span></span>|[<span data-ttu-id="6ed09-331">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="6ed09-331">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="6ed09-332">デバイスの再生ストアモードを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-332">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="6ed09-333">可能な値は、`notConfigured`、`allowList`、`blockList` です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-333">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="6ed09-334">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="6ed09-334">safeBootBlocked</span></span>|<span data-ttu-id="6ed09-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-335">Boolean</span></span>|<span data-ttu-id="6ed09-336">セーフブートでのデバイスの再起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-336">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="6ed09-337">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6ed09-337">screenCaptureBlocked</span></span>|<span data-ttu-id="6ed09-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-338">Boolean</span></span>|<span data-ttu-id="6ed09-339">スクリーンショットを撮影する機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-339">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="6ed09-340">Securityallowデバッグ機能</span><span class="sxs-lookup"><span data-stu-id="6ed09-340">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="6ed09-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-341">Boolean</span></span>|<span data-ttu-id="6ed09-342">ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-342">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="6ed09-343">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6ed09-343">securityRequireVerifyApps</span></span>|<span data-ttu-id="6ed09-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-344">Boolean</span></span>|<span data-ttu-id="6ed09-345">アプリを確認する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-345">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="6ed09-346">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="6ed09-346">statusBarBlocked</span></span>|<span data-ttu-id="6ed09-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-347">Boolean</span></span>|<span data-ttu-id="6ed09-348">通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-348">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="6ed09-349">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="6ed09-349">stayOnModes</span></span>|<span data-ttu-id="6ed09-350">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6ed09-350">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="6ed09-351">デバイスの表示がオンのままになるモードの一覧です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-351">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="6ed09-352">このコレクションには、最大4つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6ed09-352">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="6ed09-353">使用可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-353">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="6ed09-354">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="6ed09-354">storageAllowUsb</span></span>|<span data-ttu-id="6ed09-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-355">Boolean</span></span>|<span data-ttu-id="6ed09-356">USB 大容量ストレージを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-356">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="6ed09-357">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="6ed09-357">storageBlockExternalMedia</span></span>|<span data-ttu-id="6ed09-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-358">Boolean</span></span>|<span data-ttu-id="6ed09-359">外部メディアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-359">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="6ed09-360">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="6ed09-360">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="6ed09-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-361">Boolean</span></span>|<span data-ttu-id="6ed09-362">USB ファイル転送をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-362">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="6ed09-363">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="6ed09-363">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="6ed09-364">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-364">Int32</span></span>|<span data-ttu-id="6ed09-365">[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-365">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="6ed09-366">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="6ed09-366">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="6ed09-367">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="6ed09-367">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="6ed09-368">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed09-368">Int32</span></span>|<span data-ttu-id="6ed09-369">[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-369">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="6ed09-370">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="6ed09-370">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="6ed09-371">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="6ed09-371">systemUpdateInstallType</span></span>|[<span data-ttu-id="6ed09-372">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="6ed09-372">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="6ed09-373">システム更新構成の種類。</span><span class="sxs-lookup"><span data-stu-id="6ed09-373">The type of system update configuration.</span></span> <span data-ttu-id="6ed09-374">使用可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-374">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="6ed09-375">systemWindowsBlocked ブロック</span><span class="sxs-lookup"><span data-stu-id="6ed09-375">systemWindowsBlocked</span></span>|<span data-ttu-id="6ed09-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-376">Boolean</span></span>|<span data-ttu-id="6ed09-377">Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-377">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="6ed09-378">ユーザー Blockadd</span><span class="sxs-lookup"><span data-stu-id="6ed09-378">usersBlockAdd</span></span>|<span data-ttu-id="6ed09-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-379">Boolean</span></span>|<span data-ttu-id="6ed09-380">ユーザーおよびプロファイルの追加を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-380">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="6ed09-381">ユーザー Blockremove</span><span class="sxs-lookup"><span data-stu-id="6ed09-381">usersBlockRemove</span></span>|<span data-ttu-id="6ed09-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-382">Boolean</span></span>|<span data-ttu-id="6ed09-383">他のユーザーのデバイスからの削除を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-383">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="6ed09-384">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="6ed09-384">volumeBlockAdjustment</span></span>|<span data-ttu-id="6ed09-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-385">Boolean</span></span>|<span data-ttu-id="6ed09-386">マスターボリュームを調整するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-386">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="6ed09-387">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="6ed09-387">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="6ed09-388">String</span><span class="sxs-lookup"><span data-stu-id="6ed09-388">String</span></span>|<span data-ttu-id="6ed09-389">Always on VPN 接続を処理するアプリの Android アプリパッケージ名。</span><span class="sxs-lookup"><span data-stu-id="6ed09-389">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="6ed09-390">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="6ed09-390">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="6ed09-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-391">Boolean</span></span>|<span data-ttu-id="6ed09-392">Always on VPN パッケージ名が指定されている場合は、VPN が切断されたときにネットワークトラフィックをロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-392">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="6ed09-393">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="6ed09-393">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="6ed09-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-394">Boolean</span></span>|<span data-ttu-id="6ed09-395">ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-395">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="6ed09-396">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="6ed09-396">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="6ed09-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed09-397">Boolean</span></span>|<span data-ttu-id="6ed09-398">ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-398">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="6ed09-399">応答</span><span class="sxs-lookup"><span data-stu-id="6ed09-399">Response</span></span>
<span data-ttu-id="6ed09-400">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devic/オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6ed09-400">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ed09-401">例</span><span class="sxs-lookup"><span data-stu-id="6ed09-401">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ed09-402">要求</span><span class="sxs-lookup"><span data-stu-id="6ed09-402">Request</span></span>
<span data-ttu-id="6ed09-403">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ed09-403">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4123

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
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
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
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
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

### <a name="response"></a><span data-ttu-id="6ed09-404">応答</span><span class="sxs-lookup"><span data-stu-id="6ed09-404">Response</span></span>
<span data-ttu-id="6ed09-p136">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ed09-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4295

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
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
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
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
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






