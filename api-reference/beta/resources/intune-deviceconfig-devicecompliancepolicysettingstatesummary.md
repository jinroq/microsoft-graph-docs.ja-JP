---
title: deviceCompliancePolicySettingStateSummary リソースの種類
description: アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb9802ecca80178eb98ca041d26d45b8688ebb36
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173158"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a><span data-ttu-id="e2d61-103">deviceCompliancePolicySettingStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2d61-103">deviceCompliancePolicySettingStateSummary resource type</span></span>

> <span data-ttu-id="e2d61-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2d61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2d61-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2d61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2d61-106">アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="e2d61-106">Device Compilance Policy Setting State summary across the account.</span></span>

## <a name="methods"></a><span data-ttu-id="e2d61-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e2d61-107">Methods</span></span>
|<span data-ttu-id="e2d61-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e2d61-108">Method</span></span>|<span data-ttu-id="e2d61-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e2d61-109">Return Type</span></span>|<span data-ttu-id="e2d61-110">説明</span><span class="sxs-lookup"><span data-stu-id="e2d61-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2d61-111">deviceCompliancePolicySettingStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="e2d61-111">List deviceCompliancePolicySettingStateSummaries</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|<span data-ttu-id="e2d61-112">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e2d61-112">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="e2d61-113">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e2d61-113">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="e2d61-114">deviceCompliancePolicySettingStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="e2d61-114">Get deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[<span data-ttu-id="e2d61-115">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="e2d61-115">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="e2d61-116">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e2d61-116">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="e2d61-117">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="e2d61-117">Create deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[<span data-ttu-id="e2d61-118">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="e2d61-118">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="e2d61-119">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e2d61-119">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="e2d61-120">deviceCompliancePolicySettingStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="e2d61-120">Delete deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|<span data-ttu-id="e2d61-121">なし</span><span class="sxs-lookup"><span data-stu-id="e2d61-121">None</span></span>|<span data-ttu-id="e2d61-122">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e2d61-122">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>|
|[<span data-ttu-id="e2d61-123">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="e2d61-123">Update deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[<span data-ttu-id="e2d61-124">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="e2d61-124">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="e2d61-125">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e2d61-125">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2d61-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2d61-126">Properties</span></span>
|<span data-ttu-id="e2d61-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2d61-127">Property</span></span>|<span data-ttu-id="e2d61-128">型</span><span class="sxs-lookup"><span data-stu-id="e2d61-128">Type</span></span>|<span data-ttu-id="e2d61-129">説明</span><span class="sxs-lookup"><span data-stu-id="e2d61-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2d61-130">id</span><span class="sxs-lookup"><span data-stu-id="e2d61-130">id</span></span>|<span data-ttu-id="e2d61-131">文字列</span><span class="sxs-lookup"><span data-stu-id="e2d61-131">String</span></span>|<span data-ttu-id="e2d61-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e2d61-132">Key of the entity.</span></span>|
|<span data-ttu-id="e2d61-133">setting</span><span class="sxs-lookup"><span data-stu-id="e2d61-133">setting</span></span>|<span data-ttu-id="e2d61-134">String</span><span class="sxs-lookup"><span data-stu-id="e2d61-134">String</span></span>|<span data-ttu-id="e2d61-135">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="e2d61-135">The setting class name and property name.</span></span>|
|<span data-ttu-id="e2d61-136">settingName</span><span class="sxs-lookup"><span data-stu-id="e2d61-136">settingName</span></span>|<span data-ttu-id="e2d61-137">String</span><span class="sxs-lookup"><span data-stu-id="e2d61-137">String</span></span>|<span data-ttu-id="e2d61-138">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="e2d61-138">Name of the setting.</span></span>|
|<span data-ttu-id="e2d61-139">platformType</span><span class="sxs-lookup"><span data-stu-id="e2d61-139">platformType</span></span>|[<span data-ttu-id="e2d61-140">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="e2d61-140">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="e2d61-141">プラットフォームを設定します。</span><span class="sxs-lookup"><span data-stu-id="e2d61-141">Setting platform.</span></span> <span data-ttu-id="e2d61-142">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="e2d61-142">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="e2d61-143">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e2d61-143">unknownDeviceCount</span></span>|<span data-ttu-id="e2d61-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e2d61-144">Int32</span></span>|<span data-ttu-id="e2d61-145">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e2d61-145">Number of unknown devices</span></span>|
|<span data-ttu-id="e2d61-146">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e2d61-146">notApplicableDeviceCount</span></span>|<span data-ttu-id="e2d61-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e2d61-147">Int32</span></span>|<span data-ttu-id="e2d61-148">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e2d61-148">Number of not applicable devices</span></span>|
|<span data-ttu-id="e2d61-149">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e2d61-149">compliantDeviceCount</span></span>|<span data-ttu-id="e2d61-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e2d61-150">Int32</span></span>|<span data-ttu-id="e2d61-151">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e2d61-151">Number of compliant devices</span></span>|
|<span data-ttu-id="e2d61-152">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e2d61-152">remediatedDeviceCount</span></span>|<span data-ttu-id="e2d61-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e2d61-153">Int32</span></span>|<span data-ttu-id="e2d61-154">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e2d61-154">Number of remediated devices</span></span>|
|<span data-ttu-id="e2d61-155">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e2d61-155">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e2d61-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e2d61-156">Int32</span></span>|<span data-ttu-id="e2d61-157">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e2d61-157">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e2d61-158">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e2d61-158">errorDeviceCount</span></span>|<span data-ttu-id="e2d61-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e2d61-159">Int32</span></span>|<span data-ttu-id="e2d61-160">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e2d61-160">Number of error devices</span></span>|
|<span data-ttu-id="e2d61-161">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e2d61-161">conflictDeviceCount</span></span>|<span data-ttu-id="e2d61-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e2d61-162">Int32</span></span>|<span data-ttu-id="e2d61-163">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e2d61-163">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2d61-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2d61-164">Relationships</span></span>
|<span data-ttu-id="e2d61-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2d61-165">Relationship</span></span>|<span data-ttu-id="e2d61-166">型</span><span class="sxs-lookup"><span data-stu-id="e2d61-166">Type</span></span>|<span data-ttu-id="e2d61-167">説明</span><span class="sxs-lookup"><span data-stu-id="e2d61-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2d61-168">deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="e2d61-168">deviceComplianceSettingStates</span></span>|<span data-ttu-id="e2d61-169">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e2d61-169">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="e2d61-170">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2d61-170">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2d61-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2d61-171">JSON Representation</span></span>
<span data-ttu-id="e2d61-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2d61-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```




