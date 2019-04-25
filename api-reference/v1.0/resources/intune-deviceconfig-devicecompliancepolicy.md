---
title: deviceCompliancePolicy リソース タイプ
description: 'これは、コンプライアンス ポリシーの基本クラスです。 コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。 '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e556fd8619ef16b4212711511592de2b26e4772a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534774"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="39086-104">deviceCompliancePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="39086-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="39086-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="39086-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39086-106">これは、コンプライアンス ポリシーの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="39086-106">This is the base class for Compliance policy.</span></span> <span data-ttu-id="39086-107">コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。</span><span class="sxs-lookup"><span data-stu-id="39086-107">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="39086-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="39086-108">Methods</span></span>
|<span data-ttu-id="39086-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="39086-109">Method</span></span>|<span data-ttu-id="39086-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="39086-110">Return Type</span></span>|<span data-ttu-id="39086-111">説明</span><span class="sxs-lookup"><span data-stu-id="39086-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39086-112">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="39086-112">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="39086-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39086-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="39086-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="39086-114">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="39086-115">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="39086-115">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="39086-116">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="39086-116">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="39086-117">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="39086-117">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="39086-118">assign action</span><span class="sxs-lookup"><span data-stu-id="39086-118">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="39086-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39086-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="39086-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="39086-120">Not yet documented</span></span>|
|[<span data-ttu-id="39086-121">scheduleActionsForRules action</span><span class="sxs-lookup"><span data-stu-id="39086-121">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="39086-122">なし</span><span class="sxs-lookup"><span data-stu-id="39086-122">None</span></span>|<span data-ttu-id="39086-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="39086-123">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="39086-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39086-124">Properties</span></span>
|<span data-ttu-id="39086-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39086-125">Property</span></span>|<span data-ttu-id="39086-126">型</span><span class="sxs-lookup"><span data-stu-id="39086-126">Type</span></span>|<span data-ttu-id="39086-127">説明</span><span class="sxs-lookup"><span data-stu-id="39086-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39086-128">id</span><span class="sxs-lookup"><span data-stu-id="39086-128">id</span></span>|<span data-ttu-id="39086-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="39086-129">String</span></span>|<span data-ttu-id="39086-130">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="39086-130">Key of the entity.</span></span>|
|<span data-ttu-id="39086-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39086-131">createdDateTime</span></span>|<span data-ttu-id="39086-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39086-132">DateTimeOffset</span></span>|<span data-ttu-id="39086-133">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="39086-133">DateTime the object was created.</span></span>|
|<span data-ttu-id="39086-134">description</span><span class="sxs-lookup"><span data-stu-id="39086-134">description</span></span>|<span data-ttu-id="39086-135">String</span><span class="sxs-lookup"><span data-stu-id="39086-135">String</span></span>|<span data-ttu-id="39086-136">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="39086-136">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="39086-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39086-137">lastModifiedDateTime</span></span>|<span data-ttu-id="39086-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39086-138">DateTimeOffset</span></span>|<span data-ttu-id="39086-139">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="39086-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="39086-140">displayName</span><span class="sxs-lookup"><span data-stu-id="39086-140">displayName</span></span>|<span data-ttu-id="39086-141">String</span><span class="sxs-lookup"><span data-stu-id="39086-141">String</span></span>|<span data-ttu-id="39086-142">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="39086-142">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="39086-143">version</span><span class="sxs-lookup"><span data-stu-id="39086-143">version</span></span>|<span data-ttu-id="39086-144">Int32</span><span class="sxs-lookup"><span data-stu-id="39086-144">Int32</span></span>|<span data-ttu-id="39086-145">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="39086-145">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39086-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39086-146">Relationships</span></span>
|<span data-ttu-id="39086-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39086-147">Relationship</span></span>|<span data-ttu-id="39086-148">型</span><span class="sxs-lookup"><span data-stu-id="39086-148">Type</span></span>|<span data-ttu-id="39086-149">説明</span><span class="sxs-lookup"><span data-stu-id="39086-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39086-150">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="39086-150">scheduledActionsForRule</span></span>|<span data-ttu-id="39086-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39086-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="39086-152">このルールのスケジュール済みのアクションのリスト</span><span class="sxs-lookup"><span data-stu-id="39086-152">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="39086-153">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="39086-153">deviceStatuses</span></span>|<span data-ttu-id="39086-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39086-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="39086-155">DeviceComplianceDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="39086-155">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="39086-156">userStatuses</span><span class="sxs-lookup"><span data-stu-id="39086-156">userStatuses</span></span>|<span data-ttu-id="39086-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39086-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="39086-158">DeviceComplianceUserStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="39086-158">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="39086-159">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="39086-159">deviceStatusOverview</span></span>|[<span data-ttu-id="39086-160">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="39086-160">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="39086-161">デバイス コンプライアンスとデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="39086-161">Device compliance devices status overview</span></span>|
|<span data-ttu-id="39086-162">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="39086-162">userStatusOverview</span></span>|[<span data-ttu-id="39086-163">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="39086-163">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="39086-164">デバイス コンプライアンスとユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="39086-164">Device compliance users status overview</span></span>|
|<span data-ttu-id="39086-165">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="39086-165">deviceSettingStateSummaries</span></span>|<span data-ttu-id="39086-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39086-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="39086-167">コンプライアンス設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="39086-167">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="39086-168">assignments</span><span class="sxs-lookup"><span data-stu-id="39086-168">assignments</span></span>|<span data-ttu-id="39086-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39086-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="39086-170">このコンプライアンス ポリシーの割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="39086-170">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39086-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39086-171">JSON Representation</span></span>
<span data-ttu-id="39086-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39086-172">Here is a JSON representation of the resource.</span></span>
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



