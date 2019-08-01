---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed7427e05e8d48f090f991b45e3a46cbc2985b01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031116"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="00c10-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="00c10-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="00c10-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="00c10-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00c10-105">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="00c10-105">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="00c10-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="00c10-106">Methods</span></span>
|<span data-ttu-id="00c10-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="00c10-107">Method</span></span>|<span data-ttu-id="00c10-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="00c10-108">Return Type</span></span>|<span data-ttu-id="00c10-109">説明</span><span class="sxs-lookup"><span data-stu-id="00c10-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00c10-110">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="00c10-110">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="00c10-111">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="00c10-111">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="00c10-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="00c10-112">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="00c10-113">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="00c10-113">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="00c10-114">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="00c10-114">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="00c10-115">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="00c10-115">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="00c10-116">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="00c10-116">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="00c10-117">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="00c10-117">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="00c10-118">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="00c10-118">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="00c10-119">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="00c10-119">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="00c10-120">なし</span><span class="sxs-lookup"><span data-stu-id="00c10-120">None</span></span>|<span data-ttu-id="00c10-121">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="00c10-121">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="00c10-122">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="00c10-122">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="00c10-123">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="00c10-123">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="00c10-124">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="00c10-124">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00c10-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00c10-125">Properties</span></span>
|<span data-ttu-id="00c10-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00c10-126">Property</span></span>|<span data-ttu-id="00c10-127">型</span><span class="sxs-lookup"><span data-stu-id="00c10-127">Type</span></span>|<span data-ttu-id="00c10-128">説明</span><span class="sxs-lookup"><span data-stu-id="00c10-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00c10-129">id</span><span class="sxs-lookup"><span data-stu-id="00c10-129">id</span></span>|<span data-ttu-id="00c10-130">String</span><span class="sxs-lookup"><span data-stu-id="00c10-130">String</span></span>|<span data-ttu-id="00c10-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="00c10-131">Key of the entity.</span></span>|
|<span data-ttu-id="00c10-132">settingName</span><span class="sxs-lookup"><span data-stu-id="00c10-132">settingName</span></span>|<span data-ttu-id="00c10-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="00c10-133">String</span></span>|<span data-ttu-id="00c10-134">設定の名前</span><span class="sxs-lookup"><span data-stu-id="00c10-134">Name of the setting</span></span>|
|<span data-ttu-id="00c10-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="00c10-135">instancePath</span></span>|<span data-ttu-id="00c10-136">String</span><span class="sxs-lookup"><span data-stu-id="00c10-136">String</span></span>|<span data-ttu-id="00c10-137">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="00c10-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="00c10-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00c10-138">unknownDeviceCount</span></span>|<span data-ttu-id="00c10-139">Int32</span><span class="sxs-lookup"><span data-stu-id="00c10-139">Int32</span></span>|<span data-ttu-id="00c10-140">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="00c10-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="00c10-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00c10-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="00c10-142">Int32</span><span class="sxs-lookup"><span data-stu-id="00c10-142">Int32</span></span>|<span data-ttu-id="00c10-143">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="00c10-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="00c10-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00c10-144">compliantDeviceCount</span></span>|<span data-ttu-id="00c10-145">Int32</span><span class="sxs-lookup"><span data-stu-id="00c10-145">Int32</span></span>|<span data-ttu-id="00c10-146">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="00c10-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="00c10-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00c10-147">remediatedDeviceCount</span></span>|<span data-ttu-id="00c10-148">Int32</span><span class="sxs-lookup"><span data-stu-id="00c10-148">Int32</span></span>|<span data-ttu-id="00c10-149">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="00c10-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="00c10-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00c10-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="00c10-151">Int32</span><span class="sxs-lookup"><span data-stu-id="00c10-151">Int32</span></span>|<span data-ttu-id="00c10-152">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="00c10-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="00c10-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00c10-153">errorDeviceCount</span></span>|<span data-ttu-id="00c10-154">Int32</span><span class="sxs-lookup"><span data-stu-id="00c10-154">Int32</span></span>|<span data-ttu-id="00c10-155">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="00c10-155">Device error count for the setting</span></span>|
|<span data-ttu-id="00c10-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00c10-156">conflictDeviceCount</span></span>|<span data-ttu-id="00c10-157">Int32</span><span class="sxs-lookup"><span data-stu-id="00c10-157">Int32</span></span>|<span data-ttu-id="00c10-158">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="00c10-158">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="00c10-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="00c10-159">Relationships</span></span>
<span data-ttu-id="00c10-160">なし</span><span class="sxs-lookup"><span data-stu-id="00c10-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00c10-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00c10-161">JSON Representation</span></span>
<span data-ttu-id="00c10-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="00c10-162">Here is a JSON representation of the resource.</span></span>
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



