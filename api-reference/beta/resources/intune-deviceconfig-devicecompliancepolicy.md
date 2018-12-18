---
title: deviceCompliancePolicy リソース タイプ
description: 'これは、コンプライアンス ポリシーの基本クラスです。 コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。 '
author: tfitzmac
ms.openlocfilehash: 6af25f0e72f43a91a7033329929773e9aad8be42
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326223"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="17420-104">deviceCompliancePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="17420-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="17420-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="17420-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17420-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17420-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17420-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="17420-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17420-108">これは、コンプライアンス ポリシーの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="17420-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="17420-109">コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。</span><span class="sxs-lookup"><span data-stu-id="17420-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 
## <a name="methods"></a><span data-ttu-id="17420-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="17420-110">Methods</span></span>
|<span data-ttu-id="17420-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="17420-111">Method</span></span>|<span data-ttu-id="17420-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="17420-112">Return Type</span></span>|<span data-ttu-id="17420-113">説明</span><span class="sxs-lookup"><span data-stu-id="17420-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="17420-114">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="17420-114">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="17420-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17420-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="17420-116">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="17420-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="17420-117">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="17420-117">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="17420-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="17420-118">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="17420-119">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="17420-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="17420-120">assign action</span><span class="sxs-lookup"><span data-stu-id="17420-120">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="17420-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17420-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="17420-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="17420-122">Not yet documented</span></span>|
|[<span data-ttu-id="17420-123">scheduleActionsForRules action</span><span class="sxs-lookup"><span data-stu-id="17420-123">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="17420-124">なし</span><span class="sxs-lookup"><span data-stu-id="17420-124">None</span></span>|<span data-ttu-id="17420-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="17420-125">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="17420-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17420-126">Properties</span></span>
|<span data-ttu-id="17420-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17420-127">Property</span></span>|<span data-ttu-id="17420-128">種類</span><span class="sxs-lookup"><span data-stu-id="17420-128">Type</span></span>|<span data-ttu-id="17420-129">説明</span><span class="sxs-lookup"><span data-stu-id="17420-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17420-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17420-130">roleScopeTagIds</span></span>|<span data-ttu-id="17420-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="17420-131">String collection</span></span>|<span data-ttu-id="17420-132">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="17420-132">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="17420-133">id</span><span class="sxs-lookup"><span data-stu-id="17420-133">id</span></span>|<span data-ttu-id="17420-134">String</span><span class="sxs-lookup"><span data-stu-id="17420-134">String</span></span>|<span data-ttu-id="17420-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="17420-135">Key of the entity.</span></span>|
|<span data-ttu-id="17420-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17420-136">createdDateTime</span></span>|<span data-ttu-id="17420-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17420-137">DateTimeOffset</span></span>|<span data-ttu-id="17420-138">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="17420-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="17420-139">説明</span><span class="sxs-lookup"><span data-stu-id="17420-139">description</span></span>|<span data-ttu-id="17420-140">String</span><span class="sxs-lookup"><span data-stu-id="17420-140">String</span></span>|<span data-ttu-id="17420-141">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="17420-141">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="17420-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17420-142">lastModifiedDateTime</span></span>|<span data-ttu-id="17420-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17420-143">DateTimeOffset</span></span>|<span data-ttu-id="17420-144">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="17420-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="17420-145">displayName</span><span class="sxs-lookup"><span data-stu-id="17420-145">displayName</span></span>|<span data-ttu-id="17420-146">String</span><span class="sxs-lookup"><span data-stu-id="17420-146">String</span></span>|<span data-ttu-id="17420-147">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="17420-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="17420-148">version</span><span class="sxs-lookup"><span data-stu-id="17420-148">version</span></span>|<span data-ttu-id="17420-149">Int32</span><span class="sxs-lookup"><span data-stu-id="17420-149">Int32</span></span>|<span data-ttu-id="17420-150">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="17420-150">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17420-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17420-151">Relationships</span></span>
|<span data-ttu-id="17420-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17420-152">Relationship</span></span>|<span data-ttu-id="17420-153">型</span><span class="sxs-lookup"><span data-stu-id="17420-153">Type</span></span>|<span data-ttu-id="17420-154">説明</span><span class="sxs-lookup"><span data-stu-id="17420-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17420-155">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="17420-155">scheduledActionsForRule</span></span>|<span data-ttu-id="17420-156">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17420-156">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="17420-157">このルールのスケジュール済みのアクションのリスト</span><span class="sxs-lookup"><span data-stu-id="17420-157">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="17420-158">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="17420-158">deviceStatuses</span></span>|<span data-ttu-id="17420-159">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17420-159">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="17420-160">DeviceComplianceDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="17420-160">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="17420-161">userStatuses</span><span class="sxs-lookup"><span data-stu-id="17420-161">userStatuses</span></span>|<span data-ttu-id="17420-162">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17420-162">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="17420-163">DeviceComplianceUserStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="17420-163">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="17420-164">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="17420-164">deviceStatusOverview</span></span>|[<span data-ttu-id="17420-165">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="17420-165">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="17420-166">デバイス コンプライアンスとデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="17420-166">Device compliance devices status overview</span></span>|
|<span data-ttu-id="17420-167">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="17420-167">userStatusOverview</span></span>|[<span data-ttu-id="17420-168">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="17420-168">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="17420-169">デバイス コンプライアンスとユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="17420-169">Device compliance users status overview</span></span>|
|<span data-ttu-id="17420-170">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="17420-170">deviceSettingStateSummaries</span></span>|<span data-ttu-id="17420-171">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17420-171">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="17420-172">コンプライアンス設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="17420-172">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="17420-173">assignments</span><span class="sxs-lookup"><span data-stu-id="17420-173">assignments</span></span>|<span data-ttu-id="17420-174">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17420-174">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="17420-175">このコンプライアンス ポリシーの割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="17420-175">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17420-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17420-176">JSON Representation</span></span>
<span data-ttu-id="17420-177">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17420-177">Here is a JSON representation of the resource.</span></span>
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





