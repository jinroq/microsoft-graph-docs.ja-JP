---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
ms.openlocfilehash: 467970b31709b8ab7ca48e786326b89c8ee73733
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021717"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="cb555-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb555-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="cb555-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb555-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb555-105">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="cb555-105">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="cb555-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cb555-106">Methods</span></span>
|<span data-ttu-id="cb555-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cb555-107">Method</span></span>|<span data-ttu-id="cb555-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cb555-108">Return Type</span></span>|<span data-ttu-id="cb555-109">説明</span><span class="sxs-lookup"><span data-stu-id="cb555-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb555-110">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="cb555-110">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="cb555-111">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb555-111">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="cb555-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cb555-112">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="cb555-113">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="cb555-113">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="cb555-114">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cb555-114">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="cb555-115">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cb555-115">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="cb555-116">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="cb555-116">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="cb555-117">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cb555-117">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="cb555-118">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cb555-118">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="cb555-119">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="cb555-119">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="cb555-120">なし</span><span class="sxs-lookup"><span data-stu-id="cb555-120">None</span></span>|<span data-ttu-id="cb555-121">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="cb555-121">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="cb555-122">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="cb555-122">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="cb555-123">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cb555-123">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="cb555-124">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cb555-124">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb555-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb555-125">Properties</span></span>
|<span data-ttu-id="cb555-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb555-126">Property</span></span>|<span data-ttu-id="cb555-127">型</span><span class="sxs-lookup"><span data-stu-id="cb555-127">Type</span></span>|<span data-ttu-id="cb555-128">説明</span><span class="sxs-lookup"><span data-stu-id="cb555-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb555-129">id</span><span class="sxs-lookup"><span data-stu-id="cb555-129">id</span></span>|<span data-ttu-id="cb555-130">String</span><span class="sxs-lookup"><span data-stu-id="cb555-130">String</span></span>|<span data-ttu-id="cb555-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cb555-131">Key of the entity.</span></span>|
|<span data-ttu-id="cb555-132">settingName</span><span class="sxs-lookup"><span data-stu-id="cb555-132">settingName</span></span>|<span data-ttu-id="cb555-133">String</span><span class="sxs-lookup"><span data-stu-id="cb555-133">String</span></span>|<span data-ttu-id="cb555-134">設定の名前</span><span class="sxs-lookup"><span data-stu-id="cb555-134">Name of the setting</span></span>|
|<span data-ttu-id="cb555-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="cb555-135">instancePath</span></span>|<span data-ttu-id="cb555-136">String</span><span class="sxs-lookup"><span data-stu-id="cb555-136">String</span></span>|<span data-ttu-id="cb555-137">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="cb555-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="cb555-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb555-138">unknownDeviceCount</span></span>|<span data-ttu-id="cb555-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cb555-139">Int32</span></span>|<span data-ttu-id="cb555-140">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cb555-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="cb555-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb555-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="cb555-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cb555-142">Int32</span></span>|<span data-ttu-id="cb555-143">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cb555-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="cb555-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb555-144">compliantDeviceCount</span></span>|<span data-ttu-id="cb555-145">Int32</span><span class="sxs-lookup"><span data-stu-id="cb555-145">Int32</span></span>|<span data-ttu-id="cb555-146">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cb555-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="cb555-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb555-147">remediatedDeviceCount</span></span>|<span data-ttu-id="cb555-148">Int32</span><span class="sxs-lookup"><span data-stu-id="cb555-148">Int32</span></span>|<span data-ttu-id="cb555-149">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cb555-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="cb555-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb555-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="cb555-151">Int32</span><span class="sxs-lookup"><span data-stu-id="cb555-151">Int32</span></span>|<span data-ttu-id="cb555-152">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cb555-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="cb555-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb555-153">errorDeviceCount</span></span>|<span data-ttu-id="cb555-154">Int32</span><span class="sxs-lookup"><span data-stu-id="cb555-154">Int32</span></span>|<span data-ttu-id="cb555-155">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="cb555-155">Device error count for the setting</span></span>|
|<span data-ttu-id="cb555-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb555-156">conflictDeviceCount</span></span>|<span data-ttu-id="cb555-157">Int32</span><span class="sxs-lookup"><span data-stu-id="cb555-157">Int32</span></span>|<span data-ttu-id="cb555-158">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="cb555-158">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb555-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cb555-159">Relationships</span></span>
<span data-ttu-id="cb555-160">なし</span><span class="sxs-lookup"><span data-stu-id="cb555-160">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb555-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb555-161">JSON Representation</span></span>
<span data-ttu-id="cb555-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cb555-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



