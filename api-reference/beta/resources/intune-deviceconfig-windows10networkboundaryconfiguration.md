---
title: windows10NetworkBoundaryConfiguration リソースの種類
description: Windows10 ネットワーク境界の構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7231e7c1d8c509058fb18f6958e39f48cc84e4fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944293"
---
# <a name="windows10networkboundaryconfiguration-resource-type"></a><span data-ttu-id="d2462-103">windows10NetworkBoundaryConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2462-103">windows10NetworkBoundaryConfiguration resource type</span></span>

> <span data-ttu-id="d2462-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2462-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2462-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2462-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2462-106">Windows10 ネットワーク境界の構成</span><span class="sxs-lookup"><span data-stu-id="d2462-106">Windows10 Network Boundary Configuration</span></span>


<span data-ttu-id="d2462-107">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d2462-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2462-108">Methods</span></span>
|<span data-ttu-id="d2462-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2462-109">Method</span></span>|<span data-ttu-id="d2462-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d2462-110">Return Type</span></span>|<span data-ttu-id="d2462-111">説明</span><span class="sxs-lookup"><span data-stu-id="d2462-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2462-112">リスト windows10NetworkBoundaryConfigurations</span><span class="sxs-lookup"><span data-stu-id="d2462-112">List windows10NetworkBoundaryConfigurations</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-list.md)|<span data-ttu-id="d2462-113">[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d2462-113">[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) collection</span></span>|<span data-ttu-id="d2462-114">[Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d2462-114">List properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d2462-115">Windows10NetworkBoundaryConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="d2462-115">Get windows10NetworkBoundaryConfiguration</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-get.md)|[<span data-ttu-id="d2462-116">windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2462-116">windows10NetworkBoundaryConfiguration</span></span>](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)|<span data-ttu-id="d2462-117">[Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d2462-117">Read properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d2462-118">Windows10NetworkBoundaryConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="d2462-118">Create windows10NetworkBoundaryConfiguration</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-create.md)|[<span data-ttu-id="d2462-119">windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2462-119">windows10NetworkBoundaryConfiguration</span></span>](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)|<span data-ttu-id="d2462-120">新しい[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d2462-120">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d2462-121">Windows10NetworkBoundaryConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="d2462-121">Delete windows10NetworkBoundaryConfiguration</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-delete.md)|<span data-ttu-id="d2462-122">None</span><span class="sxs-lookup"><span data-stu-id="d2462-122">None</span></span>|<span data-ttu-id="d2462-123">[Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d2462-123">Deletes a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>|
|[<span data-ttu-id="d2462-124">Windows10NetworkBoundaryConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d2462-124">Update windows10NetworkBoundaryConfiguration</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-update.md)|[<span data-ttu-id="d2462-125">windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2462-125">windows10NetworkBoundaryConfiguration</span></span>](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)|<span data-ttu-id="d2462-126">[Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2462-126">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2462-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2462-127">Properties</span></span>
|<span data-ttu-id="d2462-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2462-128">Property</span></span>|<span data-ttu-id="d2462-129">種類</span><span class="sxs-lookup"><span data-stu-id="d2462-129">Type</span></span>|<span data-ttu-id="d2462-130">説明</span><span class="sxs-lookup"><span data-stu-id="d2462-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2462-131">id</span><span class="sxs-lookup"><span data-stu-id="d2462-131">id</span></span>|<span data-ttu-id="d2462-132">文字列</span><span class="sxs-lookup"><span data-stu-id="d2462-132">String</span></span>|<span data-ttu-id="d2462-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d2462-133">Key of the entity.</span></span> <span data-ttu-id="d2462-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2462-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d2462-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2462-136">DateTimeOffset</span></span>|<span data-ttu-id="d2462-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d2462-137">DateTime the object was last modified.</span></span> <span data-ttu-id="d2462-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d2462-139">roleScopeTagIds</span></span>|<span data-ttu-id="d2462-140">String collection</span><span class="sxs-lookup"><span data-stu-id="d2462-140">String collection</span></span>|<span data-ttu-id="d2462-141">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="d2462-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d2462-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-143">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d2462-143">supportsScopeTags</span></span>|<span data-ttu-id="d2462-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2462-144">Boolean</span></span>|<span data-ttu-id="d2462-145">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2462-145">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d2462-146">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="d2462-146">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d2462-147">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="d2462-147">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d2462-148">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d2462-148">This property is read-only.</span></span> <span data-ttu-id="d2462-149">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2462-150">createdDateTime</span></span>|<span data-ttu-id="d2462-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2462-151">DateTimeOffset</span></span>|<span data-ttu-id="d2462-152">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d2462-152">DateTime the object was created.</span></span> <span data-ttu-id="d2462-153">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-154">description</span><span class="sxs-lookup"><span data-stu-id="d2462-154">description</span></span>|<span data-ttu-id="d2462-155">String</span><span class="sxs-lookup"><span data-stu-id="d2462-155">String</span></span>|<span data-ttu-id="d2462-156">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="d2462-156">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d2462-157">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-158">displayName</span><span class="sxs-lookup"><span data-stu-id="d2462-158">displayName</span></span>|<span data-ttu-id="d2462-159">String</span><span class="sxs-lookup"><span data-stu-id="d2462-159">String</span></span>|<span data-ttu-id="d2462-160">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d2462-160">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d2462-161">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-162">version</span><span class="sxs-lookup"><span data-stu-id="d2462-162">version</span></span>|<span data-ttu-id="d2462-163">Int32</span><span class="sxs-lookup"><span data-stu-id="d2462-163">Int32</span></span>|<span data-ttu-id="d2462-164">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d2462-164">Version of the device configuration.</span></span> <span data-ttu-id="d2462-165">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-165">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-166">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="d2462-166">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="d2462-167">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="d2462-167">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="d2462-168">Windows ネットワーク分離ポリシー</span><span class="sxs-lookup"><span data-stu-id="d2462-168">Windows Network Isolation Policy</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2462-169">関係</span><span class="sxs-lookup"><span data-stu-id="d2462-169">Relationships</span></span>
|<span data-ttu-id="d2462-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2462-170">Relationship</span></span>|<span data-ttu-id="d2462-171">型</span><span class="sxs-lookup"><span data-stu-id="d2462-171">Type</span></span>|<span data-ttu-id="d2462-172">説明</span><span class="sxs-lookup"><span data-stu-id="d2462-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2462-173">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="d2462-173">groupAssignments</span></span>|<span data-ttu-id="d2462-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d2462-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="d2462-175">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="d2462-175">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="d2462-176">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-177">assignments</span><span class="sxs-lookup"><span data-stu-id="d2462-177">assignments</span></span>|<span data-ttu-id="d2462-178">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d2462-178">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d2462-179">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="d2462-179">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="d2462-180">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-180">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-181">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d2462-181">deviceStatuses</span></span>|<span data-ttu-id="d2462-182">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d2462-182">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="d2462-183">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="d2462-183">Device configuration installation status by device.</span></span> <span data-ttu-id="d2462-184">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-184">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-185">userStatuses</span><span class="sxs-lookup"><span data-stu-id="d2462-185">userStatuses</span></span>|<span data-ttu-id="d2462-186">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d2462-186">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="d2462-187">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="d2462-187">Device configuration installation status by user.</span></span> <span data-ttu-id="d2462-188">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2462-188">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-189">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d2462-189">deviceStatusOverview</span></span>|[<span data-ttu-id="d2462-190">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d2462-190">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="d2462-191">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d2462-191">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-192">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d2462-192">userStatusOverview</span></span>|[<span data-ttu-id="d2462-193">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d2462-193">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="d2462-194">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d2462-194">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2462-195">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="d2462-195">deviceSettingStateSummaries</span></span>|<span data-ttu-id="d2462-196">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d2462-196">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="d2462-197">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d2462-197">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2462-198">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2462-198">JSON Representation</span></span>
<span data-ttu-id="d2462-199">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2462-199">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10NetworkBoundaryConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "String"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "String",
        "proxy": "String"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "String",
        "upperAddress": "String"
      }
    ],
    "enterpriseInternalProxyServers": [
      "String"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "String"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "String"
    ]
  }
}
```




