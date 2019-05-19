---
title: iosDerivedCredentialAuthenticationConfiguration リソースの種類
description: iOS の派生した資格情報プロファイル。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1aa7bab23f6c90420e262bed0c5a3f8a72cbbb51
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33957057"
---
# <a name="iosderivedcredentialauthenticationconfiguration-resource-type"></a><span data-ttu-id="a214c-103">iosDerivedCredentialAuthenticationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a214c-103">iosDerivedCredentialAuthenticationConfiguration resource type</span></span>

> <span data-ttu-id="a214c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a214c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a214c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a214c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a214c-106">iOS の派生した資格情報プロファイル。</span><span class="sxs-lookup"><span data-stu-id="a214c-106">iOS Derived Credential profile.</span></span>


<span data-ttu-id="a214c-107">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a214c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a214c-108">Methods</span></span>
|<span data-ttu-id="a214c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a214c-109">Method</span></span>|<span data-ttu-id="a214c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a214c-110">Return Type</span></span>|<span data-ttu-id="a214c-111">説明</span><span class="sxs-lookup"><span data-stu-id="a214c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a214c-112">リスト iosDerivedCredentialAuthenticationConfigurations</span><span class="sxs-lookup"><span data-stu-id="a214c-112">List iosDerivedCredentialAuthenticationConfigurations</span></span>](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-list.md)|<span data-ttu-id="a214c-113">[iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a214c-113">[iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) collection</span></span>|<span data-ttu-id="a214c-114">[IosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a214c-114">List properties and relationships of the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a214c-115">IosDerivedCredentialAuthenticationConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="a214c-115">Get iosDerivedCredentialAuthenticationConfiguration</span></span>](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-get.md)|[<span data-ttu-id="a214c-116">iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a214c-116">iosDerivedCredentialAuthenticationConfiguration</span></span>](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)|<span data-ttu-id="a214c-117">[IosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a214c-117">Read properties and relationships of the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a214c-118">IosDerivedCredentialAuthenticationConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="a214c-118">Create iosDerivedCredentialAuthenticationConfiguration</span></span>](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-create.md)|[<span data-ttu-id="a214c-119">iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a214c-119">iosDerivedCredentialAuthenticationConfiguration</span></span>](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)|<span data-ttu-id="a214c-120">新しい[iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a214c-120">Create a new [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a214c-121">IosDerivedCredentialAuthenticationConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="a214c-121">Delete iosDerivedCredentialAuthenticationConfiguration</span></span>](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-delete.md)|<span data-ttu-id="a214c-122">None</span><span class="sxs-lookup"><span data-stu-id="a214c-122">None</span></span>|<span data-ttu-id="a214c-123">[IosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a214c-123">Deletes a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md).</span></span>|
|[<span data-ttu-id="a214c-124">IosDerivedCredentialAuthenticationConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a214c-124">Update iosDerivedCredentialAuthenticationConfiguration</span></span>](../api/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration-update.md)|[<span data-ttu-id="a214c-125">iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a214c-125">iosDerivedCredentialAuthenticationConfiguration</span></span>](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)|<span data-ttu-id="a214c-126">[IosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a214c-126">Update the properties of a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a214c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a214c-127">Properties</span></span>
|<span data-ttu-id="a214c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a214c-128">Property</span></span>|<span data-ttu-id="a214c-129">種類</span><span class="sxs-lookup"><span data-stu-id="a214c-129">Type</span></span>|<span data-ttu-id="a214c-130">説明</span><span class="sxs-lookup"><span data-stu-id="a214c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a214c-131">id</span><span class="sxs-lookup"><span data-stu-id="a214c-131">id</span></span>|<span data-ttu-id="a214c-132">文字列</span><span class="sxs-lookup"><span data-stu-id="a214c-132">String</span></span>|<span data-ttu-id="a214c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a214c-133">Key of the entity.</span></span> <span data-ttu-id="a214c-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a214c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a214c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a214c-136">DateTimeOffset</span></span>|<span data-ttu-id="a214c-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a214c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a214c-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a214c-139">roleScopeTagIds</span></span>|<span data-ttu-id="a214c-140">String collection</span><span class="sxs-lookup"><span data-stu-id="a214c-140">String collection</span></span>|<span data-ttu-id="a214c-141">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a214c-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a214c-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-143">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a214c-143">supportsScopeTags</span></span>|<span data-ttu-id="a214c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="a214c-144">Boolean</span></span>|<span data-ttu-id="a214c-145">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a214c-145">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a214c-146">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a214c-146">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a214c-147">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a214c-147">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a214c-148">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a214c-148">This property is read-only.</span></span> <span data-ttu-id="a214c-149">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a214c-150">createdDateTime</span></span>|<span data-ttu-id="a214c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a214c-151">DateTimeOffset</span></span>|<span data-ttu-id="a214c-152">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a214c-152">DateTime the object was created.</span></span> <span data-ttu-id="a214c-153">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-154">description</span><span class="sxs-lookup"><span data-stu-id="a214c-154">description</span></span>|<span data-ttu-id="a214c-155">String</span><span class="sxs-lookup"><span data-stu-id="a214c-155">String</span></span>|<span data-ttu-id="a214c-156">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a214c-156">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a214c-157">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-158">displayName</span><span class="sxs-lookup"><span data-stu-id="a214c-158">displayName</span></span>|<span data-ttu-id="a214c-159">String</span><span class="sxs-lookup"><span data-stu-id="a214c-159">String</span></span>|<span data-ttu-id="a214c-160">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a214c-160">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a214c-161">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-162">version</span><span class="sxs-lookup"><span data-stu-id="a214c-162">version</span></span>|<span data-ttu-id="a214c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="a214c-163">Int32</span></span>|<span data-ttu-id="a214c-164">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a214c-164">Version of the device configuration.</span></span> <span data-ttu-id="a214c-165">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-165">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a214c-166">関係</span><span class="sxs-lookup"><span data-stu-id="a214c-166">Relationships</span></span>
|<span data-ttu-id="a214c-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a214c-167">Relationship</span></span>|<span data-ttu-id="a214c-168">型</span><span class="sxs-lookup"><span data-stu-id="a214c-168">Type</span></span>|<span data-ttu-id="a214c-169">説明</span><span class="sxs-lookup"><span data-stu-id="a214c-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a214c-170">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="a214c-170">groupAssignments</span></span>|<span data-ttu-id="a214c-171">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a214c-171">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="a214c-172">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="a214c-172">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="a214c-173">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-173">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-174">assignments</span><span class="sxs-lookup"><span data-stu-id="a214c-174">assignments</span></span>|<span data-ttu-id="a214c-175">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a214c-175">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a214c-176">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="a214c-176">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="a214c-177">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-177">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-178">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a214c-178">deviceStatuses</span></span>|<span data-ttu-id="a214c-179">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a214c-179">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a214c-180">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="a214c-180">Device configuration installation status by device.</span></span> <span data-ttu-id="a214c-181">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-181">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-182">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a214c-182">userStatuses</span></span>|<span data-ttu-id="a214c-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a214c-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a214c-184">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="a214c-184">Device configuration installation status by user.</span></span> <span data-ttu-id="a214c-185">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a214c-185">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-186">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a214c-186">deviceStatusOverview</span></span>|[<span data-ttu-id="a214c-187">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a214c-187">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a214c-188">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a214c-188">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-189">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a214c-189">userStatusOverview</span></span>|[<span data-ttu-id="a214c-190">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a214c-190">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="a214c-191">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a214c-191">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-192">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a214c-192">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a214c-193">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a214c-193">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a214c-194">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a214c-194">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a214c-195">derivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="a214c-195">derivedCredentialSettings</span></span>|[<span data-ttu-id="a214c-196">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="a214c-196">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="a214c-197">認証に使用される派生した資格情報のテナントレベルの設定。</span><span class="sxs-lookup"><span data-stu-id="a214c-197">Tenant level settings for the Derived Credentials to be used for authentication.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a214c-198">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a214c-198">JSON Representation</span></span>
<span data-ttu-id="a214c-199">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a214c-199">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosDerivedCredentialAuthenticationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```



