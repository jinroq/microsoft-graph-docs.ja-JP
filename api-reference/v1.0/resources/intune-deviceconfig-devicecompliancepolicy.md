---
title: deviceCompliancePolicy リソース タイプ
description: 'これは、コンプライアンス ポリシーの基本クラスです。 コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。 '
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2ab919a24c7c2819963ce047612f5a829913060
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834413"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="7398a-104">deviceCompliancePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="7398a-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="7398a-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7398a-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7398a-106">これは、コンプライアンス ポリシーの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="7398a-106">This is the base class for Compliance policy.</span></span> <span data-ttu-id="7398a-107">コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。</span><span class="sxs-lookup"><span data-stu-id="7398a-107">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 
## <a name="methods"></a><span data-ttu-id="7398a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7398a-108">Methods</span></span>
|<span data-ttu-id="7398a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7398a-109">Method</span></span>|<span data-ttu-id="7398a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7398a-110">Return Type</span></span>|<span data-ttu-id="7398a-111">説明</span><span class="sxs-lookup"><span data-stu-id="7398a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7398a-112">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="7398a-112">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="7398a-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7398a-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="7398a-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7398a-114">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="7398a-115">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7398a-115">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="7398a-116">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7398a-116">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="7398a-117">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7398a-117">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="7398a-118">assign action</span><span class="sxs-lookup"><span data-stu-id="7398a-118">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="7398a-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7398a-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="7398a-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7398a-120">Not yet documented</span></span>|
|[<span data-ttu-id="7398a-121">scheduleActionsForRules action</span><span class="sxs-lookup"><span data-stu-id="7398a-121">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="7398a-122">なし</span><span class="sxs-lookup"><span data-stu-id="7398a-122">None</span></span>|<span data-ttu-id="7398a-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7398a-123">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7398a-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7398a-124">Properties</span></span>
|<span data-ttu-id="7398a-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7398a-125">Property</span></span>|<span data-ttu-id="7398a-126">種類</span><span class="sxs-lookup"><span data-stu-id="7398a-126">Type</span></span>|<span data-ttu-id="7398a-127">説明</span><span class="sxs-lookup"><span data-stu-id="7398a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7398a-128">ID</span><span class="sxs-lookup"><span data-stu-id="7398a-128">id</span></span>|<span data-ttu-id="7398a-129">String</span><span class="sxs-lookup"><span data-stu-id="7398a-129">String</span></span>|<span data-ttu-id="7398a-130">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7398a-130">Key of the entity.</span></span>|
|<span data-ttu-id="7398a-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7398a-131">createdDateTime</span></span>|<span data-ttu-id="7398a-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7398a-132">DateTimeOffset</span></span>|<span data-ttu-id="7398a-133">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7398a-133">DateTime the object was created.</span></span>|
|<span data-ttu-id="7398a-134">説明</span><span class="sxs-lookup"><span data-stu-id="7398a-134">description</span></span>|<span data-ttu-id="7398a-135">String</span><span class="sxs-lookup"><span data-stu-id="7398a-135">String</span></span>|<span data-ttu-id="7398a-136">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="7398a-136">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="7398a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7398a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7398a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7398a-138">DateTimeOffset</span></span>|<span data-ttu-id="7398a-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7398a-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7398a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7398a-140">displayName</span></span>|<span data-ttu-id="7398a-141">String</span><span class="sxs-lookup"><span data-stu-id="7398a-141">String</span></span>|<span data-ttu-id="7398a-142">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="7398a-142">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="7398a-143">version</span><span class="sxs-lookup"><span data-stu-id="7398a-143">version</span></span>|<span data-ttu-id="7398a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7398a-144">Int32</span></span>|<span data-ttu-id="7398a-145">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7398a-145">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7398a-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7398a-146">Relationships</span></span>
|<span data-ttu-id="7398a-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7398a-147">Relationship</span></span>|<span data-ttu-id="7398a-148">型</span><span class="sxs-lookup"><span data-stu-id="7398a-148">Type</span></span>|<span data-ttu-id="7398a-149">説明</span><span class="sxs-lookup"><span data-stu-id="7398a-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7398a-150">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="7398a-150">scheduledActionsForRule</span></span>|<span data-ttu-id="7398a-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7398a-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="7398a-152">このルールのスケジュール済みのアクションのリスト</span><span class="sxs-lookup"><span data-stu-id="7398a-152">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="7398a-153">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7398a-153">deviceStatuses</span></span>|<span data-ttu-id="7398a-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7398a-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="7398a-155">DeviceComplianceDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="7398a-155">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="7398a-156">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7398a-156">userStatuses</span></span>|<span data-ttu-id="7398a-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7398a-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="7398a-158">DeviceComplianceUserStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="7398a-158">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="7398a-159">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7398a-159">deviceStatusOverview</span></span>|[<span data-ttu-id="7398a-160">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7398a-160">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="7398a-161">デバイス コンプライアンスとデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="7398a-161">Device compliance devices status overview</span></span>|
|<span data-ttu-id="7398a-162">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7398a-162">userStatusOverview</span></span>|[<span data-ttu-id="7398a-163">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="7398a-163">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="7398a-164">デバイス コンプライアンスとユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="7398a-164">Device compliance users status overview</span></span>|
|<span data-ttu-id="7398a-165">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="7398a-165">deviceSettingStateSummaries</span></span>|<span data-ttu-id="7398a-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7398a-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7398a-167">コンプライアンス設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="7398a-167">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="7398a-168">assignments</span><span class="sxs-lookup"><span data-stu-id="7398a-168">assignments</span></span>|<span data-ttu-id="7398a-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7398a-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="7398a-170">このコンプライアンス ポリシーの割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="7398a-170">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7398a-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7398a-171">JSON Representation</span></span>
<span data-ttu-id="7398a-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7398a-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



