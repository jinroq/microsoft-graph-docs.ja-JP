---
title: deviceCompliancePolicy リソース タイプ
description: 'これは、コンプライアンス ポリシーの基本クラスです。 コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。 '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e556fd8619ef16b4212711511592de2b26e4772a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255613"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="801dc-104">deviceCompliancePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="801dc-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="801dc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="801dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="801dc-106">これは、コンプライアンス ポリシーの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="801dc-106">This is the base class for Compliance policy.</span></span> <span data-ttu-id="801dc-107">コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。</span><span class="sxs-lookup"><span data-stu-id="801dc-107">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="801dc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="801dc-108">Methods</span></span>
|<span data-ttu-id="801dc-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="801dc-109">Method</span></span>|<span data-ttu-id="801dc-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="801dc-110">Return Type</span></span>|<span data-ttu-id="801dc-111">説明</span><span class="sxs-lookup"><span data-stu-id="801dc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="801dc-112">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="801dc-112">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="801dc-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="801dc-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="801dc-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="801dc-114">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="801dc-115">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="801dc-115">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="801dc-116">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="801dc-116">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="801dc-117">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="801dc-117">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="801dc-118">assign action</span><span class="sxs-lookup"><span data-stu-id="801dc-118">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="801dc-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="801dc-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="801dc-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="801dc-120">Not yet documented</span></span>|
|[<span data-ttu-id="801dc-121">scheduleActionsForRules action</span><span class="sxs-lookup"><span data-stu-id="801dc-121">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="801dc-122">なし</span><span class="sxs-lookup"><span data-stu-id="801dc-122">None</span></span>|<span data-ttu-id="801dc-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="801dc-123">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="801dc-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="801dc-124">Properties</span></span>
|<span data-ttu-id="801dc-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="801dc-125">Property</span></span>|<span data-ttu-id="801dc-126">型</span><span class="sxs-lookup"><span data-stu-id="801dc-126">Type</span></span>|<span data-ttu-id="801dc-127">説明</span><span class="sxs-lookup"><span data-stu-id="801dc-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="801dc-128">id</span><span class="sxs-lookup"><span data-stu-id="801dc-128">id</span></span>|<span data-ttu-id="801dc-129">文字列</span><span class="sxs-lookup"><span data-stu-id="801dc-129">String</span></span>|<span data-ttu-id="801dc-130">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="801dc-130">Key of the entity.</span></span>|
|<span data-ttu-id="801dc-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="801dc-131">createdDateTime</span></span>|<span data-ttu-id="801dc-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="801dc-132">DateTimeOffset</span></span>|<span data-ttu-id="801dc-133">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="801dc-133">DateTime the object was created.</span></span>|
|<span data-ttu-id="801dc-134">説明</span><span class="sxs-lookup"><span data-stu-id="801dc-134">description</span></span>|<span data-ttu-id="801dc-135">String</span><span class="sxs-lookup"><span data-stu-id="801dc-135">String</span></span>|<span data-ttu-id="801dc-136">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="801dc-136">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="801dc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="801dc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="801dc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="801dc-138">DateTimeOffset</span></span>|<span data-ttu-id="801dc-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="801dc-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="801dc-140">displayName</span><span class="sxs-lookup"><span data-stu-id="801dc-140">displayName</span></span>|<span data-ttu-id="801dc-141">String</span><span class="sxs-lookup"><span data-stu-id="801dc-141">String</span></span>|<span data-ttu-id="801dc-142">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="801dc-142">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="801dc-143">version</span><span class="sxs-lookup"><span data-stu-id="801dc-143">version</span></span>|<span data-ttu-id="801dc-144">Int32</span><span class="sxs-lookup"><span data-stu-id="801dc-144">Int32</span></span>|<span data-ttu-id="801dc-145">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="801dc-145">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="801dc-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="801dc-146">Relationships</span></span>
|<span data-ttu-id="801dc-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="801dc-147">Relationship</span></span>|<span data-ttu-id="801dc-148">型</span><span class="sxs-lookup"><span data-stu-id="801dc-148">Type</span></span>|<span data-ttu-id="801dc-149">説明</span><span class="sxs-lookup"><span data-stu-id="801dc-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="801dc-150">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="801dc-150">scheduledActionsForRule</span></span>|<span data-ttu-id="801dc-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="801dc-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="801dc-152">このルールのスケジュール済みのアクションのリスト</span><span class="sxs-lookup"><span data-stu-id="801dc-152">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="801dc-153">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="801dc-153">deviceStatuses</span></span>|<span data-ttu-id="801dc-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="801dc-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="801dc-155">DeviceComplianceDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="801dc-155">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="801dc-156">userStatuses</span><span class="sxs-lookup"><span data-stu-id="801dc-156">userStatuses</span></span>|<span data-ttu-id="801dc-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="801dc-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="801dc-158">DeviceComplianceUserStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="801dc-158">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="801dc-159">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="801dc-159">deviceStatusOverview</span></span>|[<span data-ttu-id="801dc-160">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="801dc-160">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="801dc-161">デバイス コンプライアンスとデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="801dc-161">Device compliance devices status overview</span></span>|
|<span data-ttu-id="801dc-162">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="801dc-162">userStatusOverview</span></span>|[<span data-ttu-id="801dc-163">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="801dc-163">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="801dc-164">デバイス コンプライアンスとユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="801dc-164">Device compliance users status overview</span></span>|
|<span data-ttu-id="801dc-165">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="801dc-165">deviceSettingStateSummaries</span></span>|<span data-ttu-id="801dc-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="801dc-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="801dc-167">コンプライアンス設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="801dc-167">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="801dc-168">assignments</span><span class="sxs-lookup"><span data-stu-id="801dc-168">assignments</span></span>|<span data-ttu-id="801dc-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="801dc-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="801dc-170">このコンプライアンス ポリシーの割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="801dc-170">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="801dc-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="801dc-171">JSON Representation</span></span>
<span data-ttu-id="801dc-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="801dc-172">Here is a JSON representation of the resource.</span></span>
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



