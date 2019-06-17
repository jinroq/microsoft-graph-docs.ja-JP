---
title: deviceConfiguration リソースの種類
description: デバイス構成です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 980ec0e08ff43cd5b364801b3eca732bcb810188
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995967"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="723f9-103">deviceConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="723f9-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="723f9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="723f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="723f9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="723f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="723f9-106">デバイス構成です。</span><span class="sxs-lookup"><span data-stu-id="723f9-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="723f9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="723f9-107">Methods</span></span>
|<span data-ttu-id="723f9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="723f9-108">Method</span></span>|<span data-ttu-id="723f9-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="723f9-109">Return Type</span></span>|<span data-ttu-id="723f9-110">説明</span><span class="sxs-lookup"><span data-stu-id="723f9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="723f9-111">deviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="723f9-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="723f9-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="723f9-113">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="723f9-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="723f9-114">deviceConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="723f9-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="723f9-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="723f9-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="723f9-116">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="723f9-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="723f9-117">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="723f9-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="723f9-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="723f9-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="723f9-119">Not yet documented</span></span>|
|[<span data-ttu-id="723f9-120">windowsPrivacyAccessControls アクション</span><span class="sxs-lookup"><span data-stu-id="723f9-120">windowsPrivacyAccessControls action</span></span>](../api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="723f9-121">なし</span><span class="sxs-lookup"><span data-stu-id="723f9-121">None</span></span>|<span data-ttu-id="723f9-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="723f9-122">Not yet documented</span></span>|
|[<span data-ttu-id="723f9-123">assignedAccessMultiModeProfiles アクション</span><span class="sxs-lookup"><span data-stu-id="723f9-123">assignedAccessMultiModeProfiles action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="723f9-124">なし</span><span class="sxs-lookup"><span data-stu-id="723f9-124">None</span></span>|<span data-ttu-id="723f9-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="723f9-125">Not yet documented</span></span>|
|[<span data-ttu-id="723f9-126">getTargetedUsersAndDevices アクション</span><span class="sxs-lookup"><span data-stu-id="723f9-126">getTargetedUsersAndDevices action</span></span>](../api/intune-deviceconfig-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="723f9-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="723f9-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="723f9-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="723f9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="723f9-129">Properties</span></span>
|<span data-ttu-id="723f9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="723f9-130">Property</span></span>|<span data-ttu-id="723f9-131">型</span><span class="sxs-lookup"><span data-stu-id="723f9-131">Type</span></span>|<span data-ttu-id="723f9-132">説明</span><span class="sxs-lookup"><span data-stu-id="723f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="723f9-133">id</span><span class="sxs-lookup"><span data-stu-id="723f9-133">id</span></span>|<span data-ttu-id="723f9-134">文字列</span><span class="sxs-lookup"><span data-stu-id="723f9-134">String</span></span>|<span data-ttu-id="723f9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="723f9-135">Key of the entity.</span></span>|
|<span data-ttu-id="723f9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="723f9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="723f9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="723f9-137">DateTimeOffset</span></span>|<span data-ttu-id="723f9-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="723f9-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="723f9-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="723f9-139">roleScopeTagIds</span></span>|<span data-ttu-id="723f9-140">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-140">String collection</span></span>|<span data-ttu-id="723f9-141">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="723f9-141">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="723f9-142">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="723f9-142">supportsScopeTags</span></span>|<span data-ttu-id="723f9-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="723f9-143">Boolean</span></span>|<span data-ttu-id="723f9-144">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="723f9-144">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="723f9-145">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="723f9-145">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="723f9-146">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="723f9-146">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="723f9-147">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="723f9-147">This property is read-only.</span></span>|
|<span data-ttu-id="723f9-148">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="723f9-148">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="723f9-149">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="723f9-149">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="723f9-150">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="723f9-150">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="723f9-151">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="723f9-151">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="723f9-152">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="723f9-152">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="723f9-153">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="723f9-153">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="723f9-154">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="723f9-154">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="723f9-155">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="723f9-155">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="723f9-156">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="723f9-156">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="723f9-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="723f9-157">createdDateTime</span></span>|<span data-ttu-id="723f9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="723f9-158">DateTimeOffset</span></span>|<span data-ttu-id="723f9-159">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="723f9-159">DateTime the object was created.</span></span>|
|<span data-ttu-id="723f9-160">description</span><span class="sxs-lookup"><span data-stu-id="723f9-160">description</span></span>|<span data-ttu-id="723f9-161">String</span><span class="sxs-lookup"><span data-stu-id="723f9-161">String</span></span>|<span data-ttu-id="723f9-162">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="723f9-162">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="723f9-163">displayName</span><span class="sxs-lookup"><span data-stu-id="723f9-163">displayName</span></span>|<span data-ttu-id="723f9-164">String</span><span class="sxs-lookup"><span data-stu-id="723f9-164">String</span></span>|<span data-ttu-id="723f9-165">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="723f9-165">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="723f9-166">version</span><span class="sxs-lookup"><span data-stu-id="723f9-166">version</span></span>|<span data-ttu-id="723f9-167">Int32</span><span class="sxs-lookup"><span data-stu-id="723f9-167">Int32</span></span>|<span data-ttu-id="723f9-168">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="723f9-168">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="723f9-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="723f9-169">Relationships</span></span>
|<span data-ttu-id="723f9-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="723f9-170">Relationship</span></span>|<span data-ttu-id="723f9-171">型</span><span class="sxs-lookup"><span data-stu-id="723f9-171">Type</span></span>|<span data-ttu-id="723f9-172">説明</span><span class="sxs-lookup"><span data-stu-id="723f9-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="723f9-173">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="723f9-173">groupAssignments</span></span>|<span data-ttu-id="723f9-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="723f9-175">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="723f9-175">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="723f9-176">assignments</span><span class="sxs-lookup"><span data-stu-id="723f9-176">assignments</span></span>|<span data-ttu-id="723f9-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="723f9-178">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="723f9-178">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="723f9-179">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="723f9-179">deviceStatuses</span></span>|<span data-ttu-id="723f9-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="723f9-181">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="723f9-181">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="723f9-182">userStatuses</span><span class="sxs-lookup"><span data-stu-id="723f9-182">userStatuses</span></span>|<span data-ttu-id="723f9-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="723f9-184">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="723f9-184">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="723f9-185">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="723f9-185">deviceStatusOverview</span></span>|[<span data-ttu-id="723f9-186">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="723f9-186">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="723f9-187">デバイス構成のデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="723f9-187">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="723f9-188">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="723f9-188">userStatusOverview</span></span>|[<span data-ttu-id="723f9-189">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="723f9-189">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="723f9-190">デバイス構成のユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="723f9-190">Device Configuration users status overview</span></span>|
|<span data-ttu-id="723f9-191">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="723f9-191">deviceSettingStateSummaries</span></span>|<span data-ttu-id="723f9-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="723f9-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="723f9-193">デバイス構成設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="723f9-193">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="723f9-194">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="723f9-194">JSON Representation</span></span>
<span data-ttu-id="723f9-195">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="723f9-195">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```





