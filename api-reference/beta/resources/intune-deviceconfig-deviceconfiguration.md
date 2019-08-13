---
title: deviceConfiguration リソースの種類
description: デバイス構成です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88f1dc66fbbb95b4b8f9a340949f41f573eb22fb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333045"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="34748-103">deviceConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34748-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="34748-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34748-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34748-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="34748-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34748-106">デバイス構成です。</span><span class="sxs-lookup"><span data-stu-id="34748-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="34748-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="34748-107">Methods</span></span>
|<span data-ttu-id="34748-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="34748-108">Method</span></span>|<span data-ttu-id="34748-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="34748-109">Return Type</span></span>|<span data-ttu-id="34748-110">説明</span><span class="sxs-lookup"><span data-stu-id="34748-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34748-111">deviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="34748-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="34748-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="34748-113">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="34748-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="34748-114">deviceConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="34748-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="34748-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="34748-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="34748-116">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="34748-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="34748-117">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="34748-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="34748-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="34748-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="34748-119">Not yet documented</span></span>|
|[<span data-ttu-id="34748-120">windowsPrivacyAccessControls アクション</span><span class="sxs-lookup"><span data-stu-id="34748-120">windowsPrivacyAccessControls action</span></span>](../api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="34748-121">なし</span><span class="sxs-lookup"><span data-stu-id="34748-121">None</span></span>|<span data-ttu-id="34748-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="34748-122">Not yet documented</span></span>|
|[<span data-ttu-id="34748-123">assignedAccessMultiModeProfiles アクション</span><span class="sxs-lookup"><span data-stu-id="34748-123">assignedAccessMultiModeProfiles action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="34748-124">なし</span><span class="sxs-lookup"><span data-stu-id="34748-124">None</span></span>|<span data-ttu-id="34748-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="34748-125">Not yet documented</span></span>|
|[<span data-ttu-id="34748-126">getTargetedUsersAndDevices アクション</span><span class="sxs-lookup"><span data-stu-id="34748-126">getTargetedUsersAndDevices action</span></span>](../api/intune-deviceconfig-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="34748-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="34748-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="34748-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="34748-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34748-129">Properties</span></span>
|<span data-ttu-id="34748-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34748-130">Property</span></span>|<span data-ttu-id="34748-131">型</span><span class="sxs-lookup"><span data-stu-id="34748-131">Type</span></span>|<span data-ttu-id="34748-132">説明</span><span class="sxs-lookup"><span data-stu-id="34748-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34748-133">id</span><span class="sxs-lookup"><span data-stu-id="34748-133">id</span></span>|<span data-ttu-id="34748-134">文字列</span><span class="sxs-lookup"><span data-stu-id="34748-134">String</span></span>|<span data-ttu-id="34748-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="34748-135">Key of the entity.</span></span>|
|<span data-ttu-id="34748-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34748-136">lastModifiedDateTime</span></span>|<span data-ttu-id="34748-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34748-137">DateTimeOffset</span></span>|<span data-ttu-id="34748-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="34748-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="34748-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34748-139">roleScopeTagIds</span></span>|<span data-ttu-id="34748-140">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-140">String collection</span></span>|<span data-ttu-id="34748-141">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="34748-141">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="34748-142">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="34748-142">supportsScopeTags</span></span>|<span data-ttu-id="34748-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="34748-143">Boolean</span></span>|<span data-ttu-id="34748-144">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="34748-144">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34748-145">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="34748-145">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34748-146">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="34748-146">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34748-147">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="34748-147">This property is read-only.</span></span>|
|<span data-ttu-id="34748-148">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34748-148">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="34748-149">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34748-149">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="34748-150">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="34748-150">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="34748-151">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34748-151">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="34748-152">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34748-152">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="34748-153">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="34748-153">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="34748-154">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="34748-154">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="34748-155">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="34748-155">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="34748-156">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="34748-156">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="34748-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34748-157">createdDateTime</span></span>|<span data-ttu-id="34748-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34748-158">DateTimeOffset</span></span>|<span data-ttu-id="34748-159">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="34748-159">DateTime the object was created.</span></span>|
|<span data-ttu-id="34748-160">description</span><span class="sxs-lookup"><span data-stu-id="34748-160">description</span></span>|<span data-ttu-id="34748-161">String</span><span class="sxs-lookup"><span data-stu-id="34748-161">String</span></span>|<span data-ttu-id="34748-162">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="34748-162">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="34748-163">displayName</span><span class="sxs-lookup"><span data-stu-id="34748-163">displayName</span></span>|<span data-ttu-id="34748-164">String</span><span class="sxs-lookup"><span data-stu-id="34748-164">String</span></span>|<span data-ttu-id="34748-165">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="34748-165">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="34748-166">version</span><span class="sxs-lookup"><span data-stu-id="34748-166">version</span></span>|<span data-ttu-id="34748-167">Int32</span><span class="sxs-lookup"><span data-stu-id="34748-167">Int32</span></span>|<span data-ttu-id="34748-168">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="34748-168">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34748-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="34748-169">Relationships</span></span>
|<span data-ttu-id="34748-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="34748-170">Relationship</span></span>|<span data-ttu-id="34748-171">型</span><span class="sxs-lookup"><span data-stu-id="34748-171">Type</span></span>|<span data-ttu-id="34748-172">説明</span><span class="sxs-lookup"><span data-stu-id="34748-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34748-173">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="34748-173">groupAssignments</span></span>|<span data-ttu-id="34748-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="34748-175">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="34748-175">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="34748-176">assignments</span><span class="sxs-lookup"><span data-stu-id="34748-176">assignments</span></span>|<span data-ttu-id="34748-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="34748-178">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="34748-178">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="34748-179">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="34748-179">deviceStatuses</span></span>|<span data-ttu-id="34748-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="34748-181">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="34748-181">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="34748-182">userStatuses</span><span class="sxs-lookup"><span data-stu-id="34748-182">userStatuses</span></span>|<span data-ttu-id="34748-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="34748-184">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="34748-184">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="34748-185">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="34748-185">deviceStatusOverview</span></span>|[<span data-ttu-id="34748-186">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="34748-186">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="34748-187">デバイス構成のデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="34748-187">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="34748-188">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="34748-188">userStatusOverview</span></span>|[<span data-ttu-id="34748-189">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="34748-189">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="34748-190">デバイス構成のユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="34748-190">Device Configuration users status overview</span></span>|
|<span data-ttu-id="34748-191">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="34748-191">deviceSettingStateSummaries</span></span>|<span data-ttu-id="34748-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="34748-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="34748-193">デバイス構成設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="34748-193">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34748-194">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34748-194">JSON Representation</span></span>
<span data-ttu-id="34748-195">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34748-195">Here is a JSON representation of the resource.</span></span>
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



