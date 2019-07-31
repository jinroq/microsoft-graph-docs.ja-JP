---
title: deviceCompliancePolicySettingStateSummary リソースの種類
description: アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c086628d0d738eec025fc18442a8ee12609eb8e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970529"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a><span data-ttu-id="fa8e3-103">deviceCompliancePolicySettingStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa8e3-103">deviceCompliancePolicySettingStateSummary resource type</span></span>

> <span data-ttu-id="fa8e3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa8e3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa8e3-106">アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-106">Device Compilance Policy Setting State summary across the account.</span></span>

## <a name="methods"></a><span data-ttu-id="fa8e3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fa8e3-107">Methods</span></span>
|<span data-ttu-id="fa8e3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fa8e3-108">Method</span></span>|<span data-ttu-id="fa8e3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fa8e3-109">Return Type</span></span>|<span data-ttu-id="fa8e3-110">説明</span><span class="sxs-lookup"><span data-stu-id="fa8e3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fa8e3-111">deviceCompliancePolicySettingStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="fa8e3-111">List deviceCompliancePolicySettingStateSummaries</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|<span data-ttu-id="fa8e3-112">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fa8e3-112">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="fa8e3-113">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-113">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="fa8e3-114">deviceCompliancePolicySettingStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="fa8e3-114">Get deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[<span data-ttu-id="fa8e3-115">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa8e3-115">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="fa8e3-116">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-116">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="fa8e3-117">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="fa8e3-117">Create deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[<span data-ttu-id="fa8e3-118">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa8e3-118">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="fa8e3-119">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-119">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="fa8e3-120">deviceCompliancePolicySettingStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="fa8e3-120">Delete deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|<span data-ttu-id="fa8e3-121">なし</span><span class="sxs-lookup"><span data-stu-id="fa8e3-121">None</span></span>|<span data-ttu-id="fa8e3-122">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-122">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>|
|[<span data-ttu-id="fa8e3-123">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="fa8e3-123">Update deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[<span data-ttu-id="fa8e3-124">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa8e3-124">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="fa8e3-125">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-125">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa8e3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa8e3-126">Properties</span></span>
|<span data-ttu-id="fa8e3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa8e3-127">Property</span></span>|<span data-ttu-id="fa8e3-128">型</span><span class="sxs-lookup"><span data-stu-id="fa8e3-128">Type</span></span>|<span data-ttu-id="fa8e3-129">説明</span><span class="sxs-lookup"><span data-stu-id="fa8e3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa8e3-130">id</span><span class="sxs-lookup"><span data-stu-id="fa8e3-130">id</span></span>|<span data-ttu-id="fa8e3-131">String</span><span class="sxs-lookup"><span data-stu-id="fa8e3-131">String</span></span>|<span data-ttu-id="fa8e3-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-132">Key of the entity.</span></span>|
|<span data-ttu-id="fa8e3-133">setting</span><span class="sxs-lookup"><span data-stu-id="fa8e3-133">setting</span></span>|<span data-ttu-id="fa8e3-134">String</span><span class="sxs-lookup"><span data-stu-id="fa8e3-134">String</span></span>|<span data-ttu-id="fa8e3-135">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-135">The setting class name and property name.</span></span>|
|<span data-ttu-id="fa8e3-136">settingName</span><span class="sxs-lookup"><span data-stu-id="fa8e3-136">settingName</span></span>|<span data-ttu-id="fa8e3-137">String</span><span class="sxs-lookup"><span data-stu-id="fa8e3-137">String</span></span>|<span data-ttu-id="fa8e3-138">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-138">Name of the setting.</span></span>|
|<span data-ttu-id="fa8e3-139">platformType</span><span class="sxs-lookup"><span data-stu-id="fa8e3-139">platformType</span></span>|[<span data-ttu-id="fa8e3-140">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="fa8e3-140">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="fa8e3-141">プラットフォームを設定します。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-141">Setting platform.</span></span> <span data-ttu-id="fa8e3-142">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-142">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="fa8e3-143">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8e3-143">unknownDeviceCount</span></span>|<span data-ttu-id="fa8e3-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8e3-144">Int32</span></span>|<span data-ttu-id="fa8e3-145">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="fa8e3-145">Number of unknown devices</span></span>|
|<span data-ttu-id="fa8e3-146">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8e3-146">notApplicableDeviceCount</span></span>|<span data-ttu-id="fa8e3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8e3-147">Int32</span></span>|<span data-ttu-id="fa8e3-148">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="fa8e3-148">Number of not applicable devices</span></span>|
|<span data-ttu-id="fa8e3-149">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8e3-149">compliantDeviceCount</span></span>|<span data-ttu-id="fa8e3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8e3-150">Int32</span></span>|<span data-ttu-id="fa8e3-151">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="fa8e3-151">Number of compliant devices</span></span>|
|<span data-ttu-id="fa8e3-152">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8e3-152">remediatedDeviceCount</span></span>|<span data-ttu-id="fa8e3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8e3-153">Int32</span></span>|<span data-ttu-id="fa8e3-154">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="fa8e3-154">Number of remediated devices</span></span>|
|<span data-ttu-id="fa8e3-155">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8e3-155">nonCompliantDeviceCount</span></span>|<span data-ttu-id="fa8e3-156">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8e3-156">Int32</span></span>|<span data-ttu-id="fa8e3-157">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="fa8e3-157">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="fa8e3-158">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8e3-158">errorDeviceCount</span></span>|<span data-ttu-id="fa8e3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8e3-159">Int32</span></span>|<span data-ttu-id="fa8e3-160">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="fa8e3-160">Number of error devices</span></span>|
|<span data-ttu-id="fa8e3-161">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8e3-161">conflictDeviceCount</span></span>|<span data-ttu-id="fa8e3-162">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8e3-162">Int32</span></span>|<span data-ttu-id="fa8e3-163">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="fa8e3-163">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa8e3-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fa8e3-164">Relationships</span></span>
|<span data-ttu-id="fa8e3-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fa8e3-165">Relationship</span></span>|<span data-ttu-id="fa8e3-166">型</span><span class="sxs-lookup"><span data-stu-id="fa8e3-166">Type</span></span>|<span data-ttu-id="fa8e3-167">説明</span><span class="sxs-lookup"><span data-stu-id="fa8e3-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa8e3-168">deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="fa8e3-168">deviceComplianceSettingStates</span></span>|<span data-ttu-id="fa8e3-169">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fa8e3-169">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="fa8e3-170">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fa8e3-170">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa8e3-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa8e3-171">JSON Representation</span></span>
<span data-ttu-id="fa8e3-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa8e3-172">Here is a JSON representation of the resource.</span></span>
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





