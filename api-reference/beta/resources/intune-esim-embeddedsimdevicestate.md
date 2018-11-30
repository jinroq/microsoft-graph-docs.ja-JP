---
title: embeddedSIMDeviceState リソースの種類
description: デバイスに関連して埋め込み SIM アクティベーション コードの展開状態を説明します。
ms.openlocfilehash: 03d5d5d5dea85b3ecccf98fe57bc0611e2986063
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072800"
---
# <a name="embeddedsimdevicestate-resource-type"></a><span data-ttu-id="0194c-103">embeddedSIMDeviceState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0194c-103">embeddedSIMDeviceState resource type</span></span>

> <span data-ttu-id="0194c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0194c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0194c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0194c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0194c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0194c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0194c-107">デバイスに関連して埋め込み SIM アクティベーション コードの展開状態を説明します。</span><span class="sxs-lookup"><span data-stu-id="0194c-107">Describes the embedded SIM activation code deployment state in relation to a device.</span></span>
## <a name="methods"></a><span data-ttu-id="0194c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0194c-108">Methods</span></span>
|<span data-ttu-id="0194c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0194c-109">Method</span></span>|<span data-ttu-id="0194c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0194c-110">Return Type</span></span>|<span data-ttu-id="0194c-111">説明</span><span class="sxs-lookup"><span data-stu-id="0194c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0194c-112">リスト embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="0194c-112">List embeddedSIMDeviceStates</span></span>](../api/intune-esim-embeddedsimdevicestate-list.md)|<span data-ttu-id="0194c-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0194c-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="0194c-114">[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0194c-114">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="0194c-115">EmbeddedSIMDeviceState を取得します。</span><span class="sxs-lookup"><span data-stu-id="0194c-115">Get embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-get.md)|[<span data-ttu-id="0194c-116">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0194c-116">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="0194c-117">[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0194c-117">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0194c-118">EmbeddedSIMDeviceState を作成します。</span><span class="sxs-lookup"><span data-stu-id="0194c-118">Create embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-create.md)|[<span data-ttu-id="0194c-119">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0194c-119">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="0194c-120">新しい[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0194c-120">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0194c-121">EmbeddedSIMDeviceState を削除します。</span><span class="sxs-lookup"><span data-stu-id="0194c-121">Delete embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-delete.md)|<span data-ttu-id="0194c-122">なし</span><span class="sxs-lookup"><span data-stu-id="0194c-122">None</span></span>|<span data-ttu-id="0194c-123">の[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0194c-123">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>|
|[<span data-ttu-id="0194c-124">EmbeddedSIMDeviceState を更新します。</span><span class="sxs-lookup"><span data-stu-id="0194c-124">Update embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-update.md)|[<span data-ttu-id="0194c-125">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0194c-125">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="0194c-126">[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0194c-126">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0194c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0194c-127">Properties</span></span>
|<span data-ttu-id="0194c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0194c-128">Property</span></span>|<span data-ttu-id="0194c-129">型</span><span class="sxs-lookup"><span data-stu-id="0194c-129">Type</span></span>|<span data-ttu-id="0194c-130">説明</span><span class="sxs-lookup"><span data-stu-id="0194c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0194c-131">id</span><span class="sxs-lookup"><span data-stu-id="0194c-131">id</span></span>|<span data-ttu-id="0194c-132">String</span><span class="sxs-lookup"><span data-stu-id="0194c-132">String</span></span>|<span data-ttu-id="0194c-133">埋め込みの SIM のデバイスの状態の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="0194c-133">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="0194c-134">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="0194c-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0194c-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0194c-135">createdDateTime</span></span>|<span data-ttu-id="0194c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0194c-136">DateTimeOffset</span></span>|<span data-ttu-id="0194c-137">埋め込みの SIM のデバイスの状態が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="0194c-137">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="0194c-138">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="0194c-138">Generated service side.</span></span>|
|<span data-ttu-id="0194c-139">変更された日時</span><span class="sxs-lookup"><span data-stu-id="0194c-139">modifiedDateTime</span></span>|<span data-ttu-id="0194c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0194c-140">DateTimeOffset</span></span>|<span data-ttu-id="0194c-141">埋め込み SIM デバイスのステータスが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="0194c-141">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="0194c-142">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="0194c-142">Updated service side.</span></span>|
|<span data-ttu-id="0194c-143">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0194c-143">lastSyncDateTime</span></span>|<span data-ttu-id="0194c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0194c-144">DateTimeOffset</span></span>|<span data-ttu-id="0194c-145">SIM の埋め込みデバイスが最後にチェックインする時間です。</span><span class="sxs-lookup"><span data-stu-id="0194c-145">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="0194c-146">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="0194c-146">Updated service side.</span></span>|
|<span data-ttu-id="0194c-147">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="0194c-147">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="0194c-148">String</span><span class="sxs-lookup"><span data-stu-id="0194c-148">String</span></span>|<span data-ttu-id="0194c-149">汎用集積回路カードの識別子 (UICCID) を展開する先となるプロファイルは、ハードウェアを識別します。</span><span class="sxs-lookup"><span data-stu-id="0194c-149">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="0194c-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="0194c-150">deviceName</span></span>|<span data-ttu-id="0194c-151">String</span><span class="sxs-lookup"><span data-stu-id="0194c-151">String</span></span>|<span data-ttu-id="0194c-152">サブスクリプションには、デバイス名などのデスクトップでの準備</span><span class="sxs-lookup"><span data-stu-id="0194c-152">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="0194c-153">userName</span><span class="sxs-lookup"><span data-stu-id="0194c-153">userName</span></span>|<span data-ttu-id="0194c-154">String</span><span class="sxs-lookup"><span data-stu-id="0194c-154">String</span></span>|<span data-ttu-id="0194c-155">サブスクリプションが joe@contoso.com などに準備されているユーザー名</span><span class="sxs-lookup"><span data-stu-id="0194c-155">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="0194c-156">ステート</span><span class="sxs-lookup"><span data-stu-id="0194c-156">state</span></span>|[<span data-ttu-id="0194c-157">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="0194c-157">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="0194c-158">デバイスに適用されるプロファイルの操作の状態。</span><span class="sxs-lookup"><span data-stu-id="0194c-158">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="0194c-159">可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。</span><span class="sxs-lookup"><span data-stu-id="0194c-159">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="0194c-160">stateDetails</span><span class="sxs-lookup"><span data-stu-id="0194c-160">stateDetails</span></span>|<span data-ttu-id="0194c-161">String</span><span class="sxs-lookup"><span data-stu-id="0194c-161">String</span></span>|<span data-ttu-id="0194c-162">プロビジョニングの状態の説明の文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="0194c-162">String description of the provisioning state.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0194c-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0194c-163">Relationships</span></span>
<span data-ttu-id="0194c-164">なし</span><span class="sxs-lookup"><span data-stu-id="0194c-164">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0194c-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0194c-165">JSON Representation</span></span>
<span data-ttu-id="0194c-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0194c-166">Here is a JSON representation of the resource.</span></span>
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





