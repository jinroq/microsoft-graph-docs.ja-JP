---
title: deviceCompliancePolicy リソース タイプ
description: 'これは、コンプライアンス ポリシーの基本クラスです。 コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。 '
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a02fc8ab612011edf1ff6f2d1e281d8aeb8f8e6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407572"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="aaed4-104">deviceCompliancePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="aaed4-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="aaed4-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aaed4-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aaed4-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaed4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aaed4-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aaed4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaed4-108">これは、コンプライアンス ポリシーの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="aaed4-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="aaed4-109">コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。</span><span class="sxs-lookup"><span data-stu-id="aaed4-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="aaed4-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="aaed4-110">Methods</span></span>
|<span data-ttu-id="aaed4-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="aaed4-111">Method</span></span>|<span data-ttu-id="aaed4-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aaed4-112">Return Type</span></span>|<span data-ttu-id="aaed4-113">説明</span><span class="sxs-lookup"><span data-stu-id="aaed4-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aaed4-114">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="aaed4-114">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="aaed4-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="aaed4-116">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="aaed4-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="aaed4-117">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="aaed4-117">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="aaed4-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="aaed4-118">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="aaed4-119">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aaed4-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="aaed4-120">assign action</span><span class="sxs-lookup"><span data-stu-id="aaed4-120">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="aaed4-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="aaed4-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aaed4-122">Not yet documented</span></span>|
|[<span data-ttu-id="aaed4-123">scheduleActionsForRules action</span><span class="sxs-lookup"><span data-stu-id="aaed4-123">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="aaed4-124">なし</span><span class="sxs-lookup"><span data-stu-id="aaed4-124">None</span></span>|<span data-ttu-id="aaed4-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aaed4-125">Not yet documented</span></span>|
|[<span data-ttu-id="aaed4-126">refreshDeviceComplianceReportSummarization アクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-126">refreshDeviceComplianceReportSummarization action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|<span data-ttu-id="aaed4-127">なし</span><span class="sxs-lookup"><span data-stu-id="aaed4-127">None</span></span>|<span data-ttu-id="aaed4-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aaed4-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="aaed4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aaed4-129">Properties</span></span>
|<span data-ttu-id="aaed4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aaed4-130">Property</span></span>|<span data-ttu-id="aaed4-131">型</span><span class="sxs-lookup"><span data-stu-id="aaed4-131">Type</span></span>|<span data-ttu-id="aaed4-132">説明</span><span class="sxs-lookup"><span data-stu-id="aaed4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaed4-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aaed4-133">roleScopeTagIds</span></span>|<span data-ttu-id="aaed4-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-134">String collection</span></span>|<span data-ttu-id="aaed4-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="aaed4-135">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="aaed4-136">id</span><span class="sxs-lookup"><span data-stu-id="aaed4-136">id</span></span>|<span data-ttu-id="aaed4-137">String</span><span class="sxs-lookup"><span data-stu-id="aaed4-137">String</span></span>|<span data-ttu-id="aaed4-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aaed4-138">Key of the entity.</span></span>|
|<span data-ttu-id="aaed4-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aaed4-139">createdDateTime</span></span>|<span data-ttu-id="aaed4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaed4-140">DateTimeOffset</span></span>|<span data-ttu-id="aaed4-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="aaed4-141">DateTime the object was created.</span></span>|
|<span data-ttu-id="aaed4-142">説明</span><span class="sxs-lookup"><span data-stu-id="aaed4-142">description</span></span>|<span data-ttu-id="aaed4-143">String</span><span class="sxs-lookup"><span data-stu-id="aaed4-143">String</span></span>|<span data-ttu-id="aaed4-144">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="aaed4-144">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="aaed4-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaed4-145">lastModifiedDateTime</span></span>|<span data-ttu-id="aaed4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaed4-146">DateTimeOffset</span></span>|<span data-ttu-id="aaed4-147">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="aaed4-147">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="aaed4-148">displayName</span><span class="sxs-lookup"><span data-stu-id="aaed4-148">displayName</span></span>|<span data-ttu-id="aaed4-149">String</span><span class="sxs-lookup"><span data-stu-id="aaed4-149">String</span></span>|<span data-ttu-id="aaed4-150">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="aaed4-150">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="aaed4-151">version</span><span class="sxs-lookup"><span data-stu-id="aaed4-151">version</span></span>|<span data-ttu-id="aaed4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="aaed4-152">Int32</span></span>|<span data-ttu-id="aaed4-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="aaed4-153">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaed4-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aaed4-154">Relationships</span></span>
|<span data-ttu-id="aaed4-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aaed4-155">Relationship</span></span>|<span data-ttu-id="aaed4-156">型</span><span class="sxs-lookup"><span data-stu-id="aaed4-156">Type</span></span>|<span data-ttu-id="aaed4-157">説明</span><span class="sxs-lookup"><span data-stu-id="aaed4-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaed4-158">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="aaed4-158">scheduledActionsForRule</span></span>|<span data-ttu-id="aaed4-159">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-159">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="aaed4-160">このルールのスケジュール済みのアクションのリスト</span><span class="sxs-lookup"><span data-stu-id="aaed4-160">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="aaed4-161">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="aaed4-161">deviceStatuses</span></span>|<span data-ttu-id="aaed4-162">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-162">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="aaed4-163">DeviceComplianceDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="aaed4-163">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="aaed4-164">userStatuses</span><span class="sxs-lookup"><span data-stu-id="aaed4-164">userStatuses</span></span>|<span data-ttu-id="aaed4-165">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-165">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="aaed4-166">DeviceComplianceUserStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="aaed4-166">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="aaed4-167">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="aaed4-167">deviceStatusOverview</span></span>|[<span data-ttu-id="aaed4-168">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="aaed4-168">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="aaed4-169">デバイス コンプライアンスとデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="aaed4-169">Device compliance devices status overview</span></span>|
|<span data-ttu-id="aaed4-170">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="aaed4-170">userStatusOverview</span></span>|[<span data-ttu-id="aaed4-171">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="aaed4-171">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="aaed4-172">デバイス コンプライアンスとユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="aaed4-172">Device compliance users status overview</span></span>|
|<span data-ttu-id="aaed4-173">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="aaed4-173">deviceSettingStateSummaries</span></span>|<span data-ttu-id="aaed4-174">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-174">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="aaed4-175">コンプライアンス設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="aaed4-175">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="aaed4-176">assignments</span><span class="sxs-lookup"><span data-stu-id="aaed4-176">assignments</span></span>|<span data-ttu-id="aaed4-177">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aaed4-177">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="aaed4-178">このコンプライアンス ポリシーの割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="aaed4-178">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aaed4-179">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aaed4-179">JSON Representation</span></span>
<span data-ttu-id="aaed4-180">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aaed4-180">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




