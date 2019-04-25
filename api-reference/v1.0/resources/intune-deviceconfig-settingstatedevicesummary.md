---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 429ee25a57383b7356948242ce39dcb45b4067ba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534746"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="f48c0-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f48c0-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="f48c0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f48c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f48c0-105">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="f48c0-105">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="f48c0-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f48c0-106">Methods</span></span>
|<span data-ttu-id="f48c0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f48c0-107">Method</span></span>|<span data-ttu-id="f48c0-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f48c0-108">Return Type</span></span>|<span data-ttu-id="f48c0-109">説明</span><span class="sxs-lookup"><span data-stu-id="f48c0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f48c0-110">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="f48c0-110">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="f48c0-111">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f48c0-111">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="f48c0-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f48c0-112">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="f48c0-113">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="f48c0-113">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="f48c0-114">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f48c0-114">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="f48c0-115">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f48c0-115">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="f48c0-116">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="f48c0-116">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="f48c0-117">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f48c0-117">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="f48c0-118">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f48c0-118">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="f48c0-119">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="f48c0-119">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="f48c0-120">なし</span><span class="sxs-lookup"><span data-stu-id="f48c0-120">None</span></span>|<span data-ttu-id="f48c0-121">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f48c0-121">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="f48c0-122">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="f48c0-122">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="f48c0-123">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f48c0-123">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="f48c0-124">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f48c0-124">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f48c0-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f48c0-125">Properties</span></span>
|<span data-ttu-id="f48c0-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f48c0-126">Property</span></span>|<span data-ttu-id="f48c0-127">型</span><span class="sxs-lookup"><span data-stu-id="f48c0-127">Type</span></span>|<span data-ttu-id="f48c0-128">説明</span><span class="sxs-lookup"><span data-stu-id="f48c0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f48c0-129">id</span><span class="sxs-lookup"><span data-stu-id="f48c0-129">id</span></span>|<span data-ttu-id="f48c0-130">String</span><span class="sxs-lookup"><span data-stu-id="f48c0-130">String</span></span>|<span data-ttu-id="f48c0-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f48c0-131">Key of the entity.</span></span>|
|<span data-ttu-id="f48c0-132">settingName</span><span class="sxs-lookup"><span data-stu-id="f48c0-132">settingName</span></span>|<span data-ttu-id="f48c0-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f48c0-133">String</span></span>|<span data-ttu-id="f48c0-134">設定の名前</span><span class="sxs-lookup"><span data-stu-id="f48c0-134">Name of the setting</span></span>|
|<span data-ttu-id="f48c0-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="f48c0-135">instancePath</span></span>|<span data-ttu-id="f48c0-136">String</span><span class="sxs-lookup"><span data-stu-id="f48c0-136">String</span></span>|<span data-ttu-id="f48c0-137">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="f48c0-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="f48c0-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f48c0-138">unknownDeviceCount</span></span>|<span data-ttu-id="f48c0-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f48c0-139">Int32</span></span>|<span data-ttu-id="f48c0-140">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f48c0-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="f48c0-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f48c0-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="f48c0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f48c0-142">Int32</span></span>|<span data-ttu-id="f48c0-143">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f48c0-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="f48c0-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f48c0-144">compliantDeviceCount</span></span>|<span data-ttu-id="f48c0-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f48c0-145">Int32</span></span>|<span data-ttu-id="f48c0-146">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f48c0-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="f48c0-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f48c0-147">remediatedDeviceCount</span></span>|<span data-ttu-id="f48c0-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f48c0-148">Int32</span></span>|<span data-ttu-id="f48c0-149">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f48c0-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="f48c0-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f48c0-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f48c0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f48c0-151">Int32</span></span>|<span data-ttu-id="f48c0-152">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f48c0-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="f48c0-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f48c0-153">errorDeviceCount</span></span>|<span data-ttu-id="f48c0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f48c0-154">Int32</span></span>|<span data-ttu-id="f48c0-155">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="f48c0-155">Device error count for the setting</span></span>|
|<span data-ttu-id="f48c0-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f48c0-156">conflictDeviceCount</span></span>|<span data-ttu-id="f48c0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f48c0-157">Int32</span></span>|<span data-ttu-id="f48c0-158">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="f48c0-158">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="f48c0-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f48c0-159">Relationships</span></span>
<span data-ttu-id="f48c0-160">なし</span><span class="sxs-lookup"><span data-stu-id="f48c0-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f48c0-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f48c0-161">JSON Representation</span></span>
<span data-ttu-id="f48c0-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f48c0-162">Here is a JSON representation of the resource.</span></span>
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



