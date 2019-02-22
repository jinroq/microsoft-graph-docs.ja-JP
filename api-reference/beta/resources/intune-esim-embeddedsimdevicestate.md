---
title: embeddedSIMDeviceState リソースの種類
description: デバイスに関して埋め込まれた SIM ライセンス認証コードの展開状態を記述します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c358fb343282bdb30b43226a02fe127c73613dcc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151059"
---
# <a name="embeddedsimdevicestate-resource-type"></a><span data-ttu-id="5dc70-103">embeddedSIMDeviceState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5dc70-103">embeddedSIMDeviceState resource type</span></span>

> <span data-ttu-id="5dc70-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5dc70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dc70-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5dc70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dc70-106">デバイスに関して埋め込まれた SIM ライセンス認証コードの展開状態を記述します。</span><span class="sxs-lookup"><span data-stu-id="5dc70-106">Describes the embedded SIM activation code deployment state in relation to a device.</span></span>

## <a name="methods"></a><span data-ttu-id="5dc70-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5dc70-107">Methods</span></span>
|<span data-ttu-id="5dc70-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5dc70-108">Method</span></span>|<span data-ttu-id="5dc70-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5dc70-109">Return Type</span></span>|<span data-ttu-id="5dc70-110">説明</span><span class="sxs-lookup"><span data-stu-id="5dc70-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5dc70-111">リスト embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="5dc70-111">List embeddedSIMDeviceStates</span></span>](../api/intune-esim-embeddedsimdevicestate-list.md)|<span data-ttu-id="5dc70-112">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5dc70-112">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="5dc70-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5dc70-113">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="5dc70-114">embeddedSIMDeviceState を取得する</span><span class="sxs-lookup"><span data-stu-id="5dc70-114">Get embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-get.md)|[<span data-ttu-id="5dc70-115">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5dc70-115">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="5dc70-116">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5dc70-116">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="5dc70-117">embeddedSIMDeviceState を作成する</span><span class="sxs-lookup"><span data-stu-id="5dc70-117">Create embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-create.md)|[<span data-ttu-id="5dc70-118">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5dc70-118">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="5dc70-119">新しい[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5dc70-119">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="5dc70-120">embeddedSIMDeviceState の削除</span><span class="sxs-lookup"><span data-stu-id="5dc70-120">Delete embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-delete.md)|<span data-ttu-id="5dc70-121">なし</span><span class="sxs-lookup"><span data-stu-id="5dc70-121">None</span></span>|<span data-ttu-id="5dc70-122">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5dc70-122">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>|
|[<span data-ttu-id="5dc70-123">embeddedSIMDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="5dc70-123">Update embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-update.md)|[<span data-ttu-id="5dc70-124">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5dc70-124">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="5dc70-125">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5dc70-125">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5dc70-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5dc70-126">Properties</span></span>
|<span data-ttu-id="5dc70-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5dc70-127">Property</span></span>|<span data-ttu-id="5dc70-128">型</span><span class="sxs-lookup"><span data-stu-id="5dc70-128">Type</span></span>|<span data-ttu-id="5dc70-129">説明</span><span class="sxs-lookup"><span data-stu-id="5dc70-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc70-130">id</span><span class="sxs-lookup"><span data-stu-id="5dc70-130">id</span></span>|<span data-ttu-id="5dc70-131">文字列</span><span class="sxs-lookup"><span data-stu-id="5dc70-131">String</span></span>|<span data-ttu-id="5dc70-132">埋め込まれている SIM デバイスの状態を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5dc70-132">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="5dc70-133">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="5dc70-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="5dc70-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5dc70-134">createdDateTime</span></span>|<span data-ttu-id="5dc70-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dc70-135">DateTimeOffset</span></span>|<span data-ttu-id="5dc70-136">埋め込み SIM デバイスの状態が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="5dc70-136">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="5dc70-137">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="5dc70-137">Generated service side.</span></span>|
|<span data-ttu-id="5dc70-138">変更された日時</span><span class="sxs-lookup"><span data-stu-id="5dc70-138">modifiedDateTime</span></span>|<span data-ttu-id="5dc70-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dc70-139">DateTimeOffset</span></span>|<span data-ttu-id="5dc70-140">埋め込み SIM デバイスの状態が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="5dc70-140">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="5dc70-141">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="5dc70-141">Updated service side.</span></span>|
|<span data-ttu-id="5dc70-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5dc70-142">lastSyncDateTime</span></span>|<span data-ttu-id="5dc70-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dc70-143">DateTimeOffset</span></span>|<span data-ttu-id="5dc70-144">埋め込まれた SIM デバイスが最後にチェックインされた時刻。</span><span class="sxs-lookup"><span data-stu-id="5dc70-144">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="5dc70-145">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="5dc70-145">Updated service side.</span></span>|
|<span data-ttu-id="5dc70-146">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="5dc70-146">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="5dc70-147">String</span><span class="sxs-lookup"><span data-stu-id="5dc70-147">String</span></span>|<span data-ttu-id="5dc70-148">プロファイルが展開されるハードウェアを識別するユニバーサル統合回路カード識別子 (UICCID)。</span><span class="sxs-lookup"><span data-stu-id="5dc70-148">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="5dc70-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="5dc70-149">deviceName</span></span>|<span data-ttu-id="5dc70-150">String</span><span class="sxs-lookup"><span data-stu-id="5dc70-150">String</span></span>|<span data-ttu-id="5dc70-151">サブスクリプションが準備されたデバイス名 (デスクトップの例: JOE)</span><span class="sxs-lookup"><span data-stu-id="5dc70-151">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="5dc70-152">userName</span><span class="sxs-lookup"><span data-stu-id="5dc70-152">userName</span></span>|<span data-ttu-id="5dc70-153">String</span><span class="sxs-lookup"><span data-stu-id="5dc70-153">String</span></span>|<span data-ttu-id="5dc70-154">サブスクリプションが準備されたユーザー名 (joe@contoso.com など)</span><span class="sxs-lookup"><span data-stu-id="5dc70-154">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="5dc70-155">state</span><span class="sxs-lookup"><span data-stu-id="5dc70-155">state</span></span>|[<span data-ttu-id="5dc70-156">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="5dc70-156">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="5dc70-157">デバイスに適用されるプロファイル操作の状態。</span><span class="sxs-lookup"><span data-stu-id="5dc70-157">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="5dc70-158">可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。</span><span class="sxs-lookup"><span data-stu-id="5dc70-158">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="5dc70-159">statedetails</span><span class="sxs-lookup"><span data-stu-id="5dc70-159">stateDetails</span></span>|<span data-ttu-id="5dc70-160">String</span><span class="sxs-lookup"><span data-stu-id="5dc70-160">String</span></span>|<span data-ttu-id="5dc70-161">プロビジョニング状態の文字列の説明。</span><span class="sxs-lookup"><span data-stu-id="5dc70-161">String description of the provisioning state.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dc70-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5dc70-162">Relationships</span></span>
<span data-ttu-id="5dc70-163">なし</span><span class="sxs-lookup"><span data-stu-id="5dc70-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5dc70-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5dc70-164">JSON Representation</span></span>
<span data-ttu-id="5dc70-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5dc70-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "universalIntegratedCircuitCardIdentifier": "String",
  "deviceName": "String",
  "userName": "String",
  "state": "String",
  "stateDetails": "String"
}
```




