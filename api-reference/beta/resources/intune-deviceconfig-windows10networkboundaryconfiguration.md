---
title: windows10NetworkBoundaryConfiguration リソースの種類
description: Windows10 のネットワーク境界の構成
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a04da68368bff3c08629b5677457932730d08f8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990720"
---
# <a name="windows10networkboundaryconfiguration-resource-type"></a><span data-ttu-id="2a014-103">windows10NetworkBoundaryConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a014-103">windows10NetworkBoundaryConfiguration resource type</span></span>

> <span data-ttu-id="2a014-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2a014-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a014-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a014-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a014-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a014-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a014-107">Windows10 のネットワーク境界の構成</span><span class="sxs-lookup"><span data-stu-id="2a014-107">Windows10 Network Boundary Configuration</span></span>

<span data-ttu-id="2a014-108">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2a014-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a014-109">Methods</span></span>
|<span data-ttu-id="2a014-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a014-110">Method</span></span>|<span data-ttu-id="2a014-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2a014-111">Return Type</span></span>|<span data-ttu-id="2a014-112">説明</span><span class="sxs-lookup"><span data-stu-id="2a014-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a014-113">リスト windows10NetworkBoundaryConfigurations</span><span class="sxs-lookup"><span data-stu-id="2a014-113">List windows10NetworkBoundaryConfigurations</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-list.md)|<span data-ttu-id="2a014-114">[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2a014-114">[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) collection</span></span>|<span data-ttu-id="2a014-115">[Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2a014-115">List properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="2a014-116">Windows10NetworkBoundaryConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="2a014-116">Get windows10NetworkBoundaryConfiguration</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-get.md)|[<span data-ttu-id="2a014-117">windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a014-117">windows10NetworkBoundaryConfiguration</span></span>](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)|<span data-ttu-id="2a014-118">[Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a014-118">Read properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2a014-119">Windows10NetworkBoundaryConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="2a014-119">Create windows10NetworkBoundaryConfiguration</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-create.md)|[<span data-ttu-id="2a014-120">windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a014-120">windows10NetworkBoundaryConfiguration</span></span>](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)|<span data-ttu-id="2a014-121">新しい[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2a014-121">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2a014-122">Windows10NetworkBoundaryConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="2a014-122">Delete windows10NetworkBoundaryConfiguration</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-delete.md)|<span data-ttu-id="2a014-123">なし</span><span class="sxs-lookup"><span data-stu-id="2a014-123">None</span></span>|<span data-ttu-id="2a014-124">の[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="2a014-124">Deletes a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>|
|[<span data-ttu-id="2a014-125">Windows10NetworkBoundaryConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="2a014-125">Update windows10NetworkBoundaryConfiguration</span></span>](../api/intune-deviceconfig-windows10networkboundaryconfiguration-update.md)|[<span data-ttu-id="2a014-126">windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a014-126">windows10NetworkBoundaryConfiguration</span></span>](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)|<span data-ttu-id="2a014-127">[Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2a014-127">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a014-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a014-128">Properties</span></span>
|<span data-ttu-id="2a014-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a014-129">Property</span></span>|<span data-ttu-id="2a014-130">型</span><span class="sxs-lookup"><span data-stu-id="2a014-130">Type</span></span>|<span data-ttu-id="2a014-131">説明</span><span class="sxs-lookup"><span data-stu-id="2a014-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a014-132">ID</span><span class="sxs-lookup"><span data-stu-id="2a014-132">id</span></span>|<span data-ttu-id="2a014-133">String</span><span class="sxs-lookup"><span data-stu-id="2a014-133">String</span></span>|<span data-ttu-id="2a014-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2a014-134">Key of the entity.</span></span> <span data-ttu-id="2a014-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a014-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2a014-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a014-137">DateTimeOffset</span></span>|<span data-ttu-id="2a014-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2a014-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2a014-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2a014-140">roleScopeTagIds</span></span>|<span data-ttu-id="2a014-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2a014-141">String collection</span></span>|<span data-ttu-id="2a014-142">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="2a014-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2a014-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2a014-144">supportsScopeTags</span></span>|<span data-ttu-id="2a014-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a014-145">Boolean</span></span>|<span data-ttu-id="2a014-146">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a014-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2a014-147">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="2a014-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2a014-148">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="2a014-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2a014-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2a014-149">This property is read-only.</span></span> <span data-ttu-id="2a014-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a014-151">createdDateTime</span></span>|<span data-ttu-id="2a014-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a014-152">DateTimeOffset</span></span>|<span data-ttu-id="2a014-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2a014-153">DateTime the object was created.</span></span> <span data-ttu-id="2a014-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-155">説明</span><span class="sxs-lookup"><span data-stu-id="2a014-155">description</span></span>|<span data-ttu-id="2a014-156">String</span><span class="sxs-lookup"><span data-stu-id="2a014-156">String</span></span>|<span data-ttu-id="2a014-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="2a014-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2a014-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2a014-159">displayName</span></span>|<span data-ttu-id="2a014-160">String</span><span class="sxs-lookup"><span data-stu-id="2a014-160">String</span></span>|<span data-ttu-id="2a014-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="2a014-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2a014-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-163">version</span><span class="sxs-lookup"><span data-stu-id="2a014-163">version</span></span>|<span data-ttu-id="2a014-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2a014-164">Int32</span></span>|<span data-ttu-id="2a014-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2a014-165">Version of the device configuration.</span></span> <span data-ttu-id="2a014-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-167">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="2a014-167">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="2a014-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="2a014-168">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="2a014-169">Windows ネットワークの分離のポリシー</span><span class="sxs-lookup"><span data-stu-id="2a014-169">Windows Network Isolation Policy</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a014-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a014-170">Relationships</span></span>
|<span data-ttu-id="2a014-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a014-171">Relationship</span></span>|<span data-ttu-id="2a014-172">型</span><span class="sxs-lookup"><span data-stu-id="2a014-172">Type</span></span>|<span data-ttu-id="2a014-173">説明</span><span class="sxs-lookup"><span data-stu-id="2a014-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a014-174">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="2a014-174">groupAssignments</span></span>|<span data-ttu-id="2a014-175">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2a014-175">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="2a014-176">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="2a014-176">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="2a014-177">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-177">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-178">assignments</span><span class="sxs-lookup"><span data-stu-id="2a014-178">assignments</span></span>|<span data-ttu-id="2a014-179">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2a014-179">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2a014-180">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="2a014-180">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="2a014-181">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-181">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-182">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="2a014-182">deviceStatuses</span></span>|<span data-ttu-id="2a014-183">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2a014-183">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="2a014-184">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="2a014-184">Device configuration installation status by device.</span></span> <span data-ttu-id="2a014-185">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-185">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-186">userStatuses</span><span class="sxs-lookup"><span data-stu-id="2a014-186">userStatuses</span></span>|<span data-ttu-id="2a014-187">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2a014-187">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="2a014-188">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="2a014-188">Device configuration installation status by user.</span></span> <span data-ttu-id="2a014-189">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2a014-189">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-190">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="2a014-190">deviceStatusOverview</span></span>|[<span data-ttu-id="2a014-191">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2a014-191">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="2a014-192">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2a014-192">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-193">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="2a014-193">userStatusOverview</span></span>|[<span data-ttu-id="2a014-194">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="2a014-194">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="2a014-195">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2a014-195">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a014-196">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="2a014-196">deviceSettingStateSummaries</span></span>|<span data-ttu-id="2a014-197">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2a014-197">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="2a014-198">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2a014-198">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a014-199">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a014-199">JSON Representation</span></span>
<span data-ttu-id="2a014-200">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a014-200">Here is a JSON representation of the resource.</span></span>
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





