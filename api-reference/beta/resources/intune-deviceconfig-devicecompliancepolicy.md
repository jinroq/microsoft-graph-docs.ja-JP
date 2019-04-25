---
title: deviceCompliancePolicy リソース タイプ
description: 'これは、コンプライアンス ポリシーの基本クラスです。 コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。 '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d17bbba221fd95405b2f92f05efa607787b28145
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566781"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="ebfa6-104">deviceCompliancePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="ebfa6-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="ebfa6-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebfa6-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebfa6-107">これは、コンプライアンス ポリシーの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="ebfa6-108">コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="ebfa6-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ebfa6-109">Methods</span></span>
|<span data-ttu-id="ebfa6-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="ebfa6-110">Method</span></span>|<span data-ttu-id="ebfa6-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ebfa6-111">Return Type</span></span>|<span data-ttu-id="ebfa6-112">説明</span><span class="sxs-lookup"><span data-stu-id="ebfa6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebfa6-113">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="ebfa6-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="ebfa6-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebfa6-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="ebfa6-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="ebfa6-116">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ebfa6-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="ebfa6-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ebfa6-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="ebfa6-118">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="ebfa6-119">assign action</span><span class="sxs-lookup"><span data-stu-id="ebfa6-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="ebfa6-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebfa6-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="ebfa6-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebfa6-121">Not yet documented</span></span>|
|[<span data-ttu-id="ebfa6-122">scheduleActionsForRules action</span><span class="sxs-lookup"><span data-stu-id="ebfa6-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="ebfa6-123">なし</span><span class="sxs-lookup"><span data-stu-id="ebfa6-123">None</span></span>|<span data-ttu-id="ebfa6-124">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebfa6-124">Not yet documented</span></span>|
|[<span data-ttu-id="ebfa6-125">refreshDeviceComplianceReportSummarization アクション</span><span class="sxs-lookup"><span data-stu-id="ebfa6-125">refreshDeviceComplianceReportSummarization action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|<span data-ttu-id="ebfa6-126">なし</span><span class="sxs-lookup"><span data-stu-id="ebfa6-126">None</span></span>|<span data-ttu-id="ebfa6-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebfa6-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ebfa6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebfa6-128">Properties</span></span>
|<span data-ttu-id="ebfa6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebfa6-129">Property</span></span>|<span data-ttu-id="ebfa6-130">型</span><span class="sxs-lookup"><span data-stu-id="ebfa6-130">Type</span></span>|<span data-ttu-id="ebfa6-131">説明</span><span class="sxs-lookup"><span data-stu-id="ebfa6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfa6-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ebfa6-132">roleScopeTagIds</span></span>|<span data-ttu-id="ebfa6-133">String collection</span><span class="sxs-lookup"><span data-stu-id="ebfa6-133">String collection</span></span>|<span data-ttu-id="ebfa6-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-134">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="ebfa6-135">id</span><span class="sxs-lookup"><span data-stu-id="ebfa6-135">id</span></span>|<span data-ttu-id="ebfa6-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ebfa6-136">String</span></span>|<span data-ttu-id="ebfa6-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-137">Key of the entity.</span></span>|
|<span data-ttu-id="ebfa6-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebfa6-138">createdDateTime</span></span>|<span data-ttu-id="ebfa6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebfa6-139">DateTimeOffset</span></span>|<span data-ttu-id="ebfa6-140">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-140">DateTime the object was created.</span></span>|
|<span data-ttu-id="ebfa6-141">説明</span><span class="sxs-lookup"><span data-stu-id="ebfa6-141">description</span></span>|<span data-ttu-id="ebfa6-142">String</span><span class="sxs-lookup"><span data-stu-id="ebfa6-142">String</span></span>|<span data-ttu-id="ebfa6-143">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-143">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="ebfa6-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebfa6-144">lastModifiedDateTime</span></span>|<span data-ttu-id="ebfa6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebfa6-145">DateTimeOffset</span></span>|<span data-ttu-id="ebfa6-146">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-146">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ebfa6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ebfa6-147">displayName</span></span>|<span data-ttu-id="ebfa6-148">String</span><span class="sxs-lookup"><span data-stu-id="ebfa6-148">String</span></span>|<span data-ttu-id="ebfa6-149">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-149">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ebfa6-150">version</span><span class="sxs-lookup"><span data-stu-id="ebfa6-150">version</span></span>|<span data-ttu-id="ebfa6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ebfa6-151">Int32</span></span>|<span data-ttu-id="ebfa6-152">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-152">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebfa6-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ebfa6-153">Relationships</span></span>
|<span data-ttu-id="ebfa6-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ebfa6-154">Relationship</span></span>|<span data-ttu-id="ebfa6-155">型</span><span class="sxs-lookup"><span data-stu-id="ebfa6-155">Type</span></span>|<span data-ttu-id="ebfa6-156">説明</span><span class="sxs-lookup"><span data-stu-id="ebfa6-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfa6-157">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="ebfa6-157">scheduledActionsForRule</span></span>|<span data-ttu-id="ebfa6-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebfa6-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="ebfa6-159">このルールのスケジュール済みのアクションのリスト</span><span class="sxs-lookup"><span data-stu-id="ebfa6-159">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="ebfa6-160">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ebfa6-160">deviceStatuses</span></span>|<span data-ttu-id="ebfa6-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebfa6-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="ebfa6-162">DeviceComplianceDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-162">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="ebfa6-163">userStatuses</span><span class="sxs-lookup"><span data-stu-id="ebfa6-163">userStatuses</span></span>|<span data-ttu-id="ebfa6-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebfa6-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="ebfa6-165">DeviceComplianceUserStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-165">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="ebfa6-166">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ebfa6-166">deviceStatusOverview</span></span>|[<span data-ttu-id="ebfa6-167">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebfa6-167">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="ebfa6-168">デバイス コンプライアンスとデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="ebfa6-168">Device compliance devices status overview</span></span>|
|<span data-ttu-id="ebfa6-169">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ebfa6-169">userStatusOverview</span></span>|[<span data-ttu-id="ebfa6-170">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ebfa6-170">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="ebfa6-171">デバイス コンプライアンスとユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="ebfa6-171">Device compliance users status overview</span></span>|
|<span data-ttu-id="ebfa6-172">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="ebfa6-172">deviceSettingStateSummaries</span></span>|<span data-ttu-id="ebfa6-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebfa6-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="ebfa6-174">コンプライアンス設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="ebfa6-174">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="ebfa6-175">assignments</span><span class="sxs-lookup"><span data-stu-id="ebfa6-175">assignments</span></span>|<span data-ttu-id="ebfa6-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ebfa6-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="ebfa6-177">このコンプライアンス ポリシーの割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-177">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebfa6-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebfa6-178">JSON Representation</span></span>
<span data-ttu-id="ebfa6-179">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ebfa6-179">Here is a JSON representation of the resource.</span></span>
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





