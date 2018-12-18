---
title: deviceCompliancePolicySettingStateSummary リソースの種類
description: アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。
author: tfitzmac
ms.openlocfilehash: d070dd0021cd9529c55f6f4a31d8a61d0cb32413
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314953"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a><span data-ttu-id="6374b-103">deviceCompliancePolicySettingStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6374b-103">deviceCompliancePolicySettingStateSummary resource type</span></span>

> <span data-ttu-id="6374b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6374b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6374b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6374b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6374b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6374b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6374b-107">アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="6374b-107">Device Compilance Policy Setting State summary across the account.</span></span>
## <a name="methods"></a><span data-ttu-id="6374b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6374b-108">Methods</span></span>
|<span data-ttu-id="6374b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6374b-109">Method</span></span>|<span data-ttu-id="6374b-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6374b-110">Return Type</span></span>|<span data-ttu-id="6374b-111">説明</span><span class="sxs-lookup"><span data-stu-id="6374b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6374b-112">deviceCompliancePolicySettingStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="6374b-112">List deviceCompliancePolicySettingStateSummaries</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|<span data-ttu-id="6374b-113">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6374b-113">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="6374b-114">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6374b-114">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="6374b-115">deviceCompliancePolicySettingStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="6374b-115">Get deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[<span data-ttu-id="6374b-116">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6374b-116">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="6374b-117">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6374b-117">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="6374b-118">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="6374b-118">Create deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[<span data-ttu-id="6374b-119">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6374b-119">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="6374b-120">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6374b-120">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="6374b-121">deviceCompliancePolicySettingStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="6374b-121">Delete deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|<span data-ttu-id="6374b-122">なし</span><span class="sxs-lookup"><span data-stu-id="6374b-122">None</span></span>|<span data-ttu-id="6374b-123">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6374b-123">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>|
|[<span data-ttu-id="6374b-124">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="6374b-124">Update deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[<span data-ttu-id="6374b-125">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6374b-125">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="6374b-126">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6374b-126">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6374b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6374b-127">Properties</span></span>
|<span data-ttu-id="6374b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6374b-128">Property</span></span>|<span data-ttu-id="6374b-129">種類</span><span class="sxs-lookup"><span data-stu-id="6374b-129">Type</span></span>|<span data-ttu-id="6374b-130">説明</span><span class="sxs-lookup"><span data-stu-id="6374b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6374b-131">ID</span><span class="sxs-lookup"><span data-stu-id="6374b-131">id</span></span>|<span data-ttu-id="6374b-132">String</span><span class="sxs-lookup"><span data-stu-id="6374b-132">String</span></span>|<span data-ttu-id="6374b-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6374b-133">Key of the entity.</span></span>|
|<span data-ttu-id="6374b-134">setting</span><span class="sxs-lookup"><span data-stu-id="6374b-134">setting</span></span>|<span data-ttu-id="6374b-135">String</span><span class="sxs-lookup"><span data-stu-id="6374b-135">String</span></span>|<span data-ttu-id="6374b-136">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="6374b-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="6374b-137">settingName</span><span class="sxs-lookup"><span data-stu-id="6374b-137">settingName</span></span>|<span data-ttu-id="6374b-138">String</span><span class="sxs-lookup"><span data-stu-id="6374b-138">String</span></span>|<span data-ttu-id="6374b-139">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="6374b-139">Name of the setting.</span></span>|
|<span data-ttu-id="6374b-140">platformType</span><span class="sxs-lookup"><span data-stu-id="6374b-140">platformType</span></span>|[<span data-ttu-id="6374b-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="6374b-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="6374b-142">設定のプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="6374b-142">Setting platform.</span></span> <span data-ttu-id="6374b-143">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="6374b-143">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="6374b-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6374b-144">unknownDeviceCount</span></span>|<span data-ttu-id="6374b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6374b-145">Int32</span></span>|<span data-ttu-id="6374b-146">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6374b-146">Number of unknown devices</span></span>|
|<span data-ttu-id="6374b-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6374b-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="6374b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6374b-148">Int32</span></span>|<span data-ttu-id="6374b-149">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6374b-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="6374b-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6374b-150">compliantDeviceCount</span></span>|<span data-ttu-id="6374b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6374b-151">Int32</span></span>|<span data-ttu-id="6374b-152">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="6374b-152">Number of compliant devices</span></span>|
|<span data-ttu-id="6374b-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6374b-153">remediatedDeviceCount</span></span>|<span data-ttu-id="6374b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6374b-154">Int32</span></span>|<span data-ttu-id="6374b-155">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6374b-155">Number of remediated devices</span></span>|
|<span data-ttu-id="6374b-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6374b-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6374b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6374b-157">Int32</span></span>|<span data-ttu-id="6374b-158">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6374b-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="6374b-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6374b-159">errorDeviceCount</span></span>|<span data-ttu-id="6374b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6374b-160">Int32</span></span>|<span data-ttu-id="6374b-161">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="6374b-161">Number of error devices</span></span>|
|<span data-ttu-id="6374b-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6374b-162">conflictDeviceCount</span></span>|<span data-ttu-id="6374b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6374b-163">Int32</span></span>|<span data-ttu-id="6374b-164">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="6374b-164">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="6374b-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6374b-165">Relationships</span></span>
|<span data-ttu-id="6374b-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6374b-166">Relationship</span></span>|<span data-ttu-id="6374b-167">型</span><span class="sxs-lookup"><span data-stu-id="6374b-167">Type</span></span>|<span data-ttu-id="6374b-168">説明</span><span class="sxs-lookup"><span data-stu-id="6374b-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6374b-169">deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="6374b-169">deviceComplianceSettingStates</span></span>|<span data-ttu-id="6374b-170">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6374b-170">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="6374b-171">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6374b-171">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6374b-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6374b-172">JSON Representation</span></span>
<span data-ttu-id="6374b-173">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6374b-173">Here is a JSON representation of the resource.</span></span>
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





