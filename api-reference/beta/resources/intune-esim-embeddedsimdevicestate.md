---
title: embeddedSIMDeviceState リソースの種類
description: デバイスに関して埋め込まれた SIM ライセンス認証コードの展開状態を記述します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cd14c92e5619cbce071190b966d3274386cec89
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568774"
---
# <a name="embeddedsimdevicestate-resource-type"></a><span data-ttu-id="f6bdf-103">embeddedSIMDeviceState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6bdf-103">embeddedSIMDeviceState resource type</span></span>

> <span data-ttu-id="f6bdf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6bdf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6bdf-106">デバイスに関して埋め込まれた SIM ライセンス認証コードの展開状態を記述します。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-106">Describes the embedded SIM activation code deployment state in relation to a device.</span></span>

## <a name="methods"></a><span data-ttu-id="f6bdf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f6bdf-107">Methods</span></span>
|<span data-ttu-id="f6bdf-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f6bdf-108">Method</span></span>|<span data-ttu-id="f6bdf-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f6bdf-109">Return Type</span></span>|<span data-ttu-id="f6bdf-110">説明</span><span class="sxs-lookup"><span data-stu-id="f6bdf-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6bdf-111">リスト embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="f6bdf-111">List embeddedSIMDeviceStates</span></span>](../api/intune-esim-embeddedsimdevicestate-list.md)|<span data-ttu-id="f6bdf-112">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f6bdf-112">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="f6bdf-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-113">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="f6bdf-114">embeddedSIMDeviceState を取得する</span><span class="sxs-lookup"><span data-stu-id="f6bdf-114">Get embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-get.md)|[<span data-ttu-id="f6bdf-115">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="f6bdf-115">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="f6bdf-116">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-116">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="f6bdf-117">embeddedSIMDeviceState を作成する</span><span class="sxs-lookup"><span data-stu-id="f6bdf-117">Create embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-create.md)|[<span data-ttu-id="f6bdf-118">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="f6bdf-118">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="f6bdf-119">新しい[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-119">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="f6bdf-120">embeddedSIMDeviceState の削除</span><span class="sxs-lookup"><span data-stu-id="f6bdf-120">Delete embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-delete.md)|<span data-ttu-id="f6bdf-121">なし</span><span class="sxs-lookup"><span data-stu-id="f6bdf-121">None</span></span>|<span data-ttu-id="f6bdf-122">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-122">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>|
|[<span data-ttu-id="f6bdf-123">embeddedSIMDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="f6bdf-123">Update embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-update.md)|[<span data-ttu-id="f6bdf-124">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="f6bdf-124">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="f6bdf-125">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-125">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6bdf-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6bdf-126">Properties</span></span>
|<span data-ttu-id="f6bdf-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6bdf-127">Property</span></span>|<span data-ttu-id="f6bdf-128">型</span><span class="sxs-lookup"><span data-stu-id="f6bdf-128">Type</span></span>|<span data-ttu-id="f6bdf-129">説明</span><span class="sxs-lookup"><span data-stu-id="f6bdf-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6bdf-130">id</span><span class="sxs-lookup"><span data-stu-id="f6bdf-130">id</span></span>|<span data-ttu-id="f6bdf-131">String</span><span class="sxs-lookup"><span data-stu-id="f6bdf-131">String</span></span>|<span data-ttu-id="f6bdf-132">埋め込まれている SIM デバイスの状態を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-132">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="f6bdf-133">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="f6bdf-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6bdf-134">createdDateTime</span></span>|<span data-ttu-id="f6bdf-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6bdf-135">DateTimeOffset</span></span>|<span data-ttu-id="f6bdf-136">埋め込み SIM デバイスの状態が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-136">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="f6bdf-137">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-137">Generated service side.</span></span>|
|<span data-ttu-id="f6bdf-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6bdf-138">modifiedDateTime</span></span>|<span data-ttu-id="f6bdf-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6bdf-139">DateTimeOffset</span></span>|<span data-ttu-id="f6bdf-140">埋め込み SIM デバイスの状態が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-140">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="f6bdf-141">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-141">Updated service side.</span></span>|
|<span data-ttu-id="f6bdf-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f6bdf-142">lastSyncDateTime</span></span>|<span data-ttu-id="f6bdf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6bdf-143">DateTimeOffset</span></span>|<span data-ttu-id="f6bdf-144">埋め込まれた SIM デバイスが最後にチェックインされた時刻。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-144">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="f6bdf-145">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-145">Updated service side.</span></span>|
|<span data-ttu-id="f6bdf-146">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="f6bdf-146">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="f6bdf-147">String</span><span class="sxs-lookup"><span data-stu-id="f6bdf-147">String</span></span>|<span data-ttu-id="f6bdf-148">プロファイルが展開されるハードウェアを識別するユニバーサル統合回路カード識別子 (UICCID)。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-148">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="f6bdf-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="f6bdf-149">deviceName</span></span>|<span data-ttu-id="f6bdf-150">String</span><span class="sxs-lookup"><span data-stu-id="f6bdf-150">String</span></span>|<span data-ttu-id="f6bdf-151">サブスクリプションが準備されたデバイス名 (デスクトップの例: JOE)</span><span class="sxs-lookup"><span data-stu-id="f6bdf-151">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="f6bdf-152">userName</span><span class="sxs-lookup"><span data-stu-id="f6bdf-152">userName</span></span>|<span data-ttu-id="f6bdf-153">String</span><span class="sxs-lookup"><span data-stu-id="f6bdf-153">String</span></span>|<span data-ttu-id="f6bdf-154">サブスクリプションが準備されたユーザー名 (joe@contoso.com など)</span><span class="sxs-lookup"><span data-stu-id="f6bdf-154">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="f6bdf-155">state</span><span class="sxs-lookup"><span data-stu-id="f6bdf-155">state</span></span>|[<span data-ttu-id="f6bdf-156">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="f6bdf-156">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="f6bdf-157">デバイスに適用されるプロファイル操作の状態。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-157">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="f6bdf-158">可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-158">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="f6bdf-159">statedetails</span><span class="sxs-lookup"><span data-stu-id="f6bdf-159">stateDetails</span></span>|<span data-ttu-id="f6bdf-160">String</span><span class="sxs-lookup"><span data-stu-id="f6bdf-160">String</span></span>|<span data-ttu-id="f6bdf-161">プロビジョニング状態の文字列の説明。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-161">String description of the provisioning state.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6bdf-162">関係</span><span class="sxs-lookup"><span data-stu-id="f6bdf-162">Relationships</span></span>
<span data-ttu-id="f6bdf-163">なし</span><span class="sxs-lookup"><span data-stu-id="f6bdf-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6bdf-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6bdf-164">JSON Representation</span></span>
<span data-ttu-id="f6bdf-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f6bdf-165">Here is a JSON representation of the resource.</span></span>
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





