---
title: deviceCompliancePolicy リソース タイプ
description: 'これは、コンプライアンス ポリシーの基本クラスです。 コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。 '
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f6204c6054974f454a4e3370bf7ffbbe5902eed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333171"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="c91c4-104">deviceCompliancePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c91c4-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="c91c4-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c91c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c91c4-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c91c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c91c4-107">これは、コンプライアンス ポリシーの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="c91c4-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="c91c4-108">コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。</span><span class="sxs-lookup"><span data-stu-id="c91c4-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="c91c4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c91c4-109">Methods</span></span>
|<span data-ttu-id="c91c4-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c91c4-110">Method</span></span>|<span data-ttu-id="c91c4-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c91c4-111">Return Type</span></span>|<span data-ttu-id="c91c4-112">説明</span><span class="sxs-lookup"><span data-stu-id="c91c4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c91c4-113">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="c91c4-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="c91c4-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="c91c4-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c91c4-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="c91c4-116">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c91c4-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="c91c4-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c91c4-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="c91c4-118">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c91c4-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="c91c4-119">assign action</span><span class="sxs-lookup"><span data-stu-id="c91c4-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="c91c4-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="c91c4-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c91c4-121">Not yet documented</span></span>|
|[<span data-ttu-id="c91c4-122">scheduleActionsForRules action</span><span class="sxs-lookup"><span data-stu-id="c91c4-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="c91c4-123">なし</span><span class="sxs-lookup"><span data-stu-id="c91c4-123">None</span></span>|<span data-ttu-id="c91c4-124">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c91c4-124">Not yet documented</span></span>|
|[<span data-ttu-id="c91c4-125">refreshDeviceComplianceReportSummarization アクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-125">refreshDeviceComplianceReportSummarization action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|<span data-ttu-id="c91c4-126">なし</span><span class="sxs-lookup"><span data-stu-id="c91c4-126">None</span></span>|<span data-ttu-id="c91c4-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c91c4-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c91c4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c91c4-128">Properties</span></span>
|<span data-ttu-id="c91c4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c91c4-129">Property</span></span>|<span data-ttu-id="c91c4-130">型</span><span class="sxs-lookup"><span data-stu-id="c91c4-130">Type</span></span>|<span data-ttu-id="c91c4-131">説明</span><span class="sxs-lookup"><span data-stu-id="c91c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c91c4-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c91c4-132">roleScopeTagIds</span></span>|<span data-ttu-id="c91c4-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-133">String collection</span></span>|<span data-ttu-id="c91c4-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c91c4-134">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="c91c4-135">id</span><span class="sxs-lookup"><span data-stu-id="c91c4-135">id</span></span>|<span data-ttu-id="c91c4-136">文字列</span><span class="sxs-lookup"><span data-stu-id="c91c4-136">String</span></span>|<span data-ttu-id="c91c4-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c91c4-137">Key of the entity.</span></span>|
|<span data-ttu-id="c91c4-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c91c4-138">createdDateTime</span></span>|<span data-ttu-id="c91c4-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c91c4-139">DateTimeOffset</span></span>|<span data-ttu-id="c91c4-140">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c91c4-140">DateTime the object was created.</span></span>|
|<span data-ttu-id="c91c4-141">description</span><span class="sxs-lookup"><span data-stu-id="c91c4-141">description</span></span>|<span data-ttu-id="c91c4-142">String</span><span class="sxs-lookup"><span data-stu-id="c91c4-142">String</span></span>|<span data-ttu-id="c91c4-143">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="c91c4-143">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c91c4-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c91c4-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c91c4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c91c4-145">DateTimeOffset</span></span>|<span data-ttu-id="c91c4-146">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="c91c4-146">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c91c4-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c91c4-147">displayName</span></span>|<span data-ttu-id="c91c4-148">String</span><span class="sxs-lookup"><span data-stu-id="c91c4-148">String</span></span>|<span data-ttu-id="c91c4-149">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="c91c4-149">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c91c4-150">version</span><span class="sxs-lookup"><span data-stu-id="c91c4-150">version</span></span>|<span data-ttu-id="c91c4-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c91c4-151">Int32</span></span>|<span data-ttu-id="c91c4-152">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c91c4-152">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c91c4-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c91c4-153">Relationships</span></span>
|<span data-ttu-id="c91c4-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c91c4-154">Relationship</span></span>|<span data-ttu-id="c91c4-155">型</span><span class="sxs-lookup"><span data-stu-id="c91c4-155">Type</span></span>|<span data-ttu-id="c91c4-156">説明</span><span class="sxs-lookup"><span data-stu-id="c91c4-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c91c4-157">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="c91c4-157">scheduledActionsForRule</span></span>|<span data-ttu-id="c91c4-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="c91c4-159">このルールのスケジュール済みのアクションのリスト</span><span class="sxs-lookup"><span data-stu-id="c91c4-159">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="c91c4-160">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c91c4-160">deviceStatuses</span></span>|<span data-ttu-id="c91c4-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="c91c4-162">DeviceComplianceDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="c91c4-162">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="c91c4-163">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c91c4-163">userStatuses</span></span>|<span data-ttu-id="c91c4-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="c91c4-165">DeviceComplianceUserStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="c91c4-165">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="c91c4-166">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c91c4-166">deviceStatusOverview</span></span>|[<span data-ttu-id="c91c4-167">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c91c4-167">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="c91c4-168">デバイス コンプライアンスとデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="c91c4-168">Device compliance devices status overview</span></span>|
|<span data-ttu-id="c91c4-169">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c91c4-169">userStatusOverview</span></span>|[<span data-ttu-id="c91c4-170">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="c91c4-170">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="c91c4-171">デバイス コンプライアンスとユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="c91c4-171">Device compliance users status overview</span></span>|
|<span data-ttu-id="c91c4-172">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c91c4-172">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c91c4-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c91c4-174">コンプライアンス設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="c91c4-174">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="c91c4-175">assignments</span><span class="sxs-lookup"><span data-stu-id="c91c4-175">assignments</span></span>|<span data-ttu-id="c91c4-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c91c4-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="c91c4-177">このコンプライアンス ポリシーの割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="c91c4-177">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c91c4-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c91c4-178">JSON Representation</span></span>
<span data-ttu-id="c91c4-179">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c91c4-179">Here is a JSON representation of the resource.</span></span>
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



